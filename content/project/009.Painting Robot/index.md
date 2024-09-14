---
title: Painting Robot
summary: Painting Robot for Interior Finishing
date: 2023-09-01
type: docs
math: true
tags:
  - Painting Robot
  - Construction scene
---

## Overview
This project is the topic of my Master’s thesis. 

In construction spraying operations, spray robots offer significant advantages over manual labor. However, to meet the high precision required, spray robots must accurately perceive large-scale objects. Additionally, the demands of the spraying process require that spray robots incorporate new procedural constraints into their path planning for wall coverage painting. This research will focus on the following aspects. 
1. Perception of large wall surfaces.
2. Coverage path planing for the robot.
3. The software for the whole painting robot on Windows.

## Perception

Initially, we used a region-growing based method for perception, projecting the wall surface onto a 2D plane. This approach effectively transitioned the problem from 3D coverage path planning to 2D coverage path planning.

However, we discovered that this method was inadequate for handling tasks involving corners and curved surfaces. Therefore, we are now exploring a slicing-based method to address these challenges.

## Project Status

This project is still in progress...


<!--more-->
