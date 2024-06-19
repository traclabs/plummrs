---
layout: default
#title: "Demo: Inspection with Honey and Bumble"
#description: Bumble and Honey running in Gazebo and performing a visual inspection of a set of waypoints
permalink: "/demo_inspection_bumble_honey"
---

### Steps:

1. Open a terminal and go to the plummrs workspace, and source it e.g.: 
   ```
   cd ~/ros
   cd plum
   source devel/setup.bash
   ``` 
2. Launch the robots:
   ```
   roslaunch plummrs_craftsman_support demo_3_bumble_honey_robot.launch sim:=false 
   ```
3. Launch craftsman: 
   ```
   roslaunch plummrs_craftsman_support demo_3_bumble_honey_demo.launch robot:=false sim:=false
   ```
4. Robots usually start docked. Since we are starting them in a non-default pose, we need to do these
   calls to have them ready to move:
   ```
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=bumble
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=honey
   ```
5. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_3_bumble_honey_plum.launch
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations
   
   
[back](./)
