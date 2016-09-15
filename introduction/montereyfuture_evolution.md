_Introduction_
# A brief peek in the future of Monterey
## _Important note_
___This text is provided solely to facilitate the discussions with Monterey users. We are in no way implying that we will do all of these extenstions, nor that we might not add some completely different features - if these turn out to be deemed important by a large enough group of users.___

### 1. Configuration management
There is a rumor that Monterey started as Aurelia Configuration Tool (aka ACT), application designed to assist Aurelia developers with tedious and complex pedestrian work associated with configuration details of module managers like **[npm](https://www.npmjs.com/)** and module loaders like **[jspm](http://jspm.io/)** and **[webpack](http://webpack.github.io/docs/)**.

While Monterey is a lot more complex tool today (see **[What is Monterey](../introduction/what_is_monterey.html)** for details), application configuration assistence is one of the key Monterey features (see **[npm manager](../features/npm_manager.html)** and **[jspm manager](../features/jspm_manager.html)** for details) in the context of Aurelia applications management.

Here are a few ideas from the general area of configuration management we are considering at the moment

- Upgrading an existing application to the next version of Aurelia.

- Downgrading an existing application to some previous version of Aurelia (say for debugging purposes).

- Analyzing dependencies on other modules and eliminating some that are not used.

### 2. Deeper and richer integration with other development tools
Current integration level is simple and shallow - see **[Image 10 in the Creating new application, skeleton typescript aspnet.core](../creating_new_application/skeleton-typescript-aspnetcore.html)** as an example: after the application build step has finished, we could close the Task manager view and click on the Chrome tile to see the running application (Chrome will be passed the URL of `http://localhost:5000`, specific for the building pipeline of that application.)

New features would include:

- Invoking VS code, Webstorm IDE or Chrome developer tools for a debugging section directly from Sublime text editor.

- Expanding the current simple implementation of the application `build and run` workflow to support specific profiles like application integrator.

- ...

### 3. Complete life-cycle management (aka "DevOps")

While expansion in the direction of item 2 above will reach quite deep, we believe that enabling Monterey to have intelligent integration with **[Docker](https://www.docker.com/)** will completely fulfill the mantra BUILD, SHIP, RUN. 

This feature will equaly support **[kubernetes](http://kubernetes.io/)** in the context of the planned partnership with several relevant vendors.




