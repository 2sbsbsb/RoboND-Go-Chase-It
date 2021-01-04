## RoboND-Go-Chase-It


This project is to build a ball chaser mobile robot with ROS. The project is divided into two major tasks.

* my_robot  - Design the robot and put into the world build here (https://github.com/2sbsbsb/RoboND-BuildMyWorld)
* ball_chaser - Chase the white colored ball using the robot


### Directory Structure
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





