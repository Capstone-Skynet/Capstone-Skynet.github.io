---
title: Context and Purpose
author: Ardell Wilson
---

> This document contains the key notes/points/script for the
> Milestone I presentation in regards to the context and purpose. Use the final copy of the *proposal document* for reference.

<!-- Insert your content below -->
Recent years have seen dramatic improvements and increases in use of two technologies, machine learning and drones. The two have even been combined and drone based machine learning platforms are beginning to be used in a plethora of areas, such as inspecting powerlines and wildlife conservation. Typically machine learning algorithms use GPUs to do their computations, but these have drawbacks and limitations. FPGAs are potentially better platforms for machine learning algorithms. While FPGAs have been used for machine learning, to the best of our knowledge no one has done FPGA based machine learning on a drone before. 

Thus, our project will be to implement an FPGA based machine learning algorithm onto a drone. This technology has the potential to address problems that existing drone based ML systems cannot, or to tackle problems more efficiently and effectively.

The platform that we plan on building will be as follows. A camera will connect to either to a digital video processing device or directly to the FPGA if we do the video processing on the FPGA. The pedestrian data as well as the video will then be sent to a transmitter so that both can be relayed down to a base station which will display the video overlaid with the ML data. The FPGA, camera, transmitter and support hardware will be powered either from the drone power supply or from a separate power supply and power management hardware.

The primary goal of this project is to build a research platform. For the purpose of a proof of concept we will have a working ML algorithm in our final product, the algorithm is going to detect pedestrian on the ground. That said our main goal is to build the most capable drone-FPGA combination possible. This means that it must have the most capable FPGA possible and also fly for as long as possible.

My teammate will now talk more about our requirements and constraints.


