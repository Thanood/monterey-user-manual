_Features_

<h3 style="float: left">Taskmanager</h3>
<p style="float: left">
  <img src="https://cloud.githubusercontent.com/assets/2189477/18088393/a4aefae6-6eba-11e6-90c5-0d3b37df7351.png" width="50"></img>
</p>
<p style="clear: both"></p>

**Tile:**  
![img](http://i.imgur.com/4liq8Y1.png)

**Screen:**

![img](http://i.imgur.com/gw3tu81.png)

**Description:**  
Monterey is able to execute actions for you, but many of these actions take a lot of time to complete. The task manager allows you to monitor the progress of these tasks, and keeps you from having to wait for tasks to complete. 

From the taskmanager it is also possible to launch new tasks, such as `gulp watch` or `au run --watch`.

**Monitoring of running tasks**  
The [skeleton-esnext-aspnetcore](https://github.com/aurelia/skeleton-navigation/tree/master/skeleton-esnext-aspnetcore) skeleton require many different commands to be executed in order to get it running. Monterey can start all these commands for you, and execute them in the right order. In the following screenshot you can see that the "NPM install" task is running. By clicking on the task, you can see details of the execution. 

All other tasks are queued. After "NPM install" task completes, the "JSPM install" task is started automatically.

![img](http://i.imgur.com/PdLh65l.png)
A few minutes later:
![img](http://i.imgur.com/x0eezIs.png)

<br>

**Starting new tasks**  
From the taskmanager it is possible to start new tasks. 

![img](http://i.imgur.com/TnH5ebb.png)

Based on whether or not you use Gulp, DotNet or Webpack in the selected project, there will be accompanied tabs. In the favorite tab you can start tasks that are used the most. A complete list of tasks can be requested via the tabs.

![img](http://i.imgur.com/8jc4H44.png)

Here you can double click on a task to start it, or favorite tasks by clicking on a task and using the  "Favorite this task" button.

