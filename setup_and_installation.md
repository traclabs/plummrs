---
layout: default
title: "Setup and Installation"
description: Setup and installation of a Plummrs workspace
permalink: "/setup_installation"
---

## Setup and Installation

### Requirements

1. Machine: Ubuntu 20.04.
2. ROS Noetic installed.
3. Astrobee workspace installed.

### Steps:

1. Clone the plummrs metapackage: 
   ```
   cd ~/ros
   git clone git@bitbucket.org:traclabs/plummrs.git plum
   cd plum
   ``` 
2. Download the packages:
   ```
   vcs import src < src.repos
   vcs import src < robots.repos
   ```
3. Source the astrobee workspace and then build:
   ```
   source ~/ros/astrobee/devel/setup.bash
   catkin build -j4
   ```
   
[back](./)
