---
layout: single
title: "Physics-Informed Human Joint Torque Estimation for Wearable Robotics"
permalink: /projects/torque-estimation/
author_profile: true
toc: true
toc_label: "Contents"
toc_icon: "cog"
---

This project develops a joint torque estimation framework for lower-limb wearable robotics by combining biomechanical modeling with data-driven learning. The goal is to estimate biological joint torque in real time using wearable sensor measurements without relying on laboratory-grade motion capture systems.

The system is designed to support exoskeleton control and human–robot interaction studies.

---

## Problem

Accurate joint torque estimation typically requires motion capture systems and force plates, which are not practical for wearable robotics applications. Wearable sensing introduces challenges including:
- Sensor noise and drift
- Limited observability
- Model uncertainty
- Subject-to-subject variability

The goal is to develop a data-efficient estimation framework that preserves physical consistency while remaining deployable in wearable systems.

---

## Technical Approach

I developed a hybrid torque estimation framework that combines:
- A physics-based biomechanical model of the lower limb
- Wearable sensor inputs (IMUs, encoders, and force sensing insoles)
- A machine learning module to compensate for modeling errors

The learning module is constrained by biomechanical structure to maintain physically consistent outputs. 

My contributions included formulating the limb dynamics model, designing the hybrid estimation structure, implementing the training and evaluation pipeline in MATLAB and Python (Pytorch, Tensorflow), and integrating the estimator into wearable robotics workflows.

---

## Current Status

- Biomechanical model formulation completed  
- Estimation framework implemented  
- Ongoing experimental validation using wearable sensor data  

---

[← Back to Projects](/projects/)
