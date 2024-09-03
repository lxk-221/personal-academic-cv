---
title: Transport Robot
summary: This project aims to make a lightweight transport robot for a material carrying competition.
date: 2021-10-01
type: docs
math: false
tags:
  - Transport Robot
  - Visual Serving
---

## Overview
This project aims to make a lightweight transport robot for a material-carrying competition. Robots are asked to catch materials from several specific positions and carry them to some other positions. The more accurately the materials are placed, and the more materials are handled, the shorter the time used, resulting in a higher score. In this project, a mobile robot with a lightweight arm is designed, and two 2D cameras are used, which are mounted on the end effector of the arm and the side of the robot chassis, respectively. We use a visual serving strategy to adjust our arm to guarantee the accuracy of placing.

In this project, I was responsible for the control of the chassis, arm, and camera. I use a RANSAC-based method to detect the target and do a close-loop control for placing action. I also participated in the design of the robot, including the layout, the type of arm selected, and the carrying strategy.

## Description of the Task
Several materials in three colors—red, green, and blue—are arranged in different positions on the shelf. Besides, there are the same number of QR codes on the shelf as the number of materials, each QR code represents the target position of the material. With all this information, the robot should first grasp these materials onto the robot, and carry them to the desired position.

Besides, black grids on the ground allow us to use grayscale sensors for the robot's localization.

For the placement, we use a RANSAC-based method to detect the center of the target position according to the camera mounted on the end effector.

## Final Version of Our Robot
This video shows the whole process of the competition, as we can see, the robot uses a visual serving strategy to adjust the end effector and achieve precise placement.
{{< youtube XEpZW4rSB-8 >}}

<!--more-->
