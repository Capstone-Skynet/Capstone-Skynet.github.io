---
title: Requirement and Constraints
author: Wilson Wang
---

> This document contains the key notes/points/script for the
> Milestone I presentation in regards to requirements and constraints. Use the final copy of the *proposal document* for reference.

<!-- Insert your content below -->

## Slide #1

### Requirements

### Drone Requirements

* Capable to lift the entire platform.

* Flying time is at least 10 mins.

* Still controllable while lifting the platform.

### Drone Usage Requirements

* Transmission Canada has requirements regarding the drone usage.

* UBC is within the controlled airspace.

* Nav Canada has requirements regarding drone usage within the controlled airspace.

### Transmission Requirements

* Most off-the-shelf transmitters are working at 2.4/5GHz

* Need an amateur radio certification.

## Slide #2

### Constraints

### FPGA capability

* The FPGA platform is intended to be used as a development platform in the future.

* It should be future-proofed for further modifications, i.e. deploy new machine learning models onto it.

* The FPGA is expected to work under complex work environment - up in the air near four high-power motors and a lot of other electronic devices. FPGA may not function correctly under these circumstances.

### Transmission capability

* Ultimately, videos and the result form the machine learning model will be transmitted back to the ground station wirelessly.

* The transmitter should have enough bandwidth to transmit video that has a resolution of at least 640x480 and 30 frames per second along with the result from machine learning model. 

### Testing

* Can not test the drone without a licence

* The platform is not water-proofed, weather condition is a great factor.