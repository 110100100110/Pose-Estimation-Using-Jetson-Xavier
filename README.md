# Human Pose-Estimation Using Jetson/Xavier

## Introduction
Human Pose Estimation (HPE) is a way of identifying and classifying the joints in the human body.

Essentially it is a way to capture a set of coordinates for each joint (arm, head, torso, etc.,) which is known as a key point that can describe a pose of a person. The connection between these points is known as a pair. 

## Installation Guide

### Step 1: Setting Up Jetpack On Jetson Device

1. Install Jetpack/OS on Jetson Device [guide](https://developer.nvidia.com/embedded/learn/get-started-jetson-xavier-nx-devkit).
2. After installing Jetpack on Jetson Device, follow the basic system configuration.

### Step 2: Install Virtual Environment

1. On Jetson Device Open Terminal (Ctrl+T) and run the following command
  ```python
    sudo apt-get update && upgrade
    sudo apt-get install python3-dev python3-pip
    pip3 install -U virtualenv
  ```

2. Create Virtual Environment
  ```python  
  python3 -m virtualenv --system-site-packages /home/UserName/python
  ```
  Activate the virtual environment using the following command. </br>
  source /home/UserName/python/bin/activate
 
### Step 3: Install Torch & Torchvision 
