_Creating new application_
# skeleton-typescript-aspnetcore

Note the red "number-markers" which indicate the sequence of mouse clicks.

Start by selecting the template `skeleton-typescript-aspnetcore` (Image 1, marker 1).Then continue with accepting the definition of the location where the application will be persisted (marker 2). Click on the **`Next`** button (marker 3) to move to the next step.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18232933/29be0a92-72a8-11e6-9b0d-bd2e908709e2.png"></img>
 <br><br>
Image 1
</p>

<br>

Note that Monterey will offer the name of the project (marker 1), so click on the **`Next`** button (marker 2) to accept the name and move to the next step.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18232957/cb449066-72a8-11e6-92b9-92855e1e8a71.png"></img>
 <br><br>
Image 2
</p>

<br>

Since the project structure is completely defined at this point (remember, Monterey has successfuly parsed all configuration information that is defined in this **[skeleton](https://github.com/aurelia/skeleton-navigation/tree/master/skeleton-typescript-aspnetcore)** folder), you are presented with Monterey's view of the project configuration (Image 3). Click on the **`Next`** button (marker 1) to proceed.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18232981/56d157ae-72a9-11e6-8c7b-47549b047fca.png"></img>
 <br><br>
Image 3
</p>

<br>

Now (Image 4), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a "treeview" of check-boxes presenting the ordered list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

There are several details that deserve additional comments:

- Monterey "knows" that Typescript apps need one additional task - `typings install` (marker 1)
- Monterey "understands" the structure of aspnet.core project has to run the `dotnet restore` task (marker 2)
- Both `gulp watch` and `dotnet run` tasks need to be running in order for this app to work (markers 3 and 4)

Click on the **`Start`** button (marker 5) initiates the application build and run workflow - as described in **[Running The App without Visual Studio](https://github.com/aurelia/skeleton-navigation/blob/master/skeleton-typescript-aspnetcore/src/skeleton/README.md#running-the-app-without-visual-studio)** article.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18232992/97d8fcfc-72a9-11e6-8a3c-74a60a220af2.png"></img>
 <br><br>
Image 4
</p>

<br>

The next 6 screenshots depict the snapshots of the workflow pipeline - and probably need not additional explanations.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233093/01315526-72ac-11e6-828d-4a65aa5a2c05.png"></img>
 <br><br>
Image 5
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233101/232ad18e-72ac-11e6-85f2-90d1d27609e8.png"></img>
 <br><br>
Image 6
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233105/48047ea6-72ac-11e6-8184-684e42c1bd98.png"></img>
 <br><br>
Image 7
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233117/9f3c7e80-72ac-11e6-8524-cae72f78b39d.png"></img>
 <br><br>
Image 8
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233126/d05e1fb4-72ac-11e6-80f3-392820c61028.png"></img>
 <br><br>
Image 9
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233133/f747fb04-72ac-11e6-9beb-0d986fa524f9.png"></img>
 <br><br>
Image 10
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18233144/29c567ce-72ad-11e6-8438-8ffca19776b9.png"></img>
 <br><br>
Image 11
</p>






