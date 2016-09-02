_Creating new application_
# skeleton-esnext-aspnetcore
Note the red "number-markers" which indicate the sequence of mouse clicks.

Start by selecting the template `skeleton-esnext-aspnetcore` (Image 1, marker 1).Then continue with accepting the definition of the location where the application will be persisted (marker 2). This action will invoke the Files Explorer, where you have to define the folder (marker 3) and click on the `Next` button (marker 3) to move to the next step.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219405/5e2df228-7137-11e6-96fe-56f8171c2d96.png"></img>
 <br><br>
Image 1
</p>

<br>

Note that Monterey will offer the name of the project, so click on the **`Next`** button (marker 1) to accept the name and move to the next step.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219535/5296fad0-7138-11e6-95a2-8f546eb78f07.png"></img>
 <br><br>
Image 2
</p>

<br>

Since the project structure is completely defined at this point (remember, Monterey has successfuly parsed all configuration information that is defined in this **[skeleton](https://github.com/aurelia/skeleton-navigation/tree/master/skeleton-esnext-aspnetcore)** folder), you are presented with Monterey's view of the project configuration (Image 3). Click on the **`Next`** button (marker 1) to proceed 

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219578/a71bfb0a-7138-11e6-99ac-31644521de27.png"></img>
 <br><br>
Image 3
</p>

<br>

Now (Image 4), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a "treeview" of check-boxes presenting the ordered list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

Click on the **`Start`** button (marker 1) initiates the application build and run workflow - as described in **[Running The App without Visual Studio](https://github.com/aurelia/skeleton-navigation/blob/master/skeleton-esnext-aspnetcore/src/skeleton/README.md#running-the-app-without-visual-studio)** article.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219629/16fcf7e4-7139-11e6-9384-e1339afba343.png"></img>
 <br><br>
Image 4
</p>

<br>

The next 6 screenshots depict the snapshots of the workflow pipeline - and probably need not additional explanations:

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219757/3a158a06-713a-11e6-9843-6eef611768dd.png"></img>
 <br><br>
Image 5
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219844/d65bb818-713a-11e6-8af7-57b44da11835.png"></img>
 <br><br>
Image 6
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219860/04fe26e2-713b-11e6-8fcd-75f0cb7590de.png"></img>
 <br><br>
Image 7
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219885/2baefbae-713b-11e6-9576-90a9faaa709a.png"></img>
 <br><br>
Image 8
</p>

<br>

Observe that the task **`dotnet run`** finished and shows the URL to access the just built application - see Image 10, below.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219920/67ecdf8c-713b-11e6-994c-707d40054267.png"></img>
 <br><br>
Image 9
</p>

<br>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18219980/ec5314b2-713b-11e6-81c5-438e03044130.png"></img>
 <br><br>
Image 10
</p>












