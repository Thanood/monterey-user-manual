# Monterey and module loaders

As your application grows in complexity, the classic approach to loading modules via the **`<script>`** tags becomes undesirable. Just the fact that processing each **`<script>`** tag creates a new http connection explains the need that lead to the creation and use of several module loaders:

- **[RequireJS](http://requirejs.org/)**

- **[Browserify](http://browserify.org/)**

- **[Webpack](https://webpack.github.io/)**

- **[SystemJS](https://github.com/systemjs/systemjs)**

- **[WHATWG](https://whatwg.github.io/loader/)**

We recommend scanning the article **[History and Background of JavaScript Module Loaders](https://appendto.com/2016/06/the-short-history-of-javascript-module-loaders/)** to refresh / improve your understanding the purpose and use this technology