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

### **Project Background and Literature Review**
Our project is divided into five modules which are listed as following:

**Drone Hardware Selection and Assembling**
Selecting hardware for your Multi-Rotor will allow you to conclude that how much payload your
drone is going to carry what decisions are going to be made. We are considering for a Linux
based Raspberry Pi along with the flight controlled to control the motors.
There are some necessary parameters to consider like correct Thrust to Weight Ratio (TWR)
and DriveTrain (DT). A wrong TWR means not able to generate sufficient thrust. For achieving
desired TWR, we need to consider DT which is combination of Motor, Battery and Propellers.
Thrust and current draw are the important functions of DT. Selecting Electronic Speed
Controller (ESC) is again a necessary factor because if we under specify the ESC it is going to
fry and damage the whole vehicle. We can use a locking mechanism which can be controlled
through a motor pulling and pushing the cylindrical hook and release the object.
Maneuvering the Drone Autonomously

A python script can make the drone take off and land autonomously. It will arm the vehicle,
supply necessary information to the flight controller and the vehicle can take off by itself. Similar
functions can be written to perform a landing by manipulating the parameters to land the drone.
There are several drone modes like Return to Launch, Loiter, ALT-Hold and LAND.

**Coordinate Navigation Using GPS**
Our vehicle will get the coordinates using mounted GPS module on our multi-rotor. So we need
precise and accurate coordinates in order for the flight controller to perform smooth performance
towards the destination. Our companion computer should know the final destination which should
be a mission for the drone to follow.

**Precision landing using Open CV**
We can use ArUco markers, calibrate the dimension and force our drone to land precisely on the
marker which will achieve our goal of precise coordinate landing.

**Object Detection and Collision Avoidance**
We can attach ultrasonic sensors to create a bitmap and allow the companion computer to
generate the flyable region for the vehicle while avoiding the obstacles during the mission.

**Drone Tracking on Android Application (Add-On)**
The android application can have a feature to track the drone during its flight and we can check
the status of parcel being picked up and dropped on the correct coordinate.
