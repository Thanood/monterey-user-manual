# Default-ESNext

Like all Monterey application creation wizards, the process starts with the definition of the location where the application will be persisted (Image 1). Note the red "number-markers" which indicate the sequence of mouse click needed to invoke the Files Explorer, select the folder and move to the wizard's next step.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17971413/c562a758-6aa8-11e6-8d9a-fbe1a1d0cad8.png"></img>
 <br><br>
 Image 1
</p>

<br>

The next required data is the definition of the application's name (Image 2). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the name of the folder where the application "lives", this name needs to be unique. Observe that Monterey verifies each proposed application name for uniqueness.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17971502/22d9920c-6aa9-11e6-88ec-d3f2815174bc.png"></img>
 <br><br>
   Image 2
</p>

<br>

At this point (Image 3) the user is asked to choose between the several Aurelia-CLI templates (three at the time of writing this document; this number will increase as the [Aurelia-CLI command line tool](https://github.com/aurelia/cli/blob/master/README.md) evolves. 

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17971561/53178bc2-6aa9-11e6-8f51-3f9a8a5f3189.png"></img>
 <br><br>
  Image 3
</p>

<br>

The selected "Default ESNext" template is completely defined at this point and Monterey creates the **Project configuration** summary page (Image 4). You can go back through all steps that led to the Project configuration definition, if you realize that some of the specifications in any of these previous steps are not correct

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17971613/8bab32f4-6aa9-11e6-9eb5-c214e1d91606.png"></img>
 <br><br>
  Image 4
</p>

<br>

At this point we reached the most important step of the Monterey wizard - page where will eventually reside the **Monterey workflow plugin**. At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

The concrete example here is very simple: run the equivalence of `npm install` and `jspm install` tasks executed in the serial fashion in the console, by invoking npm and jspm API. This execution is triggered by the click on the `Start` button (Image 5)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17971660/c019c816-6aa9-11e6-820b-f9496fe7b917.png"></img>
 <br><br>
  Image 5
</p>

<br>

Click on the `Start` button on Image 5 above causes the switch of the Monterey's view - from the "workflow" to the Monterey **Task manager** (Image 6). This is the most often used Monterey integrated tool, which is the controlling and management entity for handling all running Monterey applications. At this time we have a single application (`Default-ESNext`) running, and you can see that the currently running task is `NPM install`, which will be followed by two more tasks. You can also see the embedded console showing the line-by-line progress of the currently running .`NPM install` task.

Note that Monterey is designed to be able to run many tasks in parallel - this view is restricted to show only the information for the selected project (`Default-ESNext`).

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17977605/5d77cd54-6ac0-11e6-8866-7419539431df.png"></img>
 <br><br>
  Image 6
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17981382/8225b0f6-6ad1-11e6-9c32-3404398a1d8c.png"></img>
 <br><br>
 Image 7
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17981545/22c51646-6ad2-11e6-9c50-d0238a821daf.png"></img>
 <br><br>
 Image 8
</p>












