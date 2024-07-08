---
layout: default
#title: "Demo 7: UR5 and Bumble"
#description: Bumble and UR5  running in Gazebo
permalink: "/demo_7_iss_ur5_bumble"
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
    roslaunch plummrs_craftsman_support demo_7_ur5_bumble_robot.launch sim:=false
   ```

3. Astrobees usually start docked. Since we are starting Bumble in a non-default pose, we need to do this
   call to have them ready to move:
   ```
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=bumble
   ```
   
4. Launch craftsman: 
   ```
   roslaunch plummrs_craftsman_support demo_7_ur5_bumble_demo.launch sim:=false robot:=false
   ```

5. Start the Plummrs nodes:
   ```
    roslaunch plummrs_craftsman_support demo_7_ur5_bumble_plum.launch 
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations, such as ...
   
   
[back](./)
