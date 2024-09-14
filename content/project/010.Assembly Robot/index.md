---
title: Assembly Robot
summary: Online Phase-Recognizing Movement Primitives for Robotic Assembly Tasks
date: 2024-10-01
type: docs
math: true
tags:
  - Robotic Assembly
  - PMP
---

## Abstrct
Movement Primitives (MP) are promising methods for modeling robot motion from human demonstrations. Using learned parameters and a phase variable typically scaled to $\boldsymbol{[0,1]}$, MP can generate a trajectory as the phase transitions from 0 to 1.
However, in assembly tasks that require high precision and online adjustments, typical MP methods do not work well, particularly when the trajectory is executed with limited controller gains, or when the task is hindered by some obstacles.
Therefore, we propose Phase-Recognizing Movement Primitive (PMP), which can make a stable estimation of the task phase online, make suitable adjustments when the assembly task is hindered by external disturbances, and finally achieve precise assembly while using a low gain compliance controller.
Specifically, given the robot state, we assume the phase is a random variable with a Gaussian distribution. Consequently, the phase velocity can be computed, enabling us to determine whether the task is hindered and to retry if the task is stuck.
We test our method on a Peg-In-Hole assembly task in simulation and a Slide-In-The-Groove assembly task on real UR5. The experimental results show that PMP can make stable estimations of the phase and thus make adjustments to complete the hindered assembly tasks.

<!--more-->
