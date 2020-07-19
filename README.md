# SLAM-for-Turtlebot3

The SLAM (Simultaneous Localization and Mapping) is a technique to draw a map by estimating current location in an arbitrary space. The SLAM is a well-known feature of TurtleBot from its predecessors.


-Run SLAM Nodes: 

write this code in your terminal:

#For run roscore 
```
$ roscore
```
#For bring up basic packages to start TurtleBot3 applications.
```
$ roslaunch turtlebot3_bringup turtlebot3_robot.launch
```
then open a new terminal and launch the SLAM file.
```
$ export TURTLEBOT3_MODEL=${TB3_MODEL}
```
```
$ roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
```
Save Map:  
```
$ rosrun map_server map_saver -f ~/map
```
