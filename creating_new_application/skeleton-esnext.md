_Creating new application_
# skeleton-esnext
Note the red "number-markers" which indicate the sequence of mouse clicks.

Start by selecting the template `skeleton-esnext-webpack`(Image 1, marker 1).Then continue with the definition of the location where the application will be persisted (marker 2).  This action will invoke the Files Explorer, where you have to define the folder (marker 3) and click on the `Select folder` button to define the location where the application will be stored.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024429/1833667c-6bd8-11e6-9335-e284bc2784fa.png"></img>
 <br><br>
Image 1
</p>

<br>

Having defined the path to the folder where the application is stored, click one the `Next` button (marker 1, Image 2).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024432/41d06f52-6bd8-11e6-9189-0ef37df4b662.png"></img>
 <br><br>
Image 2
</p>

<br>

The next required data is the definition of the application's name (Image 3). This is the name that will appear on the Monterey's list-view of all open applications. Since this same name will be used as the name of the folder where the application "lives", this name needs to be unique. Observe that Monterey proposes and verifies the application name for uniqueness.

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024459/d887300c-6bd8-11e6-8853-d11c06afd513.png"></img>
 <br><br>
Image 3
</p>

<br>

Image 4 shows the completed project's configuration, offering the choice between `Previous` button and the `Next` button - we will take that second choice (marker 1).

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024465/0f4c71ba-6bd9-11e6-8283-3a9663e6ca3e.png"></img>
 <br><br>
Image 4
</p>

<br>

Now (Image 5), we reached the most important step of the Monterey wizard - page where will eventually reside the Monterey **workflow** plugin. At this time you see the workflow's "place-holder" implemented as a list of check-boxes presenting the list of application build options that are meaningful in the given context. As Monterey gets able to handle a lot more complex tasks (managing creation, building, testing and deployment tasks of several tens of applications at the same time, the concept of the "workflow of workflows" will be the best way to ensure correct and meaningful definition of all of these tasks running in a conflict-free fashion.

The concrete example here is rather simple: run the equivalence of **`npm install`**, **`jspm install`**, **`load the app` and **`gulp watch`** tasks, by invoking respective API (action different from invoking the same service using the console). This execution is triggered by the click on the Start button (marker 1).

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024482/65e11f62-6bd9-11e6-8139-bb0b3ab28644.png"></img>
 <br><br>
Image 5
</p>

<br>

Click on the `Start` button on Image 5, marker 1 above causes the switch of the Monterey's view - from the "workflow" to the Monterey **Task manager** view (Image 6). This is the most often used Monterey integrated tool, which is the controlling and management entity for handling all running Monterey applications. At this time we have a single application (`Default-ESNext`) running, and you can see that the currently running task is `NPM install`, which will be followed by two more tasks. You can also see the embedded console showing the line-by-line progress of the currently running .`NPM install` task.

Note that Monterey is designed to be able to run many tasks in parallel - this view is restricted to show only the information for the selected project (`skeleton-esnext`).

Task manager, being aware of this application context and state, proposes two most likely used tasks - `gulp prepare release` and `gulp watch` (marker 1). Click on `gulp watch` button.

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18187345/a6f5fff8-7076-11e6-9d4c-05e50d693ccd.png"></img>
 <br><br>
Image 6
</p>

<br>

Image 7 shows the Task manager showing the details of the `gulp watch` task - which ended with the message: "Description: Project running at `http://localhost:9000`"

<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18187457/af02de7c-7077-11e6-864a-54316e4aeabf.png"></img>
 <br><br>
Image 7
</p>
<br>

<br>


<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024549/3fcc8daa-6bdb-11e6-9a5d-0fb3c5185aed.png"></img>
 <br><br>
Image 6
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024556/8283a188-6bdb-11e6-91d7-dcd0b6d1dfe2.png"></img>
 <br><br>
Image 7
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024564/a9675902-6bdb-11e6-91ef-2ff8c6c20d46.png"></img>
 <br><br>
Image 8
</p>

<br>
<p align=center>
  <img src="https://cloud.githubusercontent.com/assets/2712405/18024569/ce132d12-6bdb-11e6-9129-3554a1e1d998.png"></img>
 <br><br>
Image 9
</p>
<br>












