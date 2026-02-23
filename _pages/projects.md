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

### Technical Contributions
I built the cable transmission model and elastic element model, designed the force-control architecture, and implemented the full control codebase with Moteus motor controller integration.

I developed a higher-speed version for foot-placement perturbation experiments and built a torso perturbation setup capable of 200 N output using TTL-triggered control via DAQ.

I modified the Moteus firmware to enable direct IMU acquisition, allowing the motor controller to serve as a centralized sensing and actuation interface for the exoskeleton system.

### Experimental Validation
Benchtop experiments included:
- Step-response force tracking
- Frequency-sweep disturbance rejection testing
- Force-control evaluation under multiple programmable stiffness settings

<img src="/images/projects/1_Cable_Driven_Actuator/experimental_setup.png" alt="Experimental Setup" width="400">

### Human Perturbation Study
The actuator was tested to apply perturbations to the fast moving body segments like the foot during walking to help study human balance.


<img src="/images/projects/1_Cable_Driven_Actuator/foot_perturbation.png" alt="Foot Perturbation" width="400">

### Outcomes
- Developed and implemented a unidirectional cable-driven actuator without cable disengagement
- Force control settling time < 0.1 s
- Controlled force output up to 200 N
- Enabled controlled perturbation experiments for fast moving body segments
- Deployed in multiple exoskeleton research setups
- Submitted as a peer-reviewed journal manuscript (under review)

---
## Optimization-Driven Linkage Design for Compact Ankle Exoskeleton
This project focuses on the mechanical design and optimization of a compact ankle exoskeleton structure. The objective is to maintain alignment between the device rotation center and the human ankle joint while minimizing overall device size and weight.

The system is **currently under development** and will be integrated with the cable-driven actuator platform. Design details will be published upon completion of the study.

### Design Objective
Ankle exoskeletons must:
- Preserve joint alignment during motion
- Minimize device structural footprint and weight
- Ensure compatibility with footwear and walking gait
The challenge is to satisfy joint-alignment constraints while minimizing overall mechanism size.

### Technical Approach
We developed a parametric linkage model and derived the full kinematic relationships in MATLAB. To determine the optimal configuration, I designed an optimization framework that:
- Minimizes deviation between linkage rotation center and anatomical ankle center
- Penalizes excessive structural dimensions
- Evaluates feasibility across the gait range of motion

The resulting configurations were prototyped using 3D printing and iteratively tested for fit and alignment.

### Current Status
- Kinematic model derived and validated in MATLAB  
- Optimization-based configuration selection implemented  
- Multiple 3D-printed prototypes evaluated for fit  
- Integration with actuator platform in progress  

---

## Physics-Informed Human Joint Torque Estimation for Wearable Robotics
This project develops a joint torque estimation framework for lower-limb wearable robotics by combining biomechanical modeling with data-driven learning. The goal is to estimate biological joint torque in real time using wearable sensor measurements without relying on laboratory-grade motion capture systems.

The system is designed to support exoskeleton control and human–robot interaction studies.

### Problem
Accurate joint torque estimation typically requires motion capture systems and force plates, which are not practical for wearable robotics applications. Wearable sensing introduces challenges including:
- Sensor noise and drift
- Limited observability
- Model uncertainty
- Subject-to-subject variability
The goal is to develop a data-efficient estimation framework that preserves physical consistency while remaining deployable in wearable systems.


### Technical Approach
I developed a hybrid torque estimation framework that combines:
- A physics-based biomechanical model of the lower limb
- Wearable sensor inputs (IMUs, encoders, and force sensing insoles)
- A machine learning module to compensate for modeling errors
The learning module is constrained by biomechanical structure to maintain physically consistent outputs. 

My contributions included formulating the limb dynamics model, designing the hybrid estimation structure, implementing the training and evaluation pipeline in MATLAB and Python (Pytorch, Tensorflow), and integrating the estimator into wearable robotics workflows.

### Current Status
- Biomechanical model formulation completed  
- Estimation framework implemented  
- Ongoing experimental validation using wearable sensor data  


---

## Delay-Aware Consensus and Control of Multi-Robot Systems (PhD Dissertation)

My doctoral research investigated stability and performance of multi-robot systems operating under sensing and communication delays. Delays are traditionally viewed as destabilizing factors; this work reframed them as both constraints and design opportunities.

<div style="text-align: center;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/robot.png" alt="Multi-robot system" width="300" style="display: inline-block; margin: 10px;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/consensus.png" alt="Consensus problem" width="300" style="display: inline-block; margin: 10px;">
</div>

*Figure: Multi-robot systems face coordination challenges under communication and sensing delays. This research develops delay-aware control strategies to maintain stability and accelerate consensus.*

The dissertation developed analytical tools and redesigned delay-based controllers to maintain stability and accelerate consensus in the presence of multiple unintentional delays.

### Core Contributions

**1. Delay Margin Computation for Multi-Delay Systems**

Developed computational tools for delay margin (DM) analysis of linear time-invariant systems with multiple retarded-type delays.  
The framework identifies imaginary-axis crossings directly, enabling scalable stability analysis for large systems without exhaustive root searches.

**2. Redesign of Delay-Based Controllers (PR & IR)**

Modified proportional-retarded (PR) and integral-retarded (IR) controllers to preserve γ-stability under unintentional delays.

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/PR_design_multiagent.png" alt="PR Controller Design" width="600">

*Figure: Proportional-retarded (PR) controller design for multi-agent consensus showing stability regions and parameter selection.*

- Derived stability regions using frequency-domain graphical methods  
- Developed parameter design procedures for single- and multi-agent systems  
- Extended controller redesign from single-DOF systems to multi-robot consensus  

The redesigned controllers were validated through both simulation and experimental studies on networked robotic systems.

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/IR_experimental_setup.png" alt="IR Experimental Setup" width="600">

*Figure: Experimental validation of integral-retarded (IR) controllers on networked robotic platforms demonstrating stable operation under communication delays.*

**3. Accelerated Multi-Robot Consensus**

Integrated predictor-based state estimation and redesigned PR protocols into differential-wheeled multi-robot systems.

<div style="text-align: center;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/Consensus_animation.gif" alt="Consensus Animation" width="500">
</div>

*Figure: Animation showing multi-robot consensus convergence with delay-aware control. Robots achieve coordinated motion despite communication delays.*

Simulation studies demonstrated:
- Up to **39% faster consensus convergence** using PR predictors  
- Up to **23% speed improvement** using multiple-delay PR protocols  
- Stable operation under inherent delays up to 0.3 s 

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/consensus_withPredictor.png" alt="Consensus Results with Predictor" width="600">

*Figure: Consensus performance comparison showing accelerated convergence with predictor-based PR control versus standard delay-free protocols.*

### Impact

This dissertation bridges theoretical delay-system analysis and practical multi-robot coordination, providing tools for designing delay-aware controllers in distributed robotic systems.

Results were published in peer-reviewed control and robotics journals and received Best Paper recognition.
 
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
