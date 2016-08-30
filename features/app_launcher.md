_Features_

<h3 style="float: left">App launchers</h3>
<p style="float: left">
  <img src="https://cloud.githubusercontent.com/assets/2712405/17079177/0f3c9aa6-50d6-11e6-82c3-0e30d92ff5f2.png" width="50"></img>
</p>
<p style="clear: both"></p>

**Tile:**  
![tile](http://i.imgur.com/mWoUbnk.png)

**Screen:**
![img](http://i.imgur.com/RnCGEbc.png)
Image 1

<br>

**Introduction:**

In Monterey, app launchers are tiles that execute a command when clicked. A couple of examples are:  
- File explorer
- Atom editor  
- cmd

These app launchers are configurable through the app launcher screen as shown above, allowing you to add your own app launchers to Monterey. When configured, it is possible to call all your favorite development tools by simply clicking a few tiles.

We have predefined a few app launchers for you to use, but you can remove all of these and create your own. 

<br>

** Global vs project specific **  
App launchers can be global or project specific. Global app launchers will show up for every project, while project specific app launchers will only be visible for a single project. In image 1 (numbers 1 and 2) you can switch between the "global" and "project specific" mode.

<br>

**Create custom app launchers**  
Each app launcher has a title, icon and command. The icon can be a URL pointing to an icon. The cmd is the command that Monterey will execute when the app launcher gets clicked. In the "cmd" you can use the following variables:

- %path% - this is the root path of your project
- %url% - if you have started the project via Monterey, then this is the URL your project is running under. If Monterey did not detect the running project, %url% is "http://localhost:9000"

<br>

**Browse launchers**  
Monterey has a registery of app launchers that is maintained outside of the application. The browser can be opened via the "Get more" button:

![img](http://i.imgur.com/KduRCpn.png)
Image 2

From here you can search by name, and click the "install" button for the app launchers that you would like to install. After clicking the "install button" you will notice that the launcher was added to the "Launchers" list. From here you can modify some of the default parameters of the app launcher to fit your needs.

<br>

**Share launchers**  
We welcome anyone to create app launchers and share them with the rest of the community. By clicking the "Share this app launcher" button, the following screen will inform you of the steps to take:
![img](http://i.imgur.com/vAEaqoV.png)
After review the app launcher will show up in the browser (image 2).


