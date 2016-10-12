_Creating new application_ | _GitHub_
# CM tutorial - KendoUI edition

This application is the full implementation of Aurelia's [Contact Manager Tutorial](http://aurelia.io/hub.html#/doc/article/aurelia/framework/latest/contact-manager-tutorial) used as the teaching tool for a new [web or SPA developer](http://aurelia.io/hub.html#/doc/persona/new-developer), further augmented by rendering its User interface using [Aurelia KendoUI bridge](https://github.com/aurelia-ui-toolkits/aurelia-kendoui-bridge) based Aurelia Visual Components.

The process starts with the definition of the location where the application will be persisted (Image 1). Note the red "number-markers" which indicate the sequence of mouse click needed to invoke the Files Explorer, select the folder and move to the wizard's next step.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18107997/5409d23c-6ed8-11e6-97dd-cc82c1bb2b1c.png"></img>
 <br><br>
Image 1
</p>

<br>

This template is persisted in GitHub (note that this approach can result with a huge number of templates, with very easy access as the next screen-shot (Image 2) shows: you simply copy the repository URL into clipboard and then paste it in the `GitHub URL` field as shown on Image 3.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18107800/71e539be-6ed7-11e6-8bb5-1b095d259682.png"></img>

Image 2
</p>

<br>

Observe that Monterey "understands" the structure of the repository with the template we want to use and offers you to select a folder where the template "lives" (`kendoui` in this case), as shown on Image 3, marker 2.

<br>

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/19329389/60492c56-90a6-11e6-8c08-1428e076edb3.png"></img>
 <br><br>
Image 3
</p>

<br>

Click on the `Next` button on Image 3, Monterey prompts for the name of the application to be created (Image 4), using the chosen folder name as the placeholder. In this situation, we should accept this name.

<br>

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108133/f2735790-6ed8-11e6-9661-288bd065cdd8.png"></img>
 <br><br>
Image 4
</p>

<br>

Click on the `Next` button (marker 1 on Image 4) results with the project's configuration  view (Image 5)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108259/8465d218-6ed9-11e6-80fa-35b7c680a3eb.png"></img>
 <br><br>
Image 5
</p>

<br>

We are at the very important point in the "conversation" with the Monterey wizard, because the click on the `Next` button (marker 1 on Image 5) will result with Monterey's **workflow form** (Image 6). While at this time, this form is a simple listview enumerating the steps needed to build this app, this will eventually become a real, user programmable workflow - one of Monterey's most attractive features.

Another important point: Monterey is fully capable to detect the "type" of each project - in this case, it recognized that this project is created by Aurelia-CLI and will **automatically create the content of this workflow form**.

In this specific case, please accept all options, ensuring that the build process will start as soon as you click on the `Next` button (marker 1 on Image 6)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108367/e7ba5474-6ed9-11e6-9aec-45b59b8f8723.png"></img>
 <br><br>
Image 6
</p>

<br>

The build process started and invoked Monterey **Task Manager** which will show the progress of this build (note that the subsequent tasks `fetch tasks` and `au run --watch` are scheduled for the execution next (Image 7, down-facing arrow).

Note also the enabled check-box regulating the behavior of the embedded console, which provides the detailed information of the build process.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108395/0443b7ac-6eda-11e6-812f-8ca14078b095.png"></img>
 <br><br>
Image 7
</p>

<br>

This next screenshot (Image 8) was taken nearly 8 minutes after the build process finished and the `au run --watch` task was created. At this point, the reasonable next step would be to **close** Task manager view (Image 8, marker 1), resulting with the "main view" (Image 9)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108425/24d76ef0-6eda-11e6-9ba1-dbacfa54db7a.png"></img>
 <br><br>
Image 8
</p>

<br>

Monterey is also able to find out the running application's URL - meaning that you just have to click on the `Chrome tile` (Image 9, marker 1) in order to see the application running (Image 10)

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108449/40b6d8f4-6eda-11e6-97a8-1b4165947417.png"></img>
 <br><br>
Image 9
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18227564/7fa4e92e-71f6-11e6-8e07-cf214af15007.png"></img>
 <br><br>
Image 10
</p>

<br>

Finally, open the Task Manager view again (Image 11) and use the context menu based `End task` command to terminate the `au run --watch` process.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108673/4e1177ec-6edb-11e6-981c-2bbf570a51c5.png"></img>
 <br><br>
Image 11
</p>

***
***






























