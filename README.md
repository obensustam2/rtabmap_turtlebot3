SLAM and navigation is achieved by using rtab-map, amcl and move_base packages in a simulated environment using Turtlebot3 waffle.

To install packages
```bash
sudo apt-get install ros-melodic-turtlebot3*
sudo apt-get install ros-melodic-rtabmap-ros*
```

To start mapping
```bash
roslaunch rtabmap_turtlebot3 turtlebot3_house.launch
roslaunch rtabmap_turtlebot3 demo_turtlebot3_navigation.launch 
roslaunch rtabmap_turtlebot3 turtlebot3_teleop_key.launch model:=waffle
```

To start localization and navigation
```bash
roslaunch rtabmap_turtlebot3 turtlebot3_house.launch 
roslaunch rtabmap_turtlebot3 demo_turtlebot3_navigation.launch localization:=true 
```

To visualize created map
```bash
rtabmap-databaseViewer <database_directory>
```

