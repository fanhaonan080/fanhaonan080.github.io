---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
toc: true
toc_label: "Projects"
toc_icon: "cog"
---

---
## Cable-Driven Actuator for Exoskeletons and Human–Robot Interaction
I led control development and experimental validation of a **cable-driven actuator** with programmable compliance for wearable robotics. The actuator maintains continuous cable tension to eliminate slack and enables controlled force output during both low-force and high-force operation.

<img src="/images/projects/1_Cable_Driven_Actuator/actuator_design.png" alt="Actuator Design" width="600">

### Problem
Cable-driven systems are lightweight but suffer from slack, nonlinear force transmission, and reduced control bandwidth under dynamic loading. Slack causes impact during cable re-engagement and loss of output displacement tracking.

The objective was to design a compact, lightweight actuator that regulates minimal tension to keep the cable continuously engaged, rejects disturbances in low-force mode, and transitions to high-force output without overshoot or instability.

### My Role
I developed the cable transmission model and elastic element model, designed the force-control architecture, and implemented the full control codebase with Moteus motor controller integration.

I developed a higher-speed version for foot-placement perturbation experiments and built a torso perturbation setup capable of 200 N output using TTL-triggered control via DAQ.

I modified the Moteus firmware to enable direct IMU acquisition, allowing the motor controller to serve as a centralized sensing and actuation interface for the exoskeleton system.

### Experimental Validation
Benchtop experiments included:
- Step-response force tracking  
- Frequency-sweep disturbance rejection testing  
- Force-control evaluation under multiple programmable stiffness settings  

<img src="/images/projects/1_Cable_Driven_Actuator/experimental_setup.png" alt="Experimental Setup" width="400">

**Measured Performance:**
- Force control settling time < 0.1 s
- Continuous cable tension without disengagement  
- Controlled force output up to 200 N
- Implemented TTL-triggered perturbation

### Human Perturbation Study
The actuator applied timed cable perturbations to the foot during walking to evaluate controlled force delivery during gait.

<img src="/images/projects/1_Cable_Driven_Actuator/foot_perturbation.png" alt="Foot Perturbation" width="400">

### Impact
- Converted a slack-prone cable actuator into a continuously tensioned force-control system
- Enabled controlled perturbation experiments during walking  
- Deployed in multiple exoskeleton research setups  
- Submitted as a peer-reviewed journal manuscript (under review)

---

## Ankle Exoskeleton System Development

**Problem:** Ankle exoskeletons

**My Role:** System-level ownership, project lead

**Technical Highlights:**
- Co-designed 
**Results:**
- Delivered 

**Tools:** SolidWorks

![Ankle exoskeleton](/images/projects/ankle-exo.jpg)

---

## Human Joint Torque Estimation Using Physics-Informed Machine Learning

**Problem:** Accurate 

**My Role:** Principal investigator

**Technical Highlights:**
- Developed

**Results:**
- Achieved 

**Tools:** Python 

![Torque estimation](/images/projects/torque-estimation.jpg)

---

## Multi-Robot Consensus Control with Communication Delays

**Problem:** 

**My Role:** Lead researcher 

**Technical Highlights:**
- Designed

**Results:**
- Achieved 

**Tools:** P

![Multi-robot system](/images/projects/multi-robot.jpg)

---

## Robotic Arm Motion Control & Teaching Platform

**Problem:** 

**My Role:** 

**Technical Highlights:**
- Built


**Results:**
- Used in 

**Tools:** MATLAB/Simulink, 

![Robotic arm](/images/projects/robot-arm.jpg)

---

# Personal Projects

---

## Woodworking Projects

**Description:** Custom furniture and home decor projects combining design aesthetics with structural functionality.

**Highlights:**
- T

![Woodworking](/images/projects/woodworking.jpg)

---

## [Add Your Personal Projects]

**Description:** [Brief description of your personal project]

**Highlights:**
- [Key point 1]

![Project image](/images/projects/personal-project.jpg)
