---
layout: default
#title: "Demo: Inspection with Honey and Bumble"
#description: Bumble and Honey running in Gazebo and performing a visual inspection of a set of waypoints
permalink: "/demo_3_iss_bumble_honey"
---

Note: Corresponding Page in Confluence is [here](https://traclabs.atlassian.net/wiki/spaces/PLUM/pages/2926706689/4.+Run+Humble+and+Honey+in+Gazebo)

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
7. Now you can start one of the demonstrations, such as demo_3a_inspection.xml
   
   
[back](./)
