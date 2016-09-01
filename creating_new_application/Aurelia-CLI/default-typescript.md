_Creating new application_ | _Aurelia-CLI_
# Default-TypeScript

Like all Monterey application creation wizards, the process starts with the definition of the location where the application will be persisted (Image 1). Note the red "number-markers" which indicate the sequence of mouse click needed to invoke the Files Explorer, select the folder and move to the wizard's next step.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984002/77ce6524-6add-11e6-8ed5-b33fc0fe0637.png"></img>
 <br><br>
Image 1
</p>

<br>

The next required data is the definition of the application's name (Image 2). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the name of the folder where the application "lives", this name needs to be unique. Observe that Monterey verifies each proposed application name for uniqueness.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984042/a7029464-6add-11e6-9270-dc2b38e19ba2.png"></img>
 <br><br>
Image 2
</p>

<br>

At this point (Image 3) the user is asked to choose between the several Aurelia-CLI templates (three at the time of writing this document) This number will increase as the [Aurelia-CLI command line tool](https://github.com/aurelia/cli/blob/master/README.md) evolves. In this example the Default TypeScript template was selected (marker 1) and the action continues with the Project configuration view (Image 4) as the consequence of the click on the `Next` button (marker 2)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984082/d514366e-6add-11e6-87a5-388c6e896895.png"></img>
 <br><br>
Image 3
</p>

<br>

Image 4 shows the completed project's configuration, offering the choice between `Previous` button and the `Next` button - we will take that second choice (marker 1).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984127/ffe35500-6add-11e6-8a83-53d4654b63c2.png"></img>
 <br><br>
Image 4
</p>

<br>

Now (Image 5), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

The concrete example here is very simple: run the equivalence of **`npm install`** (marker 1), by invoking npm API. This execution is triggered by the click on the Start button (Image 5). Note also that the `au run --watch` task is also scheduled for execution once `npm install` task finishes.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984209/3a639b18-6ade-11e6-872b-a1c901cb0200.png"></img>
 <br><br>
Image 5
</p>

<br>

Image 6 depicts the task `npm install` running for 4 seconds.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984278/75d9190c-6ade-11e6-9dc2-392938520b8b.png"></img>
 <br><br>
Image 6
</p>

<br>

Finally, once the `au run --watch` task is finished, you can close the Task manager, and click on the Chrome tile on the main view - resulting with the running app (Image 7)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/17984383/d08a48a8-6ade-11e6-96c8-fe1a560bc05e.png"></img>
 <br><br>
Image 7
</p>





