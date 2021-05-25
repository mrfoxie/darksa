+++
title = "Goal"
date = 2021-05-25T15:55:16Z
weight = 10
1chapter = true
pre = "<b>B. </b>"
+++

### Goal B

![ROS.org](http://wiki.ros.org/custom/images/ros_org.png)

## Goals

A lot of people ask, "How is ROS different from X?" where X is another robotics software platform. It's a difficult question to answer as the goal of ROS is *not* to be a framework with the most features. Instead, the primary goal of ROS is to support code *reuse* in robotics research and development. ROS is a distributed framework of processes (aka *Nodes*) that enables executables to be individually designed and loosely coupled at runtime. These processes can be grouped into *Packages* and *Stacks*, which can be easily shared and distributed. ROS also supports a federated system of code *Repositories* that enable collaboration to be distributed as well. This design, from the filesystem level to the community level, enables independent decisions about development and implementation, but all can be brought together with ROS infrastructure tools.

In support of this primary goal of sharing and collaboration, there are several other goals of the ROS framework:

- [x] Thin: ROS is designed to be as thin as possible -- we won't wrap your main() -- so that code written for ROS can be used with other robot software frameworks. A corollary to this is that ROS is easy to integrate with other robot software frameworks: ROS has already been integrated with OpenRAVE, Orocos, and Player.
- [x] ROS-agnostic libraries: the preferred development model is to write ROS-agnostic libraries with clean functional interfaces.
- [x] Language independence: the ROS framework is easy to implement in any modern programming language. We have already implemented it in [Python](https://wiki.ros.org/rospy), [C++](https://wiki.ros.org/roscpp), and [Lisp](https://wiki.ros.org/roslisp), and we have experimental libraries in Java and Lua.
- [x] Easy testing: ROS has a builtin unit/integration test framework called [rostest](https://wiki.ros.org/rostest) that makes it easy to bring up and tear down test fixtures.
- [x] Scaling: ROS is appropriate for large runtime systems and for large development processes.
