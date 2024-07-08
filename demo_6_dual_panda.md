---
layout: default
#title: "Demo: Dual Panda"
#description: Dual Panda
permalink: "/demo_6_dual_panda"
---


### Steps:

1. Open a terminal and go to the plummrs workspace, and source it e.g.: 
   ```
   cd ~/ros
   cd plum
   source devel/setup.bash
   ``` 
2. Launch the robots and craftsman:
   ```
   roslaunch plummrs_craftsman_support demo_6_dual_panda_demo.launch sim:=true
   ```
3. Start the Plummrs nodes:
   ```
   roslaunch plummrs_craftsman_support demo_6_dual_panda_plum.launch
   ```
4. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
5. Now you can start one of the demonstrations, such as ...
   
   
[back](./)
