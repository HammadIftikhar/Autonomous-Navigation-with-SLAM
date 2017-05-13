# Autonomous-Navigation-with-SLAM
Autonomous Navigation of a Pioneer_p3dx in Vrep using frontier_exploration, gmapping, move_base. 


Folders contain parameter files, launch files, Rviz files. 

The launch file among many others which works is ex.launch
After cloning the repository in your catkin workspace, open a terminal and run

$ catkin_make
$ source ./devel/setup.bash
$ roslaunch <project_name> ex.launch

NOTE: If RVIZ crashes, close all other terminals, except those that are running roscore and vrep, and then retry after sourcing setup.bash file.
NOTE: As <project_name> you can rename it yourself from CMakeLists.txt and package.xml.


Problems:
 1. After launching the program, it starts registering Laser Scans and Pose but soon fails to acquire that data.
 2. After publishing exploration boundaries and an initial point the robot doesn't move.
 3. CostMap2DT Transform data aquisition fails due to a timeout.
 4. In V-Rep terminal an ERROR message is displayed saying /explore_server requires base_scan to have datatype sensor_msgs/PointCloud but out version has sensor_msgs/LaserScan. Dropping the connection!
 
 Help will be much appreaciated in figuring out how to make the algorithm work.
 Thank you.
 
