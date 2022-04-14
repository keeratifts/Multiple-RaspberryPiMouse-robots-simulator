# Multiple-RaspberryPiMouse-robots-simulator

<img src= https://user-images.githubusercontent.com/76491592/163373737-49ad4113-e28f-4b1a-8045-f6bcfc0de880.png>

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