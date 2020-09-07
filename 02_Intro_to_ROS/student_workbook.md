- Name:  Will Cody
- Date:  9/14


# Introduction to ROS -- Self Study

---

- Use this document to help you study.
- For each item, make a list of questions that you have.  Identify all of the things that don't make sense to you.  Clearly denote these as questions.
- Also, make notes when you have answered a question.  Clearly denote these as things that you now understand.
- In the end, you should have no unanswered questions.

- This document is written in *markdown*.  It's a great language for documentation.  Here's a cheatsheet for you:  https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

- You will be asked to turn in paper copies of your compiled document.  Please make sure it's neatly formatted.  I suggest using the 
`remarkable` software package that is already installed on your virtual machine.

---

## Textbook Chapters

### Chapter 1 -- Introduction

Just read this chapter...**DO NOT INSTALL ANYTHING**. Your virtual machine already has the software loaded and configured for you.  


- Questions
	-Do coders make money off ROSS
	-What is Unix
	-How do you have multiple languages at once
	-Why Linux
	-What is POSIX
	
- Answered Questions and/or General notes
	-Messages are flattened
	-Developers have firewalls to commercialize
	-POSIX is for portability
	-Linux is easy to install and work with
	-ROS is a framework


---

### Chapter 2 -- Preliminaries

Just read this chapter...**DO NOT INSTALL ANYTHING**. Your virtual machine already has the software loaded and configured for you.  

- Unanswered Questions:
	-Can ROS be done offline
	-What language is roscore
	-What is a CMake macro or custom Python script
	-Why only one Workspace
	-What is XML
	-how does tf work
	
- Answered Questions and/or General notes
	-ROS was created as it was noticed many subsystems could run on many robots
	-ROS displays the programs as a "graph" with many connected nodes
	-Nodes are modules that are sending/receiving messages
	-Modules can be swapped with no major effect
	-Nodes find each other in roscore
	-Anyone can make or get packages which are sections of code for a purpose
	-rosrun runs packages
	-Each node is anonymous to another
	-Namespaces allow better labelling
	-remapping allows named variables to be better labelled and made more specific
	-roslaunch automated launching of collections of ROS nodes
	-TAB auto-completes what is being typed
	-pose tells the x,y,z and orientation
	-tf 


---

### Chapter 3 -- Topics

- Unanswered Questions:
	-How do you document chmod
	-How does documenting topics work
	-What is a tuple
	-Don't understand defining new messages
	-What is TCP port
	
- Answered Questions and/or General notes
	-Topic is stream of messages with a defined type
	-publish sends subscribe receives
	-Messages on same topic must be same data type
	-Ctrl-C stops rostopic and other programs
	-Latched topics allow subscribers to get the last message sent
	-std_msgs package defines primitve message types
	-C++ has more native data types than Python
	-Only make new message types when you absolutely have to
	

---

### Chapter 4 -- Services	

- Unanswered Questions:
	-What does WordCount do
	-What are callbacks
	-How do proxy functions work
	-
	
- Answered Questions and/or General notes
	-Services are synchronous remote procedure calls
	-Services are good for things done occasionally and that take bounded amount of time
	-Three --- mark end of inputs and start of outputs
	-All services can be seen with rossrv
	-rosserivce to use a service
	-can only use advertised services

---

### Chapter 5 -- Actions

- Unanswered Questions:
	-How are the mechanizisms of the action explicitley defined? Preset actions?
	-Are most of these example commands created objects or Python or packages?
	-How do servers work?
	
- Answered Questions and/or General notes
	-Services are for simple interactions
	-Actions are to implement interfaces with time-extended goal oriented behaviors
	-Actions are asynchronous
	-Actions have goals, results and feedback
	-Actions use topics
	-Disable autostarting
	-Can abort actions


---

## ROS Tutorials

### 1)  [Navigating the ROS Filesystem](http://wiki.ros.org/ROS/Tutorials/NavigatingTheFilesystem)

This tutorial introduces ROS filesystem concepts, and covers using the roscd, rosls, and rospack commandline tools.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 2)  [Creating a ROS Package](http://wiki.ros.org/ROS/Tutorials/CreatingPackage)

This tutorial covers using catkin to create a new package, and rospack to list package dependencies.

**IN SECTION 4, DO NOT ADD THE WORKSPACE TO YOUR ROS ENVIRONMENT:**

> ~~$ . \~/catkin_ws/devel/setup.bash~~ 

*This has already been done for you in your virtual machine.*


- Unanswered Questions:
	
- Answered Questions and/or General notes


				
### 3) [Building a ROS Package](http://wiki.ros.org/ROS/Tutorials/BuildingPackages)

**IN SECTION 1, DO NOT DO THIS:**
> ~~# source /opt/ros/\<YOUR_ROS_DISTRO\>/setup.bash~~

> ~~$ source /opt/ros/kinetic/setup.bash             # For Kinetic for instance~~

*This has already been done for you in your virtual machine.*


- Unanswered Questions:
	
- Answered Questions and/or General notes


### 4)  [Understanding ROS Nodes](http://wiki.ros.org/ROS/Tutorials/UnderstandingNodes)

This tutorial introduces ROS graph concepts and discusses the use of roscore, rosnode, and rosrun commandline tools.		

**IN SECTION 1, DO NOT DO THIS:**
> ~~$ sudo apt-get install ros-\<distro\>-ros-tutorials~~
	
*This has already been done for you in your virtual machine.*


- Unanswered Questions:
	
- Answered Questions and/or General notes


### 5) [Understanding ROS Topics](http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics)

This tutorial introduces ROS topics as well as using the rostopic and rqt_plot commandline tools.

**IN SECTION 2.1, DO NOT DO THIS:**
> ~~$ sudo apt-get install ros-\<distro\>-rqt~~

> ~~$ sudo apt-get install ros-\<distro\>-rqt-common-plugins~~

*Your virtual machine already has these things installed.*


- Unanswered Questions:
	
- Answered Questions and/or General notes


### 6)  [Understanding ROS Services and Parameters](http://wiki.ros.org/ROS/Tutorials/UnderstandingServicesParams)

This tutorial introduces ROS services, and parameters as well as using the rosservice and rosparam commandline tools.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 7)  [Creating a ROS msg and srv](http://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv)

This tutorial covers how to create and build msg and srv files as well as the rosmsg, rossrv and roscp commandline tools.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 8a)  [Writing a Simple Publisher and Subscriber (Python)](http://wiki.ros.org/ROS/Tutorials/WritingPublisherSubscriber%28python%29)

This tutorial covers how to write a publisher and subscriber node in python.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 8b)  [Examining the Simple Publisher and Subscriber](http://wiki.ros.org/ROS/Tutorials/ExaminingPublisherSubscriber)

This tutorial examines running the simple publisher and subscriber.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 9a)  [Writing a Simple Service and Client (Python)](http://wiki.ros.org/ROS/Tutorials/WritingServiceClient%28python%29)

This tutorial covers how to write a service and client node in python.

- Unanswered Questions:
	
- Answered Questions and/or General notes


### 9b)  [Examining the Simple Service and Client](http://wiki.ros.org/ROS/Tutorials/ExaminingServiceClient)

This tutorial examines running the simple service and client.

- Unanswered Questions:
	
- Answered Questions and/or General notes

---

## Textbook Github Site

Please take a few moments to familiarize yourself with these resources:

- https://github.com/osrf/rosbook
- https://github.com/osrf/rosbook/issues?utf8=✓&q=
- https://www.oreilly.com/catalog/errata.csp?isbn=0636920024736

These will come in handy throughout the semester.


