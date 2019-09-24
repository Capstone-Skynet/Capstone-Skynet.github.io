---
title: Client Meeting Agenda
date: 2019-09-24
---

## Agenda

- Team introduction

- Overview of the intent of the meeting

  - We need to get information on high-level goals, and technical pre-requeisits. What do we need to know in order to progress in the project.  

- Need to address the project scope

  - What do we need to build?

- Our vision of the project:

  - There’s four main parts:

    1. Getting “video” data to the FPGA level
    2. FPGA acceleration on processing the frames
    3. Transmission to base station, we need to transmit video as processed ML information
    4. The drone and integration
  - The preliminary requirements in accordance to the above parts are:

    - Setup a working camera that is portable for flight.
    - The camera interfaces with the FPGA or cores that communicate with FPGA.
    - The ML implementation must track an object in real time (each video frame must be processed in real time).
    - Implement accelerator that processes video and produces an output.
    - A working video transmitter (resolution and fps unknown).
    - We are legally allowed to transmit video.
    - We are legally allowed to operate and test the drone.
    - Drone can life off the ground and can be controlled.
    - Drone is battery powered.
    - ML electronics and FPGA electronics must be powered by the battery.
      - Stable voltage and current for the electronics to ensure minimum error due to noise.
  - Budget
    - $650 per team from Capstone
    - We probably need more (depending on the drone and FPGA)
      - Depends on technical requirements
      - Depends on Mieszko’s vision
      - Depends on legacy (what kind of work will be performed after the capstone project).
  
  ---
  
- Also outline the milestone

  - Initial proposal - Oct 15th.
  - Prototype design review - Nov 25th.
  - Prototype design review II - Feb 10th.
  - Prototype design review III - April 7th.

- Deliverables

  - What should we have for the first Milestone
    - Video stream + FPGA (DE1-SoC)
    - Basic (HL) ML implementation
    - FPGA dev board

- We have two different paths:

  - Buy FPGA early and work around the constraints
  - Try figuring out the constraints/requirements and then buy the FPGA with the specs that fits us.

- Confirm work is under MIT license
- Set up regular meetings (when he gets back)

---

Team project and update will be on our team website: https://capstone-skynet.github.io/.

