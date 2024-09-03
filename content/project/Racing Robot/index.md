---
title: Racing Robot
summary: uss a webcam to guide the robot in a specific field
date: 2019-10-01
type: docs
math: false
tags:
  - Racing Robot
---

## Overview
This project aims to participate in a robot racing competition. In the competition, the robot is asked to finish the track and hit the target at the destination without getting into the black area as fast as possible. 
Robots are requested to use a humanoid robot with an omnidirectional chassis comprising three Mecanum wheels and a webcam on its backpack. All programs were running on a Raspberry Pi 4B in the backpack.

In this project, I was responsible for the simulation, vision, and control algorithm. I built a simulation environment in the V-REP simulator, tested an edge detection-based method for track detection, and used vision-based PD control for the chassis. Besides, we use Keras and TensorFlow to solve a classified problem and rotate the robot in the right direction since the robot is placed in a random direction at the starting point.

## Simulation
We first built a simulation environment in V-REP to test our algorithm, we used a remote Python API for V-REP to get simulation data from the virtual camera and control the robot's motors according to our algorithm. The field of view of the real webcam is tested to guarantee that the virtual camera has similar parameters to the real one.

## Real Robot
The original position of the webcam is too high to get enough information on the ground in front of the robot. So we used a 3D printer to create an adjustable-angle camera mount, allowing it to tilt downwards to overlook the ground. To increase the friction of the wheels, we tried a new material for molding the tire and did some tests on the real robot.

## Video of test
This video shows the whole process of the competition. As we can see, the robot starts with different orientations, then it classifies the command into three classes, namely left, right, and forward, according to the picture from the webcam. For the left or right command, the robot turns left or right with a specific angle. For the forward command, the robot starts to control its chassis with an edge detection-based PD control. The visual algorithm can be robust even when faced with camouflage plots. Finally, the robot uses an arc detection-based method to estimate the distance to the target and decelerate while adjusting its orientation.

{{< youtube cpf3xdfruAY >}}
<!--{{< youtube L-4Lpmt8hqk >}}-->
<!--more-->
