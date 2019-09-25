---
title: Client Meeting
date: 2019-09-24
---

## Agenda

- Team introduction

- Overview of the intent of the meeting

  - We need to get information on high-level goals, and technical pre-req. What do we need to know in order to progress in the project. 

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

Team project and update will be on our team website: <https://capstone-skynet.github.io/>.



## Meeting Notes

We are looking for feasibility. We need to see what kind of drone and FPGA we need. Getting video down to the FPGA level could be using SRAM. Getting ML to work on FPGA could work using HLS. We also need to deal with video transmission to a base station for processing. Lastly, we need to get the drone is the big part.

For training data, ideally we want something a couple of stories high up.

We have some FPGAs laying around which might not get high-resolution processing. Flight duration can be less prioritized for better tracking. We can also give up resolution for this proof of concept. The transmission and processing resolution can be different.

Further investigation required to see if a drone will be available. 

First thing we need to do is figure out what budget we need, which also depends on how big of an FPGA we need. 

Take TensorFlow into *Daniel*‘s work to see if there’s feasibility. The classifier may takes more time, so we may have to decouple the frame rate of the video processed and the frame rate of the transmission as well. Latency is a problem: then just allocate more space.

Transmission and receiver is part of our scope. A Wi-Fi module is recommended. Worst case, run a wire to the drone. All work is open source, but is not limited to MIT license.

In the mean time, we will be working on the proposal document. When Mieszko gets back, we will get further updates. Client is free Tuesday or Thursdays 4PM.