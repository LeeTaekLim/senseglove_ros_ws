# Costomized Senseglove_ros
Implement visualizing Sense glove pose. You can see left or right sense glove on Rviz. It works on Ubuntu 18. 

## How to run ##
1. Connect your senseglove pair to your computer.  
2. Just git clone this repository to your catkin_ws.
3. Left glove is default. But if you want right glove to be shown, you should edit some files. Change `<arg name="model" default="$(find senseglove_description)/urdf/dk1_left.xacro"/>` to `<arg name="model" default="$(find senseglove_description)/urdf/dk1_right.xacro"/>` in `senseglove_demo.launch`. Uncomment the commented lines and Comment the uncommented lines in `senseglove_hardware_demo.launch`. 
4. `cd senseglove_ros_ws` and `catkin_make`
5. `roslaunch senseglove_launch senseglove_demo.launch` and wait a second.

![Screenshot from 2021-07-14 16-26-56](https://user-images.githubusercontent.com/40909339/125587431-48834f69-7d7f-453c-9420-74b207e08726.png)
