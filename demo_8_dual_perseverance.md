---
layout: default
#title: "Demo 8: Dual Perseverance"
#description: Two Perseverances
permalink: "/demo_8_dual_perseverance"
---

### Steps:

1. Open a terminal and go to the plummrs workspace, and source it e.g.: 
   ```
   cd ~/ros
   cd plum
   source devel/setup.bash
   ``` 

4. Launch the rovers and craftsman (Rviz only): 
   ```
   roslaunch plummrs_craftsman_support demo_8_dual_perseverance_demo.launch sim:=true
   ```

5. Start the Plummrs nodes:
   ```
    roslaunch plummrs_craftsman_support demo_8_dual_perseverance_plum.launch 
   ```
6. Start the Behavior Tree node:
   ```
   roslaunch plummrs_craftsman_support demos_bt.launch
   ```
7. Now you can start one of the demonstrations, such as ...
   
   
[back](./)
