---
title: Team Meeting
date: 2019-09-17
---

## Agenda

### 1. Slack

- Make sure everyone is active on Slack
- Make sure everyone has notifications of Slack turned on
- Slack channels 

### 2. Capstone-Skynet.github.io

- Repository for documents and files
- “.github.io” is for GitHub pages so we can have it freely deployed.

### 3. Meeting with Client

- Tuesday 11AM didn’t work well today so we need to setup a Skype meeting with the client at some point.
- We need to obtain client’s availability so we can schedule the meeting.

### 4. First Meeting Agenda

- Establish a list of to-dos for that meeting
- Cover the scope of the project
  - Scope of FPGA
  - What kind of development is involved
  - Drone and drone testing (possible UAS license?)
  - Expected acceptance criteria
- Preferred version tracking
- NDA IP specifications

### 5. Administrative Extras

- Gather documents given to us by instructor and TA and complete them by their request



## Meeting Notes

- Mieszko is going to be in China for two or so weeks so a Skype meeting is desired. Desired availability is Tuesday Thursday about 4-5PM PST. For now the next possible date is Tuesday Sept 24th. 
- How us in the right direction to how to learning **machine learning**.
  - Checkout Patrick’s document on “Intro to machine learning”
  - Read up method of machine learning on FPGA.
- Ask how much Verilog is involved.
  - How much do we come up on ourselves
  - How much is using off-the shelf available technologies
- Drone possibly available not from ECE department, but we may have one off-the-shelf.
- Get started on DE1-SoC, the concern is that we don’t want to spend too much time on the IO on the DE1-SoC since we have to re-do that once we refactor IO once we move to a smaller chip.
- Look at the original project proposal in the catalogue and start working on the high-level documents. We need to start working on the **requirements document** immediately, sooner the better.
  - Focus on the project is on the mobile computing platform
  - Break down the project description and turn it into a more objective document.
- Mieszko wants the draft document week of 31st.
- Gather training data once we get the application of the project from Mieszko. Certain training data are openly available.



## Requirements Document

We need to prototype and see what kind of FPGA specifications we need. We need to know if we need a embedded core. 

There’s four main parts:

1. Getting “video” data to the FPGA level
2. FPGA acceleration on processing the frames
3. Transmission to base station, we need to transmit video as processed ML information
4. The drone and integration

---

The preliminary requirements in accordance to the above parts are:

- Setup a working camera that is portable for flight.
- The camera interfaces with the FPGA or cores that communicate with FPGA.
- The ML implementation must track an object in real time (each video frame must be processed in real time).
- Implement accelerator that processes video and produces an output.
- A working video transmitter (resolution and fps unknown).
- We are legally allowed to transmit video.
- We are legally allowed to operate and test the drone.
- Drone can life off the ground and can be controlled.
- Drone is battery powered.

