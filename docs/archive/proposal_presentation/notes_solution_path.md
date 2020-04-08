---
title: 'Solution Path / Our Plan'
author: Peter Deutsch
---

> This document contains the key notes/points/script for the
> Milestone I presentation in regards to solution path. Use the final copy of the *proposal document* for reference.

<!-- Insert your content below -->
### Slide #1
__Ultimate Deliverables__
 * Drone-mounted FPGA platform with interfaced camera
 * Machine-learning implementation using an existing model (i.e. tiny-yolo)
   * Pedestrian detection, detecting one or more pedestrians with bounding boxes -> Not the most important aspect!
   * We will _not_ be designing our own neural network, nor are we going to attempt to synthesize a large model using HLS
   * Use of accelerators, likely facilitated through use of a soft-processor
 * Drone-mounted transmitter & base-station
 * All supplementary docs ([OPS DOC ESPECIALLY IMPORTANT])

### Slide #2
__Four important deliverable dates__

__Oct 15th - Proposal__ (Don't need to include this in the slides)

__Nov 25th - First Prototype__

Tentative Implementation Deliverables:
 * Initial demonstration of ML implementation and camera capture functionality
 * If ahead of schedule, these will be combined into one demo. 
 
__Feb 10th - Second Prototype__

  Tentative Implementation Deliverables:
  * Initial drone, control, transmission, and power systems demonstration
    * Includes initial base-station implementation
  * Continued ML/camera work demo
  
__Apr 3rd - Final Product Delivery__

### Slide #3
__Immediate Steps__

Our approach to developing this platform is:
 * ___Start Small___ - Since this is intended to be a research development platform to be built on, it better for us to have a simple, fully functional implementation rather than a large (yet buggy/incomplete) implementation [FOCUS ON LEGACY RISKS]. We will start with integrating MARLANN, and then duplicate/expand functionality as necessary. 
 * ___Start Quickly___ - We will be presenting the client with potential purchasing combinations next week, with orders sent out shortly after. We expect a large amount of toolchain and integration issues right off the bat, so we need to act fast to target Milestone II.
 * ___Start Legally___ - A big risk is the legal compliance aspect - in particular drone and radio licensing. We are in contact with the UBC UAS team to get additional details regarding legal compliance, but it is expected that this will cause a large amount of overhead (ex. not being able to fly at UBC). 
