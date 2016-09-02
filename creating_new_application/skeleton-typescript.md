_Creating new application_
# skeleton-typescript
Note the red "number-markers" which indicate the sequence of mouse clicks.

Start by selecting the template `skeleton-typescript`(Image 1, marker 1).Then continue with the definition of the location where the application will be persisted (marker 2).  This action will invoke the Files Explorer, where you have to define the folder (marker 3) and click on the `Select folder` button (marker 4) to define the location where the application will be stored.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18034958/373abede-6d19-11e6-941e-e8f7d9986276.png"></img>
 <br><br>
Image 1
</p>

<br>

Having defined the path to the folder where the application is stored, click one the `Next` button (marker 1, Image 2).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18034981/6dbb471c-6d19-11e6-9332-1d9f4bd5db5e.png"></img>
 <br><br>
Image 2
</p>

<br>

The next required data is the definition of the application's name (Image 3). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the name of the folder where the application "lives", this name needs to be unique. Observe that Monterey proposes and verifies the application name for uniqueness. Lastly, click on the `Next` button (marker 1) to advance to the next step (Image 4)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035058/6f8d0bf0-6d1b-11e6-974e-72cd7f2eba20.png"></img>
 <br><br>
Image 3
</p>

<br>

Image 4 shows the completed project's configuration, offering the choice between `Previous` button and the `Next` button - we will take that second choice (marker 1).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035066/a08b0004-6d1b-11e6-8b1f-913809f990d5.png"></img>
 <br><br>
Image 4
</p>

<br>

Now (Image 5), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

The concrete example here is rather simple: run the equivalence of **`npm install`**, **`jspm install`**, **`load the app`** and **`gulp watch`** tasks, by invoking respective API (action different from invoking the same service using the console). This execution is triggered by the click on the Start button (marker 1).

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035073/ca1c247a-6d1b-11e6-8ec1-92858e7fdc1c.png"></img>
 <br><br>
Image 5
</p>

<br>

Click on the `Start` button on Image 5, marker 1 above causes the switch of the Monterey's view - from the "workflow" to the Monterey **Task manager** view (Image 6). This is the most often used Monterey integrated tool, which is the controlling and management entity for handling all running Monterey applications. At this time we have a single application (`skeleton-typescript`) running, and you can see that the currently running task is `NPM install`, which will be followed by two more tasks. You can also see the embedded console showing the line-by-line progress of the currently running .`NPM install` task.

Note that Monterey is designed to be able to run many tasks in parallel - this view is restricted to show only the information for the selected project (`skeleton-esnext`).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035079/ead01f50-6d1b-11e6-9f44-5fda8061e16c.png"></img>
 <br><br>
Image 6
</p>

<br>

Image 7 shows the Task manager showing the details of the `gulp watch` task - which ended with the message: "Description: Project running at `http://localhost:9000`"

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035090/199efd24-6d1c-11e6-8d74-245f0965fc13.png"></img>
 <br><br>
Image 7
</p>

<br>

Click on the `Close` button on Image 7 above, will result with closing the Task manager view, making the Main view visible. Click on the Chrome tile (Image 8, marker 1) to see the running app in that browser instance (Image 9, below)

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035096/36815450-6d1c-11e6-9293-e45bd7acb50a.png"></img>
 <br><br>
Image 8
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18035100/5453850c-6d1c-11e6-847b-1bd188838117.png"></img>
 <br><br>
Image 9
</p>

***
***















