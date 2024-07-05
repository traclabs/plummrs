---
layout: default
#title: "Granite Lab Demo: Criss-crossing paths with Wannabee and Bsharp"
#description: Wannabee and Bsharp running to different corners in the Granite Lab
permalink: "/demo_1_iss_bumble"
---

Note: Corresponding Page in Confluence is [here](https://traclabs.atlassian.net/wiki/spaces/PLUM/pages/3037003777/2.+Run+Bumble+in+Gazebo)

### Steps:

1. Open a terminal and go to the plummrs workspace, and source it e.g.: 
   ```
   cd ~/ros
   cd plum
   source devel/setup.bash
   ``` 
2. Launch the robots:
   ```
    roslaunch plummrs_craftsman_support demo_1_bumble_robot.launch sim:=false dds:=false
   ```
3. Launch craftsman: 
   ```
   roslaunch plummrs_craftsman_support demo_1_bumble_demo.launch sim:=false robot:=false dds:=false
   ```

4. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_1_bumble_plum.launch 
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations, such as demo_1a_inspection.xml
   
   
[back](./)
