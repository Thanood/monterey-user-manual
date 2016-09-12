# Creating new application

Current Monterey supports eight different template types for new application creation - as shown on this image below

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18231111/38b0e324-727d-11e6-8a80-e4a824aca40d.png"></img>
 <br><br>
</p>

<br>

The Aurelia-CLI template is intentionally on the first place as it is the most popular method for Aurelia application creation, despite its initial limitation to support a single module loader -  **[RequireJS](http://requirejs.org/)**. In order to maximize the power of Aurelia-CLI, Monterey internally uses this tool, acting as its GUI - a fact that any existing Aurelia-CLI user will immediately recognize while providing the answers to Monterey's application creation Wizard.


In order to increase the spectrum of supported applications, Monterey adds all six existing **[Aurelia Navigation Skeletons](https://github.com/aurelia/skeleton-navigation)** as application creation templates. These templates present you with the "CLI-like" interface and allow you to use JSPM loader (skeleton-esnext template) and Webpack (skeleton-esnext-webpack, skeleton-typescript-webpack)



The last category of templates is accessible wia **GitHub** entry on the project templates list. As you will see, this is the most universal template as it allows you to use any existing Aurelia project existing in [GitHub](https://github.com/) as the start. Check the **[GitHub](./creating_new_application/github.html)** page of this document, as an example of such approach.


All subsections of this chapter are written the same way - lots of screen-shots and as little text as possible, provided only where the continuity between consecutive screen-shots is needed. While this approach requires a lot of redundant information - it also allows that each section is without any references or jumps to a page that would contain the information common to all subsections. 

***
***




