# Multiple RaspberryPiMouse robots simulator
Gazebo simulator fot multiple RT RaspberryPiMouse robots

## Requirements

- Computer
  - ROS
    - [Kinetic Kame](http://wiki.ros.org/kinetic/Installation/Ubuntu)
    - [Melodic Morenia](http://wiki.ros.org/melodic/Installation/Ubuntu)
    - [Noetic Ninjemys](http://wiki.ros.org/noetic/Installation/Ubuntu)
  - Gazebo
    - Gazebo 9.x

## Installation

Download this package & install all system dependecies
```sh
cd ~/<your_workspace>/src
git clone https://github.com/keeratifts/Multiple-RaspberryPiMouse-robots-simulator.git
cd ~/<your_workspace>/src/Multiple-RaspberryPiMouse-robots-simulator
rosdep install -r -y -i --from-paths raspimouse*
```
Build up this package
```sh
cd ~/<your_workspace>
catkin_make
source devel/setup.bash
```
Download the Gazebo model
```sh
rosrun raspimouse_gazebo download_gazebo_models.sh
```

## Getting started
Enter the following command for single robot simulator.
<img src= https://user-images.githubusercontent.com/76491592/163380533-5103b6ea-b992-492e-9933-5321be3ad36c.png>
```sh
roslaunch raspimouse_gazebo main_singlerobot.launch 
```
Enter the following command for 2 robots simulator.
<img src= https://user-images.githubusercontent.com/76491592/163373737-49ad4113-e28f-4b1a-8045-f6bcfc0de880.png>
```sh
roslaunch raspimouse_gazebo main_2robots.launch
```
Enter the following command for 20 robots simulator.
<img src= https://user-images.githubusercontent.com/76491592/163380538-98233b19-4b15-424c-88c8-25b922b0ae73.png>
```sh
roslaunch raspimouse_gazebo main_20robots.launch
```
Enter the following command for 8 multicolor-robots simulator in the crossroad scenario.
<img src= https://user-images.githubusercontent.com/76491592/163380323-3e26d3a3-fa07-47b1-ad64-1b29eac75bc6.png>
```sh
roslaunch raspimouse_gazebo main_multicolor.launch 
```



