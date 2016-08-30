_Features_

<h3 style="float: left">JSPM Package Manager&nbsp;&nbsp;</h3>
<p style="float: left">
  <img src="https://cloud.githubusercontent.com/assets/2712405/17079208/081249b4-50d7-11e6-8c67-77c55ef8b0ea.png" width="50"></img>
</p>
<p style="clear: both"></p>

**Tile:**  
![tile](http://i.imgur.com/eRH6bYH.png)

<br>

**Screen:**
<br>
<p align=center>
  <img src="http://i.imgur.com/YTp9kFs.png"></img>
 <br><br>
Image 1
</p>


<br>

**Description**:  
Without Monterey, you have to open the `config.js` file in an editor to see which dependencies a JSPM application has. It is also impossible to know which dependencies are out of date.

Monterey gives you insight into the JSPM dependencies of your application. It not only shows the dependencies in a list, it also looks up the latest version of each dependency and will let you know which dependencies can be updated.

<br>
<p align=center>
  <img src="http://i.imgur.com/AzE9ZfX.png"></img>
 <br><br>
Image 2
</p>

<br>

The JSPM package manager screen allows you to install and update packages. If you created a new Aurelia project, then JSPM dependencies are not yet installed. The **`Install`** button in Monterey will install these dependencies for you. If you want to update all dependencies (but only dependencies that have a version above 1.0.0), then you can use the **`Update all`** button. If you want to update packages with versions below 1.0.0, then you can select these packages and click the **`Update selected (ignore semver)`** button.

<br>

**Forks**  
We have noticed that JSPM forks often cause issues. As such, we have taught Monterey to detect forks, and it will display a big warning message whenever forks are detected:

<p align=center>
  <img src="http://i.imgur.com/Y7146N7.png"></img>
 <br><br>
Image 3
</p>


<br>
Monterey also gives the user advice on how to resolve these forks:


<p align=center>
  <img src="http://i.imgur.com/wZ9zCpx.png"></img>
 <br><br>
Image 4
</p>


***
***


