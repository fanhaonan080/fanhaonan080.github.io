---
layout: single
title: "Projects"
permalink: /engineering/
author_profile: true
toc: true
toc_label: "Projects"
toc_icon: "cog"
---

---

## Cable-Driven Actuator with Programmable Elasticity

**Problem:** Traditional rigid actuators cannot safely adapt to variable loads in wearable robotics and rehabilitation devices. Existing variable stiffness actuators are complex, heavy, and difficult to control.

**My Role:** Lead researcher — designed mechanical system, developed control algorithms, conducted all experimental validation.

**Technical Highlights:**
- Designed novel cable-driven mechanism enabling real-time stiffness modulation (0.5–5 Nm/rad range)
- Implemented force-field rendering control with impedance parameter optimization
- Developed embedded control system with 1 kHz loop for torque and position tracking
- Integrated multi-sensor fusion (encoders, load cells) for precise force/position estimation

**Results:**
- Achieved <5% steady-state error in stiffness rendering across full range
- Validated human-in-the-loop interaction with 10+ subjects
- Demonstrated 60% weight reduction vs. comparable systems
- Published in *IEEE Transactions on Control Systems Technology*

**Tools:** MATLAB/Simulink, C/C++ (embedded), SolidWorks, dSPACE, CAN bus

![Cable-driven actuator](/images/projects/cable-actuator.jpg)

---

## Ankle Exoskeleton System Design & Control

**Problem:** Ankle exoskeletons for gait assistance require precise torque delivery synchronized with human walking dynamics, while remaining lightweight and backdrivable.

**My Role:** Co-lead — mechanical design, actuation system integration, motion control implementation.

**Technical Highlights:**
- Co-designed lightweight (2.3 kg) cable-driven ankle exoskeleton with 4-bar linkage transmission
- Implemented phase-based assistive torque control synchronized to gait cycle detection
- Developed real-time trajectory planning for smooth torque transitions
- Integrated IMU and encoder feedback for robust state estimation during walking

**Results:**
- Delivered up to 30 Nm assistive torque with <50ms latency
- Validated on treadmill walking (0.8–1.5 m/s speeds) with multiple subjects
- Achieved metabolic cost reduction in preliminary trials
- Published in *ASME Journal of Computational and Nonlinear Dynamics*

**Tools:** SolidWorks, MATLAB, Python, Arduino, 3D printing, motor drives (FOC)

![Ankle exoskeleton](/images/projects/ankle-exo.jpg)

---

## Human Joint Torque Estimation Using Physics-Informed Machine Learning

**Problem:** Accurate joint torque estimation during dynamic movements requires expensive force sensors or complex biomechanical models. Can we achieve sensor-less estimation with minimal training data?

**My Role:** Principal investigator — algorithm development, experimental design, data collection and analysis.

**Technical Highlights:**
- Developed hybrid physics-informed neural network combining rigid body dynamics with learned corrections
- Integrated biomechanical constraints (joint limits, torque bounds) into loss function
- Implemented real-time estimation pipeline processing IMU and kinematic data
- Validated against ground-truth dynamometer measurements

**Results:**
- Achieved <8% RMSE on unseen movements with only 5 minutes of training data
- Outperformed pure data-driven methods by 35% in generalization
- Real-time inference (<10ms latency) on standard hardware
- Published in *IEEE Control Systems Letters*

**Tools:** Python (PyTorch), MATLAB, motion capture system, IMU sensors

![Torque estimation](/images/projects/torque-estimation.jpg)

---

## Multi-Robot Consensus Control with Communication Delays

**Problem:** Coordinating multiple robots over wireless networks introduces time delays that destabilize traditional consensus algorithms, especially in fast-moving systems.

**My Role:** Lead researcher — controller design, stability analysis, hardware implementation and testing.

**Technical Highlights:**
- Designed predictor-based distributed consensus controller robust to time-varying delays (50–300ms)
- Proved stability using Lyapunov-Krasovskii functional analysis
- Implemented on network of 4 differential-drive robots with WiFi communication
- Developed ROS-based framework for distributed control and data logging

**Results:**
- Achieved consensus within 5 seconds despite 200ms average delay
- 70% faster convergence than delay-independent methods
- Zero collisions in 50+ experimental trials
- Published in *IEEE Transactions on Control of Network Systems* and *American Control Conference*

**Tools:** Python, C++, ROS, MATLAB, Raspberry Pi, motor controllers

![Multi-robot system](/images/projects/multi-robot.jpg)

---

## Robotic Arm Motion Control & Teaching Platform

**Problem:** Educational robotics platforms often lack transparent low-level control access, limiting students' ability to learn practical servo tuning and trajectory planning.

**My Role:** System architect — designed control architecture, developed teaching modules, mentored 15+ students.

**Technical Highlights:**
- Built 6-DOF robotic arm teaching platform with modular control architecture
- Implemented multiple control modes: joint-space PID, workspace impedance, trajectory tracking
- Developed user-friendly MATLAB/Simulink interface for parameter tuning
- Created hands-on labs covering kinematics, dynamics, and feedback control

**Results:**
- Used in 3 semesters of graduate robotics course (45 students)
- Students achieved autonomous pick-and-place tasks within 4-week module
- Open-sourced control framework (GitHub: 200+ stars)
- Reduced lab setup time by 60% vs. previous platform

**Tools:** MATLAB/Simulink, Arduino, Dynamixel servos, forward/inverse kinematics

![Robotic arm](/images/projects/robot-arm.jpg)

---

[Add more projects as needed]
