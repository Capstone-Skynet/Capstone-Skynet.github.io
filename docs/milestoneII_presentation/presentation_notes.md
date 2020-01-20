---
title: milestone 2 presentaiton points
author: Arthur Hsueh
---

> This document contains the key notes/points/script for the
> Milestone 2 presentation.

<!-- CONTENT BELOW -->

# Presentation 'Slide' points

Remark: bullet points are slide points

## Title Page

blah

## Presentation Overview

* Scope refinement
* Project Requirements
* Project Design
* Project Validation
* Current stage and moving forward
* Demo

## Scope Refinement

<!--- Milestone 1 was the week of Oct 14 -->

Remark: not sure about this. based this off of WSRs since milestone 1 and compared to milestone 1 presentation. May just be included with requirements.

* Machine learning model no longer a top-priority requirement.
* Flying over people and pedestrian detection no longer a requirement.
    * Drone licensing is not required if we fly inside, so we will target indoor use cases

## Requirements

* Defined metrics of the Project (performance, quality, longevity, environmental impact, cost, legality, and safety)
    * Functional, Non-functional and Constraints

## Project Design

Remark: Include the intpic.png we used in the docs

* Computing Platform
    * Platform management board (PMB) - Raspberry Pi
        * Video acquisition and data transmission controller
    * Programmable logic board (PLB) - Digilient Zedboard
        * hardware acceleration functions
    * Base Station - Laptop
        * Video display,  ML analytics and system monitoring
* Multirotor - drone but formally RPAS
    * Will carry the PMB and PLB
    * Controlled independently from the computing platform

## Project Validation

* Devised test procedures that map to the requirements defined in the requirements document
* Manual and Automated tests
    * Manual - cannot be performed by the device itself and must be manually performed by a quality controller
        * ex. Camera characteristics, Drone functionality
    * Automated - Can be monitored by the device itself.
        * ex. wireless connection checking
* Status of the performed tests will be adjusted and recorded in the validation doc as they are performed
    * PEND, FAIL, PASS

## Current stage and moving forward

Remarks: maybe use the APSC 100 design_cycle.JPG? Maybe talk about this after the demos

* Develop and testing Solutions stage
    * Demos show connection between subsystems
* Moving forward <!---Actual work or just overview?-->
    * Gradual full scale creation and integration of other components
    * Testing will be performed to verify fulfillment of requirements
    * Failed test cases will be reviewed and design reiterated

## Demo

* _Zedboard_ Ethernet communication - Peter
* Raspberry Pi Wifi transmission - Wilson & Muchen
* Power Management System - Ardell
* Drone (maybe) - Muchen



---
<!-- SCRIPT -ish -->
### Title slide
Hello Patrick, Amin and Mieszko, thank you for taking the time for this Design Review. Today we are going to give you an overview on the work the Capstone team has completed on the project since Milestone I.

### table of Contents
So to give an overview on what we'll be presenting in this design review, First well talk about some refinements in the project scope and how those affect the project requirements. Following that well give a high level overview on our design of the system and how we're going to validate the defined requirements. We'll then give a demo on the work we've done so far and then finish with the current state of the project and plans for the future.

### Scope Refinement/Requirements
So the first thing was that there has been a slight adjustment in the main requirements defined by the client since milestone 1. Originally the machine learning model was going to be a big part of the project but it is now not a top-level requirement. We'll still be implementing a machine learning model, but the priority will focus on system integration.

The other adjustment was regarding of the ability for the system to fly over and detect pedestrians. Now, these no longer requirements of the project and this will alleviate some of the strictness of the legal constraints.

In general, we've fully defined the metrics of the project, including performance, costs quality and others, and these can be found in the Requirements Document.


### Project Design
Moving onto Proejct Design, after going through mutliple potential designs, we decided on this one (shown on the slide) as it best aligns with the requirements of the project. 

The design is split into to main Compoenents, the Computing platform and the Multirotor. The computing platform is further divided into subsystems which you can see are the PLB, PMB and the Base station. The PLB will perform the hardware accelerations functions of the system, the PMB will perfrom the video capture and data transmission, and the base station will display video and machinel earning analytics as wel as system monitoring.

The multirotor is essentially the drone, but it will be formally called the Remotely Piloted Aircraft System or RPAS and will simply carry the PLB and PMB in flight.

In terms of overall system flow, the camera will first take in live video, feed it to the PMB and which will feed it to the PLB which will perform the processing in hardware. Once the data is processed, it is fed back to the PMB which be tranmissted data to the base station to be analyzed.


### Project Validation
To ensure that the system fulfills the project requirements, we have devised test procedures, which can be found in the Valdiation document. 

Each test procedure maps to the requirements defined in the Requirements document and each has a status of PENDING, PASSED and FAIL will be assigned as the tests are performed. 

Some tests will be automated (self checking), like wireless connection checking between devices, but a large majority will be manually conducted.

### Demo
Now the rest of the team is going to demo the work that we've completed since milestone 1.

### Current state and Moving forward
So currently, if we were to give a stage for where we are in design cycle, we would be on the develop and testing solutions stage. From the demo, we've shown working subsystems and their connections between each other. 

Moving forward, we're going to gradually create more compoenents and integrate them into the project. The tests we've defined will be performed when they are applicable and their statuses will be updated accordingly.

Questions.


