[![Netlify Status](https://api.netlify.com/api/v1/badges/9b3309e5-bdb4-412d-9daf-a565cba9426e/deploy-status)](https://app.netlify.com/sites/dark-side-association/deploys)
---
![ROS.org](http://wiki.ros.org/custom/images/ros_org.png)

# ROS System

ROS is an open-source, meta-operating system for your robot. It provides the services you would expect from an operating system, including hardware abstraction, low-level device control, implementation of commonly-used functionality, message-passing between processes, and package management. It also provides tools and libraries for obtaining, building, writing, and running code across multiple computers. ROS is similar in some respects to 'robot frameworks,' such as [Player](http://playerstage.sf.net/), [YARP](http://eris.liralab.it/yarp/), [Orocos](http://www.orocos.org/), [CARMEN](http://carmen.sourceforge.net/), [Orca](http://orca-robotics.sourceforge.net/), [MOOS](http://www.robots.ox.ac.uk/~pnewman/TheMOOS/index.html), and [Microsoft Robotics Studio](http://msdn.microsoft.com/en-us/robotics/default.aspx).

The ROS runtime "graph" is a peer-to-peer network of processes (potentially distributed across machines) that are loosely coupled using the ROS communication infrastructure. ROS implements several different styles of communication, including synchronous RPC-style communication over [services](https://wiki.ros.org/Services), asynchronous streaming of data over [topics](https://wiki.ros.org/Topics), and storage of data on a [Parameter Server](https://wiki.ros.org/Parameter Server). These are explained in greater detail in our [Conceptual Overview](https://wiki.ros.org/ROS/Concepts).

ROS is not a realtime framework, though it is possible to integrate ROS with realtime code. The Willow Garage PR2 robot uses a system called [pr2_etherCAT](https://wiki.ros.org/pr2_etherCAT), which transports ROS messages in and out of a realtime process. ROS also has [seamless integration with the Orocos Real-time Toolkit](http://www.willowgarage.com/blog/2009/06/10/orocos-rtt-and-ros-integrated).

# Goals

A lot of people ask, "How is ROS different from X?" where X is another robotics software platform. It's a difficult question to answer as the goal of ROS is *not* to be a framework with the most features. Instead, the primary goal of ROS is to support code *reuse* in robotics research and development. ROS is a distributed framework of processes (aka *Nodes*) that enables executables to be individually designed and loosely coupled at runtime. These processes can be grouped into *Packages* and *Stacks*, which can be easily shared and distributed. ROS also supports a federated system of code *Repositories* that enable collaboration to be distributed as well. This design, from the filesystem level to the community level, enables independent decisions about development and implementation, but all can be brought together with ROS infrastructure tools.

In support of this primary goal of sharing and collaboration, there are several other goals of the ROS framework:

- [x] Thin: ROS is designed to be as thin as possible -- we won't wrap your main() -- so that code written for ROS can be used with other robot software frameworks. A corollary to this is that ROS is easy to integrate with other robot software frameworks: ROS has already been integrated with OpenRAVE, Orocos, and Player.
- [x] ROS-agnostic libraries: the preferred development model is to write ROS-agnostic libraries with clean functional interfaces.
- [x] Language independence: the ROS framework is easy to implement in any modern programming language. We have already implemented it in [Python](https://wiki.ros.org/rospy), [C++](https://wiki.ros.org/roscpp), and [Lisp](https://wiki.ros.org/roslisp), and we have experimental libraries in Java and Lua.
- [x] Easy testing: ROS has a builtin unit/integration test framework called [rostest](https://wiki.ros.org/rostest) that makes it easy to bring up and tear down test fixtures.
- [x] Scaling: ROS is appropriate for large runtime systems and for large development processes.

# Operating Systems

ROS currently only runs on Unix-based platforms. Software for ROS is primarily tested on Ubuntu and Mac OS X systems, though the ROS community has been contributing support for Fedora, Gentoo, Arch Linux and other Linux platforms.

While a port to Microsoft Windows for ROS is possible, it has not yet been fully explored.

# Releases

The core ROS system, along with useful tools and libraries are regularly released as a [ROS Distribution](https://wiki.ros.org/Distributions). This distribution is similar to a Linux distribution and provides a set of compatible software for others to use and build upon.

