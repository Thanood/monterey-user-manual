_Introduction_
# Monterey and module loaders

### Introduction
As your application grows in complexity, the classic approach to loading modules via the **`<script>`** tags becomes undesirable. Just the fact that processing each **`<script>`** tag creates a new http connection explains the need that lead to the creation and use of several module loaders:

- **[RequireJS](http://requirejs.org/)**

- **[Browserify](http://browserify.org/)**

- **[Webpack](https://webpack.github.io/)**

- **[SystemJS](https://github.com/systemjs/systemjs)**

- **[WHATWG](https://whatwg.github.io/loader/)**

We recommend scanning the article **[History and Background of JavaScript Module Loaders](https://appendto.com/2016/06/the-short-history-of-javascript-module-loaders/)** to refresh / improve your understanding of the purpose and use of this technology.

### Monterey's support for module loaders

Monterey is designed to be the preferred tool for development of complex Aurelia applications, so its ability to support all module loaders is of vital importance. 

In one of its roles as the application generator (see [How ES6 Generators are changing the way we write Javascript](http://riadbenguella.com/how-es6-generators-are-changing-how-we-write-javascript/) for more information on this subject) Monterey is acting as the GUI for the [Aurelia-CLI](https://github.com/aurelia/cli) application generator. Since Aurelia-CLI supports only the RequireJS module loader, this also reduces Monterey's support for module loaders to RequireJS only. In other words: **if you wish to generate an aurelia-cli application via Monterey, you will by default use the RequireJS module loader** - until Aurelia-CLI expands its support for module loaders.

Realizing the this restriction will severely impact Monterey's functionality, declared as the tool to **[create](../../content/creating_new_application.html)** and **[maintain](../../content/managing_existing_application.html)** any Aurelia applications, we added the ability to create applications from the [Aurelia starter kits](https://github.com/aurelia/skeleton-navigation) repository:

- **[ESNext Skeletons](https://github.com/aurelia/skeleton-navigation#esnext-skeletons)**
- **[TypeScript Skeletons](https://github.com/aurelia/skeleton-navigation#typescript-skeletons)**

Going even further, we added the support to use any Aurelia application residing in GitHub - see **[this section](../../content/creating_new_application/github.html)**  for more details. This last approach will be used to provide the support for application developers that want to use Monterey to create applications with KendoUI, Materialize or Syncfusion bridges.

### Summary

1. Monterey offers two different approaches to application generation - either using the **[Aurelia-CLI application generator](../../content/creating_new_application/aurelia-cli.html)** or starting from some existing applications persisted in GitHub. 

1. If you want to use Monterey to create your application from scratch, where the application structure is defined by your answers to the Aurelia-CLI wizard, you have to use the **[Aurelia-CLI application generator](../../content/creating_new_application/aurelia-cli.html)**. This choice results with your application using the RequireJS module loader.

2. If using the RequireJS module loader is not an acceptable choice, you should consider using the above mentioned approach to create applications from the **[Aurelia starter kits repository](https://github.com/aurelia/skeleton-navigation)**  or to use any Aurelia application residing in GitHub as the starting point. This will result with applications that use SystemJS or Webpack loader, depending on the choice of the starter kit.

***
***
