-----------


# Your turn now!

<img src="https://media.giphy.com/media/13GIgrGdslD9oQ/giphy.gif" width=50%/>

  - [1) Add Monitoring to Your Systems](#\1)-Add-Monitoring-to-Your-Systems)
  - [2) Software Maintenance](#2\)-Software-Maintenance)
  - [3) Software Maintenance II](#3\)-Software-Maintenance-II)


## 1) Add Monitoring to Your Systems

Your task until next week is to add monitoring to your _ITU-MiniTwit_ systems. Add for sure some application monitoring and infrastructure monitoring. Add all other categories of monitoring after your liking and after what you deem important for your application.

In case you adapt the monitoring example from class (https://github.com/itu-devops/itu-minitwit-monitoring) make sure to turn your Grafana configuration/dashboard into code so that you do not have to click together your dashboard every time you restart the Grafana container. To do so, you may start reading:

  * https://grafana.com/docs/grafana/latest/installation/configure-docker/
  * https://runkiss.blogspot.com/2020/01/using-prometheus-grafana-to-monitor.html
  
Add a link to your monitoring dashboard via a pull request to the file [`misc_urls.py`](https://github.com/itu-devops/lecture_notes/blob/master/misc_urls.py) in https://github.com/itu-devops/lecture_notes. (Replace the URL `"http(s)://<TBA>/"` below the comment `# Monitoring URL:` with your respective URL.
Link either a read-only dashboard or add a user with name and credentials that Helge provides you via the Teams chat channel, so that we can see what you are monitoring and can provide feedback on it in the start of the next session.


## 2) Software Maintenance 

From now on, we are in software maintenance. That is, fix issues of your version of _ITU-MiniTwit_ **as soon as possible**. Let's say that as soon as possible means within 24 hours if possible, i.e., if it is not a super big issue that requires a big rewrite. 

Likely, after the simulator is started you will experience some issues in your systems. Just fix them as soon as you realize them.

For example, you will be able to see status and potential errors as the simulator 'sees' them [here](http://164.92.246.227/status.html).

Continue to release (now likely automatically) at least once per week versions of your system with corresponding fixes.


## 3) Software Maintenance II

In case you have not done so yet, check the user interface of another group's _ITU-MiniTwit_ application for functionality. That is, connect via a browser to another group's application and check if the system is working similar to the original _ITU-MiniTwit_, i.e.,

  * Do you see a public timeline?
  * Does the public timeline show messages that the application received from the simulator?
  * Can you create a new user?
  * Can you login as a new user?
  * Can you write a message?
  * After publishing a message, does it appear on you private timeline?
  * Can you follow another user?

In case you find non-functional/erroneous behavior please report it via issues to the respective Github repositories (find them in [`repositories.py`](https://github.com/itu-devops/lecture_notes/blob/master/repositories.py)).

**Do not** send requests to the simulator API of the other group. It is really only meant for the simulator (behave nicely towards the other group!). In case you want to make sure that non of the other groups sends requests to the simulator API of your group, you might want to only accept connections from the simulator server, which has the IP `164.92.246.227`.

Please find which group's user interface you are checking in the list below. Find your own group on the left-hand side and the name of the group your are checking behind the arrow. You will find the URL of the _ITU-MiniTwit_ application from the respective group in file [`repositories.py`](https://github.com/itu-devops/lecture_notes/blob/master/repositories.py) (first of the two given URLs).


### Who checks whom?

#### BSc

  * Group a _Group A_ -[checks]-> Group c _DevOpps_
  * Group c _DevOpps_ -[checks]-> Group f _PayRespect_
  * Group f _PayRespect_ -[checks]-> Group g _Call Of Duty _
  * Group g _Call Of Duty BlackOps_ -[checks]-> Group h _Continuous disintegration_
  * Group h _Continuous disintegration_ -[checks]-> Group j _Root_
  * Group j _Root_ -[checks]-> Group l _iBois_
  * Group l _iBois_ -[checks]-> Group o _TBD_
  * Group o _TBD_ -[checks]-> Group r _Rhododevdron_
  * Group r _Rhododevdron_ -[checks]-> Group a _Group A_

#### MSc

  * Group b Group Bee -[checks]-> Group d DevelOps
  * Group d DevelOps -[checks]-> Group e ASPirin
  * Group e ASPirin -[checks]-> Group i A-team
  * Group i A-team -[checks]-> Group k DevUps
  * Group k DevUps -[checks]-> Group m DeadlyDevops
  * Group m DeadlyDevops -[checks]-> Group n DevØps
  * Group n DevØps -[checks]-> Group b Group Bee


<!-- 
## 3) MSc Students

Prepare a ten minute presentation about your systems. Include presentation of:

  * the architecture (including important subsystems)
  * the used technologies and programming languages
  * a view to your systems through the monitoring dashboard
  * anything that you want to highlight about your solution -->
