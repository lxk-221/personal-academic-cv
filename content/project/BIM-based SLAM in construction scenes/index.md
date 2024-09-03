---
title: Transport Robot
summary: Building Information Modeling‑based Simultaneous Localization and Mapping for mobile robot in construction scenes.
date: 2022-06-01
type: docs
math: true
tags:
  - BIM
  - SLAM
  - Construction scene
---

## Introduction
This is the topic of my Bachelor’s thesis.

## Simulation
We firstly build a simulation environment in V-REP to test our algorithm, we use a remote python API for V-REP to get simulation data from virtual camera and control the robot's motors according to our algorithm.

## Video of test
{{< math >}}
$$
\begin{figure}[!htb]
  \centering
  
  \subfloat[目标点1]{\label{Nav1-1}
  \includegraphics[height=1.2in]{figures/Nav1-1.png}}
  \quad
  \subfloat[目标点1]{\label{Nav1-2}
  \includegraphics[height=1.2in]{figures/Nav1-2.png}}
  \quad
  \subfloat[目标点1]{\label{Nav1-3}
  \includegraphics[height=1.2in]{figures/Nav1-3.png}}
  
  \subfloat[目标点2]{\label{Nav2-1}
  \includegraphics[height=1.2in]{figures/Nav2-1.png}}
  \quad
  \subfloat[目标点2]{\label{Nav2-2}
  \includegraphics[height=1.2in]{figures/Nav2-2.png}}
  \quad
  \subfloat[目标点2]{\label{Nav2-3}
  \includegraphics[height=1.2in]{figures/Nav2-3.png}}
  
  \subfloat[目标点3]{\label{Nav3-1}
  \includegraphics[height=1.2in]{figures/Nav3-1.png}}
  \quad
  \subfloat[目标点3]{\label{Nav3-2}
  \includegraphics[height=1.2in]{figures/Nav3-2.png}}
  \quad
  \subfloat[目标点3]{\label{Nav3-3}
  \includegraphics[height=1.2in]{figures/Nav3-3.png}}
  
  \subfloat[目标点4]{\label{Nav4-1}
  \includegraphics[height=1.2in]{figures/Nav4-1.png}}
  \quad
  \subfloat[目标点4]{\label{Nav4-2}
  \includegraphics[height=1.2in]{figures/Nav4-2.png}}
  \quad
  \subfloat[目标点4]{\label{Nav4-3}
  \includegraphics[height=1.2in]{figures/Nav4-3.png}}
  
  \subfloat[目标点5]{\label{Nav5-1}
  \includegraphics[height=1.2in]{figures/Nav5-1.png}}
  \quad
  \subfloat[目标点5]{\label{Nav5-2}
  \includegraphics[height=1.2in]{figures/Nav5-2.png}}
  \quad
  \subfloat[目标点5]{\label{Nav5-3}
  \includegraphics[height=1.2in]{figures/Nav5-3.png}}
  
  \caption{基于理想2D地图的机器人室内导航}
  \label{Nav2D}
\end{figure}
$$
{{< math >}}
<!--more-->
