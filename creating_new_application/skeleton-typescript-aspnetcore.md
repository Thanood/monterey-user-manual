_Creating new application_
# skeleton-typescript-aspnetcore
Note the red "number-markers" which indicate the sequence of mouse clicks.

Start by selecting the template `skeleton-esnext-aspnetcore` (Image 1, marker 1).Then continue with the definition of the location where the application will be persisted (marker 2). This action will invoke the Files Explorer, where you have to define the folder (marker 3) and click on the `Select folder` button (marker 4) to define the location where the application will be stored.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18028256/f990485a-6c47-11e6-8a89-741920ca8a02.png"></img>
 <br><br>
Image 1
</p>

<br>

Note that Monterey will offer the name of the project, so click on the `Next` button (marker 1) to accept the name and move to the next step.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18028266/2539871e-6c48-11e6-8611-9290ee5226de.png"></img>
 <br><br>
Image 2
</p>

<br>

Since the project structure is completely defined at this point (remember, Monterey has successfuly parsed all configuration information that is defined in this **[skeleton](https://github.com/aurelia/skeleton-navigation/tree/master/skeleton-typescript-aspnetcore)** folder), you are presented with Monterey's view of the project configuration (Image 3). Click on the `Next` button (marker 1) to proceed 

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029733/640b26ac-6c6e-11e6-864e-1bfb984e236b.png"></img>
 <br><br>
Image 3
</p>

<br>

Now (Image 4), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

The concrete example here is simple: run the equivalence of **`npm install`** (marker 1), and **`jspm install`** by invoking npm and jspm API (action different from invoking the same service using the console). The last "workflow" step is of course **`gulp watch`**

This execution is triggered by the click on the Start button (marker 2).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029741/95d167a0-6c6e-11e6-846f-cd0521001f90.png"></img>
 <br><br>
Image 4
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029747/c45ce194-6c6e-11e6-919f-c1043b02672d.png"></img>
 <br><br>
Image 5
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029752/eb70ecda-6c6e-11e6-8a35-299f6925ed7b.png"></img>
 <br><br>
Image 6
</p>

***

### Next few screens show failed attempts to run `gulp watch` 

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029871/6dc36a2a-6c72-11e6-891d-69b04d29503d.png"></img>
 <br><br>
Image 7
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029875/9cdc74d2-6c72-11e6-94b2-5000ab71e6a6.png"></img>
 <br><br>
Image 8
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18029878/c20e874a-6c72-11e6-891c-c30c0d043b5c.png"></img>
 <br><br>
Image 9
</p>











