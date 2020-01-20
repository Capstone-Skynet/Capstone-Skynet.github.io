---
title: Viability
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




<!-- SCRIPT -ish -->