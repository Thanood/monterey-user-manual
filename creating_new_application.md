# Creating new application

Current Monterey supports several different templates for new application creation - as shown on this image below

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18060529/b6dfddc6-6dec-11e6-9058-68548acd89f0.png"></img>
 <br><br>
Image 1
</p>
<br><br>
The Aurelia-CLI template is intentionally on the first place as it is the most popular method for Aurelia application creation, despite its initial limitation to support a single module loader (RequireJS). In order to maximize the power if Aurelia-CLI, Monterey completely depends on this tool, acting as its Visual "proxy" - a fact that any existing Aurelia-CLI user will immediately recognize while providing the answers to Monterey presenting the application creation Wizard.

In order to increase the spectrum of supported applications, Monterey adds all six existing **[Aurelia Navigation Skeletons](https://github.com/aurelia/skeleton-navigation)** as application creation templates. These templates present you with the "CLI-like" interface and offer you to use JSPM loader (skeleton-esnext template)

The last category of templates is accessible wia **ZIP** entry on the project templates list. As you will see, this is the most universal template as it allows you to use any existing Aurelia project as the base. As the example of that template use, please check the [ZIP](./ZIP.html) page of this document.




