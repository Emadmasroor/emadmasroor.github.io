---
layout: page
permalink: /teaching/
title: teaching
description: Course Materials
nav: true
nav_order: 2
---

## E83 Lab 5: Boundary Layers
In this lab, you will measure the streamwise flow velocities in the boundary layer of a flat plate placed in a wind tunnel. Your goal is to see the extent to which an experimentally observed boundary layer agrees with the Blasius solution for laminar flow. If possible, you will also observe a turbulent boundary layer and see how it differs from a laminary boundary layer.

### MATLAB code for conducting experiment
You are provided with a series of MATLAB routines, listed below. 

1. `connectController.m`: connect the linear actuator that moves the flat plate to MATLAB.
2. `disconnectController.m`: disconnect the linear actuator that moves the flat plate from MATLAB.
3. `getPlatePosition.m`: Returns, in mm, the current position of the flat plate.
4. `resetPlatePosition.m`: Moves the flat plate downstream until limit switch is activated, then sets this position as zero.
5. `movePlate.m`: Moves the flat plate upstream (positive argument) or downstream (negative argument) a specified number of millimeters. Returns as output the position at the end of the move.
6. `moveHotWireYZ.m`: Moves the hot wire in the vertical direction (positive up) by a specified number of millimeters. Y motion has been disabled for this lab.
7. `readHotwire.m`: Reads the current horizontal speed in the wind tunnel using the hot wire, in meters per second.
8. `RPM.m`: increases the speed of the fan inside the wind tunnel to the specified value.
9. `waittilRPM.m`: incorporates a delay until the specified fan speed has been reached.

### Preliminary Steps
#### Theory
Before conducting measurements in the wind tunnel, prepare the following plots using your knowledge of the laminary boundary layer in air. Recall that air has a kinematic viscosity of $$1.5 \times 10^{-5}.$$
1. Plot the Reynolds number $$Re_x = U x / \nu$$ as a function of $x$, the downstream distance from the leading edge, for three different values of the free stream speed $$U = 10, 20, 40$$ meters per second. Choose an appropriate range on the horizontal and vertical axes, and use a log scale for the vertical axis.
2. Plot the approximate height of the boundary layer, $$\delta_{99},$$ as a function of $$x,$$ the downstream distance from the leading edge, for three different values of the free stream speed $$U = 10, 20, 40$$ meters per second. Choose an appropriate range on the horizontal and vertical axes, and use a log scale for the vertical axis.

#### Trial experiment
For $$x = 100 \mathrm{mm}$$, measure the velocity profile $$u(y)$$ using a stepping size $$\Delta y$$ of your choice. Use this informaiton to plot 
- the velocity profile $$u(y)$$ against $$y$$ in dimensional form (i.e., with units)
- the non-dimensional quantities $$u(y)/U$$ against $$\eta = \frac{y}{x}\sqrt{\frac{U x}{\nu}} = \frac{y}{x} Re_x$$

### Main Experiment
For three different free-stream speeds $U$ and three different downstream locations $$x$$, make measurments of $$u(y)$$. Choose an appropriate number of steps in $$y$$ and range of $$y$$ values that will allow you to scan the entirety of the boundary layer (and some part of the free stream) for each of the nine sets of data you will collect.
**Speeds**: $$ U = 10, 20, 40 \mathrm{m}/\mathrm{s}$$
**Locations**: $$ x = 50, 150, 250 \mathrm{mm}$$


