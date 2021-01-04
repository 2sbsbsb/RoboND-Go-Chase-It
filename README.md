## RoboND-Go-Chase-It


This project is to build a ball chaser mobile robot with ROS. The project is divided into two major tasks.

* my_robot  - Design the robot and put into the world build here (https://github.com/2sbsbsb/RoboND-BuildMyWorld)
* ball_chaser - Chase the white colored ball using the robot


#### my_robot 

The my_robot ROS package has a robot, white ball and the world built here (https://github.com/2sbsbsb/RoboND-BuildMyWorld). 
It is designed and configured with the Unified Robot Description format. The robot perceives the surrounding by two sensors a camera and a lidar. 

 - [Lidar hokuyo](http://gazebosim.org/tutorials?tut=ros_gzplugins#GPULaser)
 - [camera](http://gazebosim.org/tutorials?tut=ros_gzplugins#Camera)
 
 
 A white color is added to the Gazebo world which can be moved around and the robot will follow when it is its view. 
 
 To launch the my_robot 
 # roslaunch my_robot world.launch 
 
 
 
 #### ball_chaser 
 
 # roslaunch ball_chaser ball_chaser.launch 
 

#### Directory Structure
```
~/RoboND-Go-Chase-It/catkin_ws/src$ tree
.
├── ball_chaser
│   ├── CMakeLists.txt
│   ├── include
│   │   └── ball_chaser
│   ├── launch
│   │   └── ball_chaser.launch
│   ├── package.xml
│   ├── src
│   │   ├── drive_bot.cpp
│   │   └── process_image.cpp
│   └── srv
│       └── DriveToTarget.srv
├── CMakeLists.txt -> /opt/ros/kinetic/share/catkin/cmake/toplevel.cmake
└── my_robot
    ├── CMakeLists.txt
    ├── launch
    │   ├── robot_description.launch
    │   └── world.launch
    ├── meshes
    │   └── hokuyo.dae
    ├── package.xml
    ├── roscore
    ├── urdf
    │   ├── my_robot.gazebo
    │   └── my_robot.xacro
    └── worlds
        ├── office.world
        └── santosh_bhushan.world

11 directories, 17 files
```


#### RQT Graph

![rqt_graph](https://github.com/2sbsbsb/RoboND-Go-Chase-It/blob/main/rqt_graph.png?raw=true)


#### Demonstation 
[<img src="https://i9.ytimg.com/vi/Ry_-DpFcquo/mq2.jpg?sqp=CJTlzf8F&rs=AOn4CLCsKvv-QaU3_yegSqabMT5oPeY_Qg" width="50%">](https://youtu.be/Ry_-DpFcquo>)



