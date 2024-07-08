---
layout: default
#title: "Demo: Inspection with Bumble and Queen"
#description: Bumble and Queen running in Gazebo and performing a visual inspection of a set of waypoints
permalink: "/demo_5_iss_bumble_queen"
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
   roslaunch plummrs_craftsman_support demo_5_bumble_queen_robot.launch sim:=false 
   ```
3. Launch craftsman: 
   ```
   roslaunch plummrs_craftsman_support demo_5_bumble_queen_demo.launch robot:=false sim:=false
   ```
4. Robots usually start docked. Since we are starting them in a non-default pose, we need to do these
   calls to have them ready to move:
   ```
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=bumble
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=queen
   ```
5. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_5_bumble_queen_plum.launch
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations, such as FILL ONE DEMO HERE
  
   
[back](./)
