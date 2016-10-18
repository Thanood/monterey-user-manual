_Creating new application_ | _GitHub_ | _CM tutorial - Materialize edition_
# Differences from the original version

This document is not a tutorial on Materialize bridge base application development - check [Aurelia Materialize Bridge](https://aurelia-ui-toolkits.github.io/demo-materialize) to learn more. Similarly this document does not teach you about [RequireJS module loader](http://requirejs.org/). Instead it will show you how to manually enhance the [original Contact Manager tutorial](http://aurelia.io/hub.html#/doc/article/aurelia/framework/latest/contact-manager-tutorial) to use Materialize bridge and render its view using Aurelia Materialize components, instead of using Bootstrap.

The source code for for the Contact Manager tutorial - Materialize edition is [here](https://github.com/aurelia-ui-toolkits/cm-bridges/tree/master/materialize), and this article will describe the details of changes applied to the **application configuration files**.

### 1. [package.json](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/package.json)
Add reference to aurelia-materialize-bridge and add three npm scripts (see below for a copy&paste source).

![image](https://cloud.githubusercontent.com/assets/677826/19490538/d2296afc-956f-11e6-8848-dbfb319369ce.png)

Copy the script lines from here:

```json
  "scripts": {
    "materialize": "node node_modules/requirejs/bin/r.js -o tools/rbuild.js",
    "postinstall": "npm run materialize",
    "postmaterialize": "au prepare-materialize"
  },
```

<br>

These scripts create an AMD-compatible version of Materialize and copy fonts to your app root. See step 2 on how to obtain these scripts.

<br>

### 2. [materialize-scripts](https://github.com/aurelia-ui-toolkits/cm-bridges/tree/master/materialize/tools)

#### Creating an AMD-compatible Materialize version

*Why is this necessary?* - The original Materialize doesn't play well with AMD loaders. As Aurelia-CLI uses `requirejs` (an AMD loader), the sources have to be adopted to be able to run in an AMD environment.

Instead of using a fork, [someone came up with a brilliant idea](https://github.com/Dogfalo/materialize/issues/634#issuecomment-113213629) to create an AMD package of Materialize "on the fly". Someone else [created a repo out of this idea](https://github.com/noodny/materializecss-amd).

- Create a folder `tools` in your project root:

![image](https://cloud.githubusercontent.com/assets/677826/19490757/a428f928-9570-11e6-933d-3ca96fdb1ce2.png)

<br>

- Copy the two files [rbuild.js](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/tools/rbuild.js) and [materialize-css.js](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/tools/materialize-css.js) into that folder.

<br>

#### Creating a build task to copy fonts and CSS

*Why is this necessary?* - Aurelia-CLI doesn't support bundling fonts at the time of writing this article. When running the app without this change, you will get a bunch of `404 - not found` errors when the loads css from Materialize.

These css files contain references to the Roboto font. If not copied, these fonts are still in `node_modules` which is not accessible by the application.

<br>

- Open the folder `aurelia_project/tasks` and create a file `prepare-materialize.js`
- Add the following content to this file:

```javascript
import gulp from 'gulp';
import merge from 'merge-stream';
import * as project from '../aurelia.json';
import path from 'path';

export default function prepareMaterialize() {
  let source = 'node_modules/materialize-css';

  let taskCss = gulp.src(path.join(source, 'dist/css/materialize.min.css'))
    .pipe(gulp.dest(path.join(project.platform.output, '../', 'styles')));

  let taskFonts = gulp.src(path.join(source, 'dist/fonts/roboto/*'))
    .pipe(gulp.dest(path.join(project.platform.output, '../', 'fonts/roboto')));

  return merge(taskCss, taskFonts);
}
```

### 3. [aurelia.json](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/aurelia_project/aurelia.json)
- Set `"stub: false` in the loader section:
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/19351777/15f7134a-912b-11e6-8893-00aa320518fa.png"></img>
 <br><br>
Image 2
</p>

- Add a new bundle `materialize-bundle.js` to `aurelia.json`: 
 ```json
      {
        "name": "materialize-bundle.js",
        "dependencies": [
          "jquery",
          {
            "name": "materialize-css",
            "path": "../node_modules/materialize-css/dist",
            "main": "js/materialize.amd",
            "deps": [
              "jquery"
            ],
            "resources": [
              "css/materialize.css"
            ],
            "exports": "Materialize"
          },
          {
            "name": "aurelia-materialize-bridge",
            "path": "../node_modules/aurelia-materialize-bridge/dist/amd",
            "main": "index",
            "deps": [
              "jquery"
            ],
            "resources": [
              "**/*.{css,html}"
            ]
          }
        ]
      }
 ```

<br>

**Note**: the rest of the changes required to change the application rendering are of course specific to  Aurelia Materialize components. Check the following files for details:

- [contact-list](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/src/contact-list.html) replaced the original bootstrap list with a Materialize collection.
- [contact-detail](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/src/contact-detail.html) replaced the contact detail panel with a Materialize card
- [app.html](https://github.com/aurelia-ui-toolkits/cm-bridges/blob/master/materialize/src/app.html) replaced bootstrap's nav-bar with a Materialize version

In the former two files the original content is still present for direct comparison.

***
***





