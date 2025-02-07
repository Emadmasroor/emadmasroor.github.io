---
title: Numerical Solution of Initial Value Problems
description: 
code: E91
term: Spring 2025
institution: Swarthmore College
giscus_comments: false
tags: teaching 
date: 2025-01-01
layout: distill
permalink: /classes/E91_S25/Labs/Lab1

authors:
  - name: Emad Masroor
    url: "https://emadmasroor.github.io"
    affiliations:
      name: Swarthmore College
      department: Department of Engineering
      state: 


bibliography: 


toc:
  - name: Introduction



---

# Lab 1: Linearity, Nonlinearity, and the Compound Pendulum

## Introduction
In this lab, you will ...

## Equipment and hardware

This lab makes use of a compound pendulum mounted onto a potentiometer. The compound pendulum is made of Aluminum, and measures 10" x 1" x 1/4". It is secured with the help of a set-screw to the shaft of the poteniometer. The potentiometer is the [Vishay Spectrol 157-11103](https://www.vishay.com/docs/57042/157.pdf), which provides a voltage reading that is expected to scale, hopefully linearly, with the angle of rotation of the shaft. The potentiometer is wired with alligator clips: red for power, black for ground, and white for the voltage reading.

Data collection is carried out using the [Analog Discovery 3](https://digilent.com/shop/analog-discovery-3/), a multi-purpose data acquisition and signal-generating device. In this lab, the Analog Discovery powers the potentiometer by providing 5V across pins 1 and 3, and reads the voltage from pin 2.

## Software
This lab will make use of the open-source software [WaveForms](https://tinyurl.com/E91LabSoftware) from Digilent, the manufacturer of the analog I/O device that you'll use to collect data. Download WaveForms, install it on your computer, and bring it with you to the lab.

WaveForms can load a 'workspace', which is a collection of settings that you can pre-load when you run WaveForms. Download the workspace needed for this lab [here]({{ page.permalink }}/../Lab1Workspace.dwf3work). It will look something like this:

![workspace]({{ page.permalink }}/../waveforms.png){:style="max-width: 100%; height: auto;"}

A reference manual for WaveForms is available [here](https://digilent.com/reference/software/waveforms/waveforms-3/reference-manual).

## Wiring and Connections

The wiring should already be set up for you; all you need to do is plug in the USB-c cable from the Analog Discovery. In case you need to re-wire the potentiometer to the Analog Discovery:

- Connect the red wire to V+
- Connect the black wire to any GND
- Connect the white wire to 1+

## Testing and calibration


After connecting your Analog Discovery to your computer and opening WaveForms, the software should recognize the Discovery 3 with a panel on the bottom right as shown here.

![connected]({{ page.permalink }}/../pic1.png){:style="max-width: 100%; height: auto;"}

Start scanning the voltage reading by clicking 'scan' near the top left, which will start a real-time scan of the voltage reading from the potentiometer. Make sure that 'mode' is set to 'Screen' as shown here. ![scan]({{ page.permalink }}/../pic2.png)

You should see a trace of the voltage develop across the screen. 'C2' reads the voltage directly, whereas 'M1' is a moving average that acts as a low-pass filter, smoothing out the noise in the voltage. ![gif1]({{ page.permalink }}/../gif1.gif))



## The Initial Value Problem
Numerically solve the initial value problem given by

$$ \dot{y} = \sin y, \, y(0) = \pi/6.$$

## Using Python

You must have the packages `scipy`, `numpy`, and `matplotlib` installed in order to use the import statements shown below. If you don't know how to install these packages, please see the tutorial [here](https://packaging.python.org/en/latest/tutorials/installing-packages/).

```
from scipy.integrate import solve_ivp
import matplotlib.pyplot as plt
from numpy import array,exp,sin,pi,linspace

def f1(t,x):
    return sin(x)

x_init      = array([pi/6]) 
t_vector    = linspace(0,2*pi,100)
solution1   = solve_ivp(f1,                         # r.h.s of diff. eq
                        (t_vector[0],t_vector[-1]), # start & end time
                        x_init,                     # initial condition
                        t_eval=t_vector)            # times to plot

plt.figure(1)
plt.plot(solution1.t,solution1.y[0],'r.-')
plt.grid()
plt.xlabel('t')
plt.ylabel('x(t)')
plt.show()    # uncomment to preview figure
```

![Python image](python_ivp.png){:style="max-width: 100%; height: auto;"}

## Using Mathematica

```
solution = 
 NDSolve[{y'[t] == Sin[y[t]], y[0] == \[Pi]/6}, y[t], {t, 0, 2 \[Pi]}]

Plot[y[t] /. solution, {t, 0, 2 \[Pi]}]
```

![Mathematica image](mathematica_ivp.png){:style="max-width: 100%; height: auto;"}

## Using MATLAB

```
x_init      = pi/6;
t_vector    = linspace(0,2*pi,100);
[t,x]       = ode45(@rhs,t_vector,x_init);

figure(1);
plot(t,x,LineWidth=2,Marker=".",MarkerSize=12,Color='Red');
xlabel('t');
ylabel('x(t)');
grid on;
```

For this to work, you must have the file `rhs.m` in the same directory, and the file should contain:

```
function [dydt] = rhs(t,y)
dydt = sin(y);
end
```

![MATLAB image](matlab_ivp.png){:style="max-width: 100%; height: auto;"}
