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
For $$x = 100 \mathrm{mm},$$ measure the velocity profile $$u(y)$$ using a stepping size $$\Delta y$$ of your choice. Use this informaiton to plot 
- the velocity profile $$u(y)$$ against $$y$$ in dimensional form (i.e., with units)
- the non-dimensional quantities $$u(y)/U$$ against $$\eta = \frac{y}{x}\sqrt{\frac{U x}{2 \nu}} = \frac{y}{x} \sqrt{Re_x/2}$$

#### Comparison with Blasius' Theory
Numerical solutions of the Blasius equations suggest that $$u/U$$ as a function of $$\eta = \frac{y}{x} \sqrt{Re_x/2}$$ takes on the following graphical form. A `csv` file containing this information is included [here](../assets/csv/uU_Blasius.csv).

{% include figure.html path="assets/img/Blasius_profile.jpg" title="Blasius profile" class="img-fluid rounded z-depth-1" width="240px" %} 

### Main Experiment
##### Parameters
For three different free-stream speeds $$U$$ and three different downstream locations $$x,$$ make measurments of $$u(y)$$. Choose an appropriate number of steps in $$y$$ and range of $$y$$ values that will allow you to scan the entirety of the boundary layer (and some part of the free stream) for each of the nine sets of data you will collect.
- **Speeds**: $$ U = 10, 20, 40 \mathrm{m}/\mathrm{s}$$
- **Locations**: $$ x = 50, 150, 250 \mathrm{mm}$$

#### Programmatically conducting experiment
Write a MATLAB script that will collect the entire set of data for this experiment. Use your plots of $$\delta_{99}(x)$$ to determine the values of $$y$$ at which measurmenets will be taken.

### Compiling Results
Generate:
1. A 3x3 grid of plots showing the velocity profile in each of the nine experiments that you conducted.
2. A single plot that combines this information into non-dimensional form. Do not connect your data plots with lines. Overlay on this plot the Blasius profile.


