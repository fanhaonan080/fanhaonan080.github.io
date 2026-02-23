---
layout: single
title: "Cable-Driven Actuator for Exoskeletons and Human–Robot Interaction"
permalink: /projects/cable-actuator/
author_profile: true
toc: true
toc_label: "Contents"
toc_icon: "cog"
---

I led control development and experimental validation of a **cable-driven actuator** with programmable compliance for wearable robotics. The actuator maintains continuous cable tension to eliminate slack and enables controlled force output during both low-force and high-force operation.

<img src="/images/projects/1_Cable_Driven_Actuator/actuator_design.png" alt="Actuator Design" width="600">

---

## Problem

Cable-driven systems are lightweight but suffer from slack, nonlinear force transmission, and reduced control bandwidth under dynamic loading. Slack causes impact during cable re-engagement and loss of output displacement tracking.

The objective was to design a compact, lightweight actuator that regulates minimal tension to keep the cable continuously engaged, rejects disturbances in low-force mode, and transitions to high-force output without overshoot or instability.

---

## Technical Contributions

I built the cable transmission model and elastic element model, designed the force-control architecture, and implemented the full control codebase with Moteus motor controller integration.

I developed a higher-speed version for foot-placement perturbation experiments and built a torso perturbation setup capable of 200 N output using TTL-triggered control via DAQ.

I modified the Moteus firmware to enable direct IMU acquisition, allowing the motor controller to serve as a centralized sensing and actuation interface for the exoskeleton system.

---

## Experimental Validation

Benchtop experiments included:
- Step-response force tracking
- Frequency-sweep disturbance rejection testing
- Force-control evaluation under multiple programmable stiffness settings

<img src="/images/projects/1_Cable_Driven_Actuator/experimental_setup.png" alt="Experimental Setup" width="400">

---

## Human Perturbation Study

The actuator was tested to apply perturbations to the fast moving body segments like the foot during walking to help study human balance.

<img src="/images/projects/1_Cable_Driven_Actuator/foot_perturbation.png" alt="Foot Perturbation" width="400">

---

## Outcomes

- Developed and implemented a unidirectional cable-driven actuator without cable disengagement
- Force control settling time < 0.1 s
- Controlled force output up to 200 N
- Enabled controlled perturbation experiments for fast moving body segments
- Deployed in multiple exoskeleton research setups
- Submitted as a peer-reviewed journal manuscript (under review)

---

[← Back to Projects](/projects/)
