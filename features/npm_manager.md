_Features_

<h3 style="float: left">NPM Package Manager&nbsp;&nbsp;</h3>
<p style="float: left">
  <img src="https://cloud.githubusercontent.com/assets/2712405/17079203/c0c68b92-50d6-11e6-818e-dc763b1998db.png" width="50"></img>
</p>
<p style="clear: both"></p>

**Tile:**  
![img](http://i.imgur.com/tFgJ34c.png)

**Screen:**
![screen](http://i.imgur.com/RQLwdVc.png)

<br>

**Description:**  
The main goal of the NPM Package Manager screen is to give you insight into the set of NPM dependencies of your application. Not only does Monterey display a list of dependencies, Monterey will look up the latest version and will match it with the currently installed version. By using two different colors (green and red), a visual representation of your dependencies' versions is displayed.

Currently, there are 3 actions that can be performed from the NPM package manager screen:  
![buttons](http://i.imgur.com/tLk5A2k.png)

The install button will run the equivalent of `npm install`, installing all dependencies using the version declared in package.json, without updating them. The install button can be used to install dependencies for new applications.

You may decide to update certain dependencies. After selecting these dependencies in the list and clicking the "Update selected" button, Monterey will execute the update process for the selected dependencies.

After the installation of update process has completed, you may want to refresh the list of dependencies to make sure that your dependencies are up to date. By clicking the refresh button, Monterey will read the package.json file again and will update the visual representation of your app's dependencies.

***
***