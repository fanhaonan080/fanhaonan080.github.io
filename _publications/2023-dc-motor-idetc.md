---
title: "DC Motor Velocity Control With Integral Retarded Controller Under Unintentional Delay"
collection: publications
category: conferences
permalink: /publication/2023-dc-motor-idetc
excerpt: 'This conference paper addresses DC motor velocity control using integral retarded controllers under unintentional delay conditions, presented at IDETC-CIE 2023. **🏆 Best Paper Award**'
date: 2023-08-01
venue: 'International Design Engineering Technical Conferences and Computers and Information in Engineering Conference (IDETC-CIE)'
slidesurl: # 'http://academicpages.github.io/files/slides6.pdf'
paperurl: 'https://asmedigitalcollection.asme.org/IDETC-CIE/proceedings-abstract/IDETC-CIE2023/87387/1170748'
---

**🏆 Best Paper Award - 19th MSNDC, ASME IDETC-CIE 2023**

This conference paper addresses DC motor velocity control using integral retarded controllers under unintentional delay conditions, presented at IDETC-CIE 2023.

## Abstract

[Add your abstract here if you'd like to include it on the website]

## Key Contributions

- Integral retarded controller for DC motors
- Handling unintentional delays in motor control
- Experimental validation
- Practical implementation considerations

## BibTeX

```bibtex
@proceedings{10.1115/DETC2023-116814,
  author = {Fan, Haonan and Ramírez, Adrián and Mondié, Sabine and Sipahi, Rifat},
  title = {DC Motor Velocity Control With Integral Retarded Controller Under Unintentional Delay},
  volume = {Volume 10: 19th International Conference on Multibody Systems, Nonlinear Dynamics, and Control (MSNDC)},
  series = {International Design Engineering Technical Conferences and Computers and Information in Engineering Conference},
  pages = {V010T10A023},
  year = {2023},
  month = {08},
  abstract = {PID controllers are an industry standard. These controllers are not only effective in many applications, but also intuitive for practitioners to utilize them under a variety of conditions. However, balancing multiple control objectives is still not a trivial task, especially one has to deal with noisy measurements and a relatively high bandwidth of operation is expected from the closed-loop system. An alternative to PIDs has been recently revisited with promising, analytical tuning formula and capabilities to effectively control plants with noisy measurement even without low-pass filters. These controllers are called delay-based controllers whereby an intentional delay is introduced into the controller to improve speed of response, reduce noise, and even improve set point regulation. One such controller is the focus of this manuscript, namely, an Integral Retarded (IR) controller. This controller utilizes an intentional delay to reduce actuator chattering against noisy measurements, while its integral part achieves zero steady-state error for set-point regulation of Type-0 open loop systems. This controller can be tuned analytically to achieve, at the same time, rightmost root placement to render certain speed of response in closed loop. However, measurements can be unintentionally delayed in many applications. IR framework for such cases has not been studied in the literature. Here, we provide new tuning rules for such cases, as well as validations through simulations and a DC motor speed control hardware experiment.},
  doi = {10.1115/DETC2023-116814},
  url = {https://doi.org/10.1115/DETC2023-116814},
  eprint = {https://asmedigitalcollection.asme.org/IDETC-CIE/proceedings-pdf/IDETC-CIE2023/87387/V010T10A023/7062018/v010t10a023-detc2023-116814.pdf},
}
```
