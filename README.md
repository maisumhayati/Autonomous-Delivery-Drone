# **Autonomous Parcel Delivery Drone**

### ABSTRACT
Unmanned Aerial Vehicles, UAVs, are becoming more and more available as technology
advances. Adding colors to it by a twist of an autonomous flight feature is something that we can
look forward to in today’s world. This paper represents an Autonomous Delivery Drone which is
an Unmanned Aerial Vehicle (UAV) comprising of an autonomous flight feature.
In the world of truly autonomous vehicles, UAVs should respond on their own through external
stimuli which help UAVs to respond and acquire designated goals accordingly. These stimuli can
be taken from various components and sensors on the craft but also be remotely accessed by the
ground stations. Our Autonomous Delivery Drone will include design decisions, a
communication protocol, waypoint system and user interface while utilizing other software that
helps with the control and flow of the system.

The goal of our Autonomous Delivery Drone is to deliver parcel to our destined location. This
will ensure time delivery, considering the fact that how often we get to interact with traffic jams
in our cities throughout the country. Use of this Drone will bring advances to the transportation
sector by providing efficient transport management as it cut downs the vehicle fuel cost and saves
time of the human labor responsible for the parcel delivery. The idea is to use the technology in
order to help humanity and a system like this can bring hope that not all tasks are futile.

## Some Screenshots from the working simulations and code snippets

![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/Gazebo.PNG)

![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/MAV.PNG)


![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/QGROUNDCONTROL.PNG)


![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/ROS.PNG)


![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/ROS_2.PNG)


![alt text](https://github.com/maisumhayati/Autonomous-Delivery-Drone/blob/main/Images/ROS_3.PNG)

### Methodology and Equipment/Tools
#### 1. METHODOLOGY
The methodology is to have a drone that takes coordinates in terms of longitude and latitude and
moves to a destination way point after reaching target altitude. The coordinates can be reset by
using by SSH via Laptop to the mission script. The drone adjusts its path using GPS and Open
CV. On reaching its destination, precision landing would be performed by using ArUco marker
by which delivery process is performed. Finally the drone takes off again and reallocates to its
launch zone where again precession landing is performed using ArUco marker.

#### 2. EQUIPMENT/TOOLS
**Hardware Tools:**
Drone Frame, Brushless Motors, Propellers, ESC (Electronic Speed Controller), Battery, Flight
Controller, Power Distribution Board, GPS module, Ultrasonic sensors, Raspberry Pi, RPi
Camera, Delivery Module, USB 4G LTE Dongle

**Software Tools:**
Python based scripts, OS-Linux, ROS (Robot Operating System) and ArduPilot, DroneKit,
Gazebo Simulator


