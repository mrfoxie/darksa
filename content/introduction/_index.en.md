+++
title = "What is ROS?"
date = 2021-05-25T15:50:32Z
weight = 5
chapter = true
pre = "<b>A. </b>"
+++

### What is ROS? A

![ROS.org](http://wiki.ros.org/custom/images/ros_org.png)

# ROS System

ROS is an open-source, meta-operating system for your robot. It provides the services you would expect from an operating system, including hardware abstraction, low-level device control, implementation of commonly-used functionality, message-passing between processes, and package management. It also provides tools and libraries for obtaining, building, writing, and running code across multiple computers. ROS is similar in some respects to 'robot frameworks,' such as [Player](http://playerstage.sf.net/), [YARP](http://eris.liralab.it/yarp/), [Orocos](http://www.orocos.org/), [CARMEN](http://carmen.sourceforge.net/), [Orca](http://orca-robotics.sourceforge.net/), [MOOS](http://www.robots.ox.ac.uk/~pnewman/TheMOOS/index.html), and [Microsoft Robotics Studio](http://msdn.microsoft.com/en-us/robotics/default.aspx).

The ROS runtime "graph" is a peer-to-peer network of processes (potentially distributed across machines) that are loosely coupled using the ROS communication infrastructure. ROS implements several different styles of communication, including synchronous RPC-style communication over [services](https://wiki.ros.org/Services), asynchronous streaming of data over [topics](https://wiki.ros.org/Topics), and storage of data on a [Parameter Server](https://wiki.ros.org/Parameter Server). These are explained in greater detail in our [Conceptual Overview](https://wiki.ros.org/ROS/Concepts).

ROS is not a realtime framework, though it is possible to integrate ROS with realtime code. The Willow Garage PR2 robot uses a system called [pr2_etherCAT](https://wiki.ros.org/pr2_etherCAT), which transports ROS messages in and out of a realtime process. ROS also has [seamless integration with the Orocos Real-time Toolkit](http://www.willowgarage.com/blog/2009/06/10/orocos-rtt-and-ros-integrated).

