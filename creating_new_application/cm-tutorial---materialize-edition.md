_Creating new application_ | _GitHub_
# CM tutorial - Materialize edition

This application is the full implementation of Aurelia's [Contact Manager Tutorial](http://aurelia.io/hub.html#/doc/article/aurelia/framework/latest/contact-manager-tutorial) used as the teaching tool for a new [web or SPA developer](http://aurelia.io/hub.html#/doc/persona/new-developer), further augmented by rendering its User interface using [Aurelia Materialize bridge](https://github.com/aurelia-ui-toolkits/aurelia-materialize-bridge) based Aurelia Visual Components.

The process starts with the definition of the location where the application will be persisted (Image 1). Note the red "number-markers" which indicate the sequence of mouse click needed to invoke the Files Explorer, select the folder and move to the wizard's next step.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18107997/5409d23c-6ed8-11e6-97dd-cc82c1bb2b1c.png"></img>
 <br><br>
Image 1
</p>

<br>

This template is persisted in GitHub (note that this approach can result with a huge number of templates) with very easy access as the next screen-shot (Image 2) shows: you simply copy the repository URL (https://github.com/aurelia-ui-toolkits/cm-bridges) into clipboard and then paste it in the `GitHub URL` field as shown on Image 3.

<br>
![](cm-tutorial-step-1.png)
Image 2

<br>

Observe that Monterey "understands" the structure of the repository with the template we want to use and offers you to select a folder where the template "lives" (`kendoui` in this case), as shown on Image 3, marker 2.

![image](https://cloud.githubusercontent.com/assets/677826/19489712/9aba7226-956c-11e6-9a1c-97b4a833c15e.png)

Image 3

<br>

Click on the `Next` button on Image 3, marker 3, Monterey prompts for the name of the application to be created (Image 4), using the chosen folder name as the placeholder. In this situation, we should accept this name.

<br>

![image](https://cloud.githubusercontent.com/assets/677826/19489791/f12f53f6-956c-11e6-93bf-a2daecb5400a.png)

Image 4

<br>

Click on the `Next` button results with the project's configuration  view (Image 5)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/19335350/8099313e-90d0-11e6-93b9-9012f1abb238.png"></img>
 <br><br>
Image 5
</p>

<br>

We are at the very important point in the "conversation" with the Monterey wizard, because the click on the `Next` button (marker 1 on Image 5) will result with Monterey's **workflow form** (Image 6). While at this time, this form is a simple listview enumerating the steps needed to build this app, this will eventually become a real, user programmable workflow - one of Monterey's most attractive features.

Another important point: Monterey is fully capable to detect the "type" of each project - in this case, it recognized that this project is created by Aurelia-CLI and will **automatically create the content of this workflow form**.

In this specific case, please accept all options, ensuring that the build process will start as soon as you click on the `Next` button (marker 1 on Image 6)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/19335508/e2d8fa0e-90d1-11e6-827f-eda462fb231f.png"></img>
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

At this point, the reasonable next step would be to **close** Task manager view (Image 7) resulting with the "main view" (Image 8)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/19335616/ab250a70-90d2-11e6-844d-3818661e6c2d.png"></img>
 <br><br>
Image 8
</p>

<br>

Monterey is also able to find out the running application's URL - meaning that you just have to click on the `Chrome tile` (Image 8, marker 1) in order to see the application running (Image 9)

![image](https://cloud.githubusercontent.com/assets/677826/19490310/ef33d8f4-956e-11e6-8c1d-45034267a61c.png)


Image 9

<br>

Finally, open the Task Manager view again (Image 11) and use the context menu based `End task` command to terminate the `au run --watch` process.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18108673/4e1177ec-6edb-11e6-981c-2bbf570a51c5.png"></img>
 <br><br>
Image 11
</p>

***
***

