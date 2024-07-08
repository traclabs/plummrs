---
layout: default
#title: "Demo: R2 and Bumble"
#description: Bumble and R2  running in Gazebo
permalink: "/demo_2_iss_bumble_r2"
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
    roslaunch plummrs_craftsman_support demo_2_bumble_r2_robot.launch sim:=false
   ```

3. Astrobees usually start docked. Since we are starting Bumble in a non-default pose, we need to do this
   call to have them ready to move:
   ```
   roslaunch plummrs_craftsman_support start_mobility_config_astrobee.launch robot_name:=bumble
   ```   
   
4. Launch craftsman: 
   ```
     roslaunch plummrs_craftsman_support demo_2_bumble_r2_demo.launch robot:=false sim:=false
   ```

5. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_2_bumble_r2_plum.launch
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations, such as demo_3a_inspection.xml
   
   
[back](./)
