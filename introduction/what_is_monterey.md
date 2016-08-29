# What is Monterey

As mentioned in the Introduction chapter, it is advisable to read the **[Monterey overview](https://aurelia-ui-toolkits.gitbooks.io/monterey-overview/content/)** document before using this User maanual with intent to create new or manage existing Aurelia applications. This recommendation is the consequence of the fact that Monterey is a very unique tool, that requires some familiarization.

For reader's convenience, here is a copy of the Monterey definition from the **[Monterey overview](https://aurelia-ui-toolkits.gitbooks.io/monterey-overview/content/)** document:

Rather than creating yet another Integrated Development Environment (IDE) application, AureliaTools team's aproach  is to "integrate all development tools, including various IDEs, CLI tools, File managers into a single top level "command center" application. We named this application Monterey

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17080202/5e5d07b0-50f4-11e6-9666-95916050aad8.png"></img>
 <br><br>
Image 1
</p>
<br>

Monterey acts as a hub with Graphical User Interface which allows activation of each integrated tool (often referred to as `tile`). In this initial implementation, the application developer is in charge of "playing the tiles" in a meaningful sequence, in order to start from a blank slate and end with a working application.

Monterey's interactions with the integrated tools go beyond activation - monterey's mimics the human operator, and collects the information from one tile with the intent to pass it to the next.
<br><br>

As an **example**, check the `selecting the application template` on Image 3 in the [Creating the application]() article:

<br><br>

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17080217/e01c3e9c-50f4-11e6-90e8-18b4f234553e.png"></img>
 <br><br>
Image 2
</p>

The click on the drop-box item results with a several actions behind the scene:

- get the name of the selected item
- fetch the zip file with that name from GitHub and unzip it in the folder where the application will be stored
- unzip the file

All these actions would otherwise be done by using the browser to access the GitHub and the console application to run the command `git clone xxxx.git` - and it is the application developer who uses the clipboard to transfer the information from the browse to the console