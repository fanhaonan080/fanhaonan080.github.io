---
layout: single
title: "Delay-Aware Consensus and Control of Multi-Robot Systems"
permalink: /projects/multi-robot-systems/
author_profile: true
toc: true
toc_label: "Contents"
toc_icon: "cog"
---

My doctoral research investigated stability and performance of multi-robot systems operating under sensing and communication delays. Delays are traditionally viewed as destabilizing factors; this work reframed them as both constraints and design opportunities.

<div style="text-align: center;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/robot.png" alt="Multi-robot system" width="300" style="display: inline-block; margin: 10px;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/consensus.png" alt="Consensus problem" width="300" style="display: inline-block; margin: 10px;">
</div>

*Multi-robot systems face coordination challenges under communication and sensing delays. This research develops delay-aware control strategies to maintain stability and accelerate consensus.*

The dissertation developed analytical tools and redesigned delay-based controllers to maintain stability and accelerate consensus in the presence of multiple unintentional delays.

---

## Core Contributions

### 1. Delay Margin Computation for Multi-Delay Systems

Developed computational tools for delay margin (DM) analysis of linear time-invariant systems with multiple retarded-type delays.  
The framework identifies imaginary-axis crossings directly, enabling scalable stability analysis for large systems without exhaustive root searches.

---

### 2. Redesign of Delay-Based Controllers (PR & IR)

Modified proportional-retarded (PR) and integral-retarded (IR) controllers to preserve γ-stability under unintentional delays.

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/PR_design_multiagent.png" alt="PR Controller Design" width="600">

*Proportional-retarded (PR) controller design for multi-agent consensus showing stability regions and parameter selection.*

- Derived stability regions using frequency-domain graphical methods  
- Developed parameter design procedures for single- and multi-agent systems  
- Extended controller redesign from single-DOF systems to multi-robot consensus  

The redesigned controllers were validated through both simulation and experimental studies on networked robotic systems.

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/IR_experimental_setup.png" alt="IR Experimental Setup" width="600">

*Experimental validation of integral-retarded (IR) controllers on networked robotic platforms demonstrating stable operation under communication delays.*

---

### 3. Accelerated Multi-Robot Consensus

Integrated predictor-based state estimation and redesigned PR protocols into differential-wheeled multi-robot systems.

<div style="text-align: center;">
  <img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/Consensus_animation.gif" alt="Consensus Animation" width="500">
</div>

*Animation showing multi-robot consensus convergence with delay-aware control. Robots achieve coordinated motion despite communication delays.*

Simulation studies demonstrated:
- Up to **39% faster consensus convergence** using PR predictors  
- Up to **23% speed improvement** using multiple-delay PR protocols  
- Stable operation under inherent delays up to 0.3 s 

<img src="/images/projects/4_Multi_Robot_Fast_Consensus_Using_Delays/consensus_withPredictor.png" alt="Consensus Results with Predictor" width="600">

*Consensus performance comparison showing accelerated convergence with predictor-based PR control versus standard delay-free protocols.*

---

## Impact

This dissertation bridges theoretical delay-system analysis and practical multi-robot coordination, providing tools for designing delay-aware controllers in distributed robotic systems.

Results were published in peer-reviewed control and robotics journals and received Best Paper recognition.

---

[← Back to Projects](/projects/)
