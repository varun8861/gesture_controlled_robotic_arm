# **MoveWithIt**

## **Description**
MoveWithIt helps you to control robotic arms just by using your hand gestures. This reduces the complexity of using and setting up different controllers on your system (like keyboard inputs) and is easy to use!

*This package has been created and tested on Ubuntu 22.04 with ROS2 Humble.*

## **Prerequisites**
The only prerequisite is to complete [this](https://moveit.picknik.ai/main/doc/tutorials/getting_started/getting_started.html) tutorial to set up MoveIt on your system.

## **How to build**
*Creating a workspace to build the package*
```
mkdir -p ~/movewithit_ws/src && cd ~/movewithit_ws/src
```
*Cloning the package*
```
git clone https://github.com/AlapatiChandrasekhar/gesture_controlled_robotic_arm.git
cd ~/movewithit_ws
```
*Installing the dependencies and building the workspace*
```
rosdep install --from-paths src -y --ignore-src
colcon build
```
## **How to use**
```
# source the workspaceS
source ~/movewithit_ws/install/setup.bash
source ~/ws_moveit/install/setup.bash       
# 'ws_moveit' is the workspace created during the installation of moveit

# You're all set to go! Run the launch file
ros2 launch move_with_it main.launch.py
```  

