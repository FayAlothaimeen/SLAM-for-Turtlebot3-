# SLAM-for-Turtlebot3

-Run SLAM Nodes: 

write this code in your terminal:

#for run roscore 

$ roscore

#for bring up basic packages to start TurtleBot3 applications.

$ roslaunch turtlebot3_bringup turtlebot3_robot.launch

then open a new terminal and launch the SLAM file.

$ export TURTLEBOT3_MODEL=${TB3_MODEL}
$ roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping

Save Map:  

$ rosrun map_server map_saver -f ~/map
