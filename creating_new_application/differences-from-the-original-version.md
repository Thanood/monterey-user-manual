\_Creating new application\_ \| \_GitHub\_ \| \_CM tutorial - KendoUI edition\_

\# Differences from the original version



This document is not a tutorial on KendoUI bridge base application development - check \[Aurelia KendoUI Bridge\]\(https:\/\/aurelia-ui-toolkits.github.io\/demo-kendo-beta\) to learn more. Similarly this document does not teach you about \[RequireJS module loader\]\(http:\/\/requirejs.org\/\). Instead it will show you how to manually enhance the \[original Contact Manager tutorial\]\(http:\/\/aurelia.io\/hub.html\#\/doc\/article\/aurelia\/framework\/latest\/contact-manager-tutorial\) to use KendoUI bridge and render its view using Aurelia KendoUI components, instead of using Bootstrap.



The source code for for the Contact Manager tutorial - KendoUI edition is \[here\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/tree\/master\/kendoui\), and this article will describe the details of changes applied to the \*\*application configuration files\*\*.



\#\#\# 1. \[package.json\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/package.json\)

Add references to as specific versions of jQuery and aurelia-kendoui-bridge

&lt;p align=center&gt;

 &lt;img src="https:\/\/cloud.githubusercontent.com\/assets\/2712405\/19351324\/4fdaf966-9129-11e6-845d-28063a4521a1.png"&gt;&lt;\/img&gt;

 &lt;br&gt;&lt;br&gt;

Image 1

&lt;\/p&gt;



&lt;br&gt;



\#\#\# 2. \[aurelia.json\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/aurelia\_project\/aurelia.json\)

- Set \`"stub: false\` in the loader section:

&lt;p align=center&gt;

 &lt;img src="https:\/\/cloud.githubusercontent.com\/assets\/2712405\/19351777\/15f7134a-912b-11e6-8893-00aa320518fa.png"&gt;&lt;\/img&gt;

 &lt;br&gt;&lt;br&gt;

Image 2

&lt;\/p&gt;



- Add the code

 \`\`\`

 {

 "name": "aurelia-kendoui-bridge",

 "path": "..\/node\_modules\/aurelia-kendoui-bridge\/dist\/amd",

 "main": "index"

 }

 \`\`\`

 to the \[dependencies section\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/aurelia\_project\/aurelia.json\#L94-L160\)



&lt;p align=center&gt;

 &lt;img src="https:\/\/cloud.githubusercontent.com\/assets\/2712405\/19351954\/ccb4eac6-912b-11e6-95ca-87f92980a7e1.png"&gt;&lt;\/img&gt;

 &lt;br&gt;&lt;br&gt;

Image 3

&lt;\/p&gt;



&lt;br&gt;



\*\*Note\*\*: the rest of the changes required to change the application rendering are of course specific to Aurelia KendoUI components. Check the following files for details:



- \[contact-list\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/src\/contact-list.html\) replaced the original bootstrap list with KendoUI panel bar.



- \[app\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/src\/app.html\) added KendoUI tab strip



- new component \[contact-grid\]\(https:\/\/github.com\/aurelia-ui-toolkits\/cm-bridges\/blob\/master\/kendoui\/src\/contact-grid.html\).



\*\*\*

\*\*\*



