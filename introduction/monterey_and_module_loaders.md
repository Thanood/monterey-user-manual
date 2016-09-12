# Monterey and module loaders

### Introduction
As your application grows in complexity, the classic approach to loading modules via the **`<script>`** tags becomes undesirable. Just the fact that processing each **`<script>`** tag creates a new http connection explains the need that lead to the creation and use of several module loaders:

- **[RequireJS](http://requirejs.org/)**

- **[Browserify](http://browserify.org/)**

- **[Webpack](https://webpack.github.io/)**

- **[SystemJS](https://github.com/systemjs/systemjs)**

- **[WHATWG](https://whatwg.github.io/loader/)**

We recommend scanning the article **[History and Background of JavaScript Module Loaders](https://appendto.com/2016/06/the-short-history-of-javascript-module-loaders/)** to refresh / improve your understanding the purpose and use this technology.

### Monterey's support for module loaders

Monterey is designed to be the preferred tool for development of complex Aurelia applications, so its ability to support all module loaders is of vital importance.

In its role as the application generator (see [How ES6 Generators are changing the way we write Javascript](http://riadbenguella.com/how-es6-generators-are-changing-how-we-write-javascript/) for more information on this subject) Monterey is acting as the GUI for the [Aurelia-CLI](https://github.com/aurelia/cli) application generator. Since Aurelia-CLI supports only the RequireJS module loader, this also reduces Monterey's support for module loaders to RequireJS only. In other words: **if you wish to use Monterey as the application generator, you can only create applications that use RequireJS module loader**.

Realizing the this restriction will severely impact Monterey's functionality, declared as the tool to **[create](../creating_new_application.html)** and **[maintain](../managing_existing_application.html)** any Aurelia applications, we added the ability to create applications from the [Aurelia starter kits](https://github.com/aurelia/skeleton-navigation) repository:

- **[ESNext Skeletons](https://github.com/aurelia/skeleton-navigation#esnext-skeletons)**
- **[TypeScript Skeletons](https://github.com/aurelia/skeleton-navigation#typescript-skeletons)**

Going even further, 

