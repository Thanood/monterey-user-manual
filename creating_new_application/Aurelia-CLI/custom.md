_Creating new application_ | _Aurelia-CLI_
# Custom
_Note the red "number-markers" which indicate the sequence of mouse clicks needed to invoke Monterey UI elements._

Like all Monterey application creation wizards, the process starts with the choice of the template (Image 1, marker 1), followed by the definition of the location where the application will be persisted (Image 1):
- select the folder (marker 2)
- navigate it to the right location (marker 3) 
- select the folder (marker 4) 

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18404870/4c7e99d6-76bb-11e6-9c9d-bb617058e8b5.png"></img>
 <br><br>
Image 1
</p>

<br>

The next required data is the definition of the application's name (Image 2). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the **name of the folder** where the application "lives", this name needs to be unique and should not contain blank spaces. Observe that Monterey verifies each proposed application name for uniqueness.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986764/5f872ade-6aea-11e6-8fd4-7ffb08f3a999.png"></img>
 <br><br>
Image 2
</p>

<br>

At this point (Image 3) the user is asked to choose between the several Aurelia-CLI templates (three at the time of writing this document; this number will increase as the [Aurelia-CLI command line tool](https://github.com/aurelia/cli/blob/master/README.md) evolves.In this case we will select the Custom template (marker 1), which is currently the most customizable Aurelia-CLI template.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986798/8f3c7e0a-6aea-11e6-83b7-0fa3c9250952.png"></img>
 <br><br>
Image 3
</p>

<br>

This is the first in the series of Aurelia-CLI custom template additional specifications (Image 4) where we selected the `Default` template (marker 1). Click on the `Next` button (marker 2) leads to to the Transpiler selection (Image 5)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18405079/ebbbc8ba-76bc-11e6-87cd-da361ef50684.png"></img>
 <br><br>
Image 4
</p>

<br>

Transpiler selection dialog (Image 5). We chose `Babel` (marker 1) and continue to Image 6 clicking on the **`Next`** button (marker 2).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986865/dc0b6070-6aea-11e6-8a87-72c8692a5e89.png"></img>
 <br><br>
Image 5
</p>

<br>

Style selection dialog - for simplicity we pick the standard CSS with no pre-processor (marker 1). Click on the `Next` button (marker 2) leads us to Image 7.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986897/067f9592-6aeb-11e6-9041-705d93ebdf6e.png"></img>
 <br><br>
Image 6
</p>

<br>

Testing selection dialog (Image 7) where we select the `Yes` choice (marker 1). Click on the `Next` button (marker 2) leads us to Image 8.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986934/2dd77218-6aeb-11e6-99ca-e2bef5583ca8.png"></img>
 <br><br>
Image 7
</p>

<br>

Image 8 shows the selection of the Editor / IDE from the list of alternatives that are defined using the  **[App Launcher plugin](https://aurelia-ui-toolkits.gitbooks.io/monterey-user-manual/content/features/app_launcher.html)** (tile). For this example, we will select the **[Atom](https://atom.io/)** editor (marker 1) and move ahead by the clock on the **`Next`** button (marker 2).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18405175/ce8cdb52-76bd-11e6-8018-5616fdbd8c2b.png"></img>
 <br><br>
Image 8
</p>

Image 9 depicts the complete project configuration definition, allowing the user to verify that the process so far resulted with the intended outcome (the `previous` button is provided for the case where something needs to be changed). In our situation, click on the `Next` button (marker 1).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18406000/77904b4c-76c5-11e6-9432-38b054f7a11f.png"></img>
 <br><br>
Image 9
</p>
<br>

<br>

At this point we reached the most important step of the Monterey wizard - page where will eventually reside the **Monterey workflow plugin** (Image 10). At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

Unlike other examples showing how to create the application from a template, in this situation we accepted the complete offered workflow (marker 1) which will schedule the sequence of **`npm install`** and **`au run --watch`** for execution. Finish this wizard with the click on the **`Start`** button (marker 2), resulting with the activation of the **[Task manager]()** plugin.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18406039/cfa7e614-76c5-11e6-9e94-8e4ccb3d27bd.png"></img>
 <br><br>
Image 10
</p>
<br>

<br>

Image 11 presents Monterey's main view indicating our `custom-1` project as active (shown in red). Notice the `Show irrrelevant tiles` check-box (marker 1) and **set** it to checked state.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987184/9031b0f8-6aec-11e6-8620-235c930e533a.png"></img>
 <br><br>
Image 11
</p>

<br>


Here (Image 12) we can see the effect of requesting to see `irrelevant tiles` which are shown with diagonal stripes - indicating that all these tiles cannot play any role in this specific project. This proves that Monterey has the ability to recognize any project's type (Aurelia-CLI in our case). See **[Monterey technical documentation - Project detection](https://aurelia-ui-toolkits.gitbooks.io/monterey-technical-documentation/content/project_detection.html)** for more details.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987221/cdd13780-6aec-11e6-993c-767339ef3a0b.png"></img>
 <br><br>
Image 12
</p>

<br>

Now, we have the opportunity to verify the fact that all Monterey tiles (plugins) are indeed integrated in the sense that they are invoked by passing the relevant context data to them. Click on the `Files Explorer` tile invokes the platform specific files viewer with the definition of the project's folder path. Dismiss the files view as proper for the platform (marker 3).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987264/02271f7c-6aed-11e6-9e1c-a9be6c35f679.png"></img>
 <br><br>
Image 13
</p>

<br>

In order to build this project manually (as we elected to do on Image 10, above), we need to run the `npm install` task - by clicking on the NPM tile (Monterey main view - Image 11). Observe the grid presenting the application dependencies obtained by **`parsing`** the `package.json` file of this project (generated by Aurelia-CLI behind the scenes). 

Click on the `Install` button (marker 1), will start the task and the view will show the `npm install` task running (Image 15). 

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987306/323a0508-6aed-11e6-89da-636cce6e1204.png"></img>
 <br><br>
Image 14
</p>

<br>

This screenshot (Image 14, below) is a snapshot of the running `npm install` task, with the embedded console showing the details of this running task.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987327/5569740a-6aed-11e6-9484-41bd3a7089cb.png"></img>
 <br><br>
Image 15
</p>

<br>

As the `npm install` task typically takes several minutes, we provided a cool little game activated by a click on the `T-rex` button (bottom right corner of the Task manager view

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987362/8e974856-6aed-11e6-8e7b-699e376887b8.png"></img>
 <br><br>
Image 16
</p>

<br>

This "CPU load graph" (Image 17) demonstrates how "heavy" is a typical load imposed by running `npm` application.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987392/bc070e20-6aed-11e6-976c-4aa1392ed057.png"></img>
 <br><br>
Image 17
</p>

<br>

After 239 seconds (on a very fast machine) the NPM install task finally ended (Image 18). Close the Task manager (marker 1), so we can see what changed as the consequence of running NPM install.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987419/e97b3958-6aed-11e6-9306-3d347848437b.png"></img>
 <br><br>
Image 18
</p>

<br>

At this point, the NPM manager is a lot "smarter" and provides the insight into the set of NPM dependencies of this application. Besideds displaying the list of dependencies, Monterey will look up the latest version and will match it with the currently installed version. By using two different colors (green and red), a visual representation of your dependencies' versions is displayed.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987453/1281d9c4-6aee-11e6-8215-03378c0dfe59.png"></img>
 <br><br>
Image 19
</p>

<br>

Now, let's switch back to the main view, so we can (again) invoke the Task manager (Image 20, marker 1) with the intent to run the just built application.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987505/446edefa-6aee-11e6-81f8-8136b563b869.png"></img>
 <br><br>
Image 20
</p>

<br>

We can see that the NPM install task finished (Image 21, marker 1 - something we already knew), so select the `au run --watch` task (marker 2) from the list of meaningful tasks in this context and click on the `Start this task` button (marker 3) (indicating that we want to start the selected task).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987536/6dbc0e68-6aee-11e6-8d04-0842d3aadc93.png"></img>
 <br><br>
Image 21
</p>

<br>

This Task manager view (Image 22) shows that the application is running (`au run --watch`), successfully started 4 seconds ago. 

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987589/aa726d70-6aee-11e6-92f9-8f2a731ae00a.png"></img>
 <br><br>
Image 22
</p>

___more to come___

***
***












