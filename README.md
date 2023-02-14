
# Arm Control

Simulation and Control for the 7DOF Franka Emika Panda Robotic Arm in Gazebo and ROS Noetic.



## Installation

To install ROS Noetic + Gazebo, follow the instructions and install ```ros-noetic-desktop-full ``` [here](http://wiki.ros.org/noetic/Installation/Ubuntu).

#### Installing Dependencies
---
```bash
sudo apt install ros-noetic-libfranka ros-noetic-franka-ros
sudo apt install build-essential cmake git libpoco-dev libeigen3-dev
```

#### Setting Up Repository
---
```bash
 source /opt/ros/noetic/setup.bash 
 mkdir -p {workspace}/src       # workspace name of your choice
 cd {workspace}/src/
 
 git clone https://github.com/ShahhhVihaan/arm_control.git
 cd ../../                      # go back to {worksapce} directory
 catkin_make
 source {worksapce}/devel/setup.bash
```
#### Sourcing Scripts
---
To automatically source this script every time a new shell is launched 


  
## Usage/Examples

```bash
roslaunch franka_gazebo panda.launch rviz:=true
```