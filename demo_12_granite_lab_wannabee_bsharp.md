---
layout: default
#title: "Granite Lab Demo: Criss-crossing paths with Wannabee and Bsharp"
#description: Wannabee and Bsharp running to different corners in the Granite Lab
permalink: "/demo_12_granite_lab_wannabee_bsharp"
---

Note: Corresponding Page in Confluence is [here](https://traclabs.atlassian.net/wiki/spaces/PLUM/pages/3165782043/8.+Gazebo+Run+Bsharp+and+Wannabee+in+Granite+Lab)

### Steps:

1. Open a terminal and go to the plummrs workspace, and source it e.g.: 
   ```
   cd ~/ros
   cd plum
   source devel/setup.bash
   ``` 
2. Launch the robots:
   ```
    roslaunch plummrs_craftsman_support demo_12_wannabee_bsharp_robot.launch sim:=false dds:=false
   ```
3. Launch craftsman: 
   ```
   roslaunch plummrs_craftsman_support demo_12_wannabee_bsharp_demo.launch sim:=false robot:=false dds:=false
   ```

4. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_12_wannabee_bsharp_plum.launch 
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations
   
   
[back](./)
