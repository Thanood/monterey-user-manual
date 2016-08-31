_Creating new application_ | _Aurelia-CLI_
# Custom
Like all Monterey application creation wizards, the process starts with the definition of the location where the application will be persisted (Image 1). Note the red "number-markers" which indicate the sequence of mouse click needed to invoke the Files Explorer (marker 1) navigate it to the right location (marke3 2), select the folder (marker 3) and by that, define the location path.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986728/234d84be-6aea-11e6-8320-0c10376ef56c.png"></img>
 <br><br>
Image 1
</p>

<br>

The next required data is the definition of the application's name (Image 2). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the name of the folder where the application "lives", this name needs to be unique. Observe that Monterey verifies each proposed application name for uniqueness.

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

This is the first in the series of Aurelia-CLI custom template additional specifications (Image 4) where we selected the `ASP.NET Core` template (see [this site](http://www.asp.net/core) for more details). Click on the `Next` button leads to to the Transpiler selection (Image 5)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986829/b45245a8-6aea-11e6-9793-cf35c6ae3620.png"></img>
 <br><br>
Image 4
</p>

<br>

Transpiler selection dialog (Image 5). We chose `Babel` and continue to Image 6 clicking on the `Next` button (marker 2).

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

Image 8 depicts the complete project configuration definition, allowing the user to verify that the process so far resulted with the intended outcome (the `previous` button is provided for the case where something needs to be changed). In our situation, click on the `Next` button (marker 1).
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17986961/5b4b6d80-6aeb-11e6-90c8-d2d4922f137b.png"></img>
 <br><br>
Image 8
</p>

<br>

At this point we reached the most important step of the Monterey wizard - page where will eventually reside the **Monterey workflow plugin** (Image 9). At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

Unlike other examples showing how to create the application from a template, in this situation we disabled the offered workflow (marker 1) which would schedule the sequence of `npm install` and `au run --watch` for execution, so we can show how to do this manually. So, we proceed with the click on the `close` button (marker 2), knowing that the application project has been created.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987075/fcf8937e-6aeb-11e6-9dc3-5f511a4a8e66.png"></img>
 <br><br>
Image 9
</p>

<br>

Image 10 presents Monterey's main view indicating our `custom-1` project as active (shown in red). Notice the `Show irrrelevant tiles` check-box (marker 1) and **set** it to checked state.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987184/9031b0f8-6aec-11e6-8620-235c930e533a.png"></img>
 <br><br>
Image 10
</p>

<br>


Here (Image 11) we can see the effect of requesting to see `irrelevant tiles` which are shown with diagonal stripes - indicating that all these tiles cannot play any role in this specific project. This proves that Monterey has the ability to recognize any project's type (Aurelia-CLI in our case).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987221/cdd13780-6aec-11e6-993c-767339ef3a0b.png"></img>
 <br><br>
Image 11
</p>

<br>

Now, we have the opportunity to verify the fact that all Monterey tiles (plugins) are indeed integrated in the sense that they are invoked by passing the relevant context data to them. Click on the `Files Explorer` tile invokes the platform specific files viewer with the definition of the project's folder path. Dismiss the files view as proper for the platform (marker 3).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987264/02271f7c-6aed-11e6-9e1c-a9be6c35f679.png"></img>
 <br><br>
Image 12
</p>

<br>

In order to build this project manually (as we elected to do on Image 9, above), we need to run the `npm install` task - by clicking on the NPM tile (Monterey main view - Image 11). Observe the grid presenting the application dependencies obtained by **`parsing`** the `package.json` file of this project (generated by Aurelia-CLI behind the scenes). 

Click on the `Install` button (marker 1), will start the task and the view will show the `npm install` task running (Image 14). 

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987306/323a0508-6aed-11e6-89da-636cce6e1204.png"></img>
 <br><br>
Image 13
</p>

<br>

This screenshot (Image 14, below) is a snapshot of the running `npm install` task, with the embedded console showing the details of this running task.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987327/5569740a-6aed-11e6-9484-41bd3a7089cb.png"></img>
 <br><br>
Image 14
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987362/8e974856-6aed-11e6-8e7b-699e376887b8.png"></img>
 <br><br>
Image 15
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987392/bc070e20-6aed-11e6-976c-4aa1392ed057.png"></img>
 <br><br>
Image 16
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987419/e97b3958-6aed-11e6-9306-3d347848437b.png"></img>
 <br><br>
Image 17
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987453/1281d9c4-6aee-11e6-8215-03378c0dfe59.png"></img>
 <br><br>
Image 18
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987505/446edefa-6aee-11e6-81f8-8136b563b869.png"></img>
 <br><br>
Image 19
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987536/6dbc0e68-6aee-11e6-8d04-0842d3aadc93.png"></img>
 <br><br>
Image 20
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987589/aa726d70-6aee-11e6-92f9-8f2a731ae00a.png"></img>
 <br><br>
Image 21
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987630/f4118ccc-6aee-11e6-8b91-e5ab16aaa08b.png"></img>
 <br><br>
Image 22
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17987661/1b0f1d1c-6aef-11e6-88bb-dcfcff04225d.png"></img>
 <br><br>
Image 23
</p>

***
***












