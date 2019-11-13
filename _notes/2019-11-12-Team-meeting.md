---
date: 2019-11-12
title: Team Meeting and Project Plan Update
author: Muchen He
---

- toc
{:toc}

## Raspberry Pi WiFi

There are two options we are now considering for using WiFi to transmit data from the PI to a client (computer or phone). 

### 1. PI as Hotspot

The PI will open up a WiFi hotspot and will essentially act as a router. And there will be a WiFi option one can connect to from their computer.

### 2. PI Connects to Existing Network

Alternatively, the PI uses its WiFi module and connect to an existing WiFi network: either `ubcsecure` or setup our own router + wireless network. Using `ubcsecure` is less predictable and has a higher risk of not working for the demo.

### Hosting Webserver

Regardless of the two options above, our current plan is to have PI host a webserver on *some* network. The webserver hosts a simple website that has some client-side JavaScript that receives data (from socket.io for example) and display it to the client.

## PI &harr; FPGA (PF) Interface

It is suggested that Ethernet could be a viable alternative to HDMI input to the FPGA. Ethernet is beneficial as it offers more bandwidth and require less encoding/decoding. If implemented correctly, the interface should not be a bottleneck.

The output data from the FPGA could also use Ethernet. The back-up plan for output data is to use serial, but this is unlikely.

### Work Required

The work done on the Raspberry Pi to get Ethernet working should be straight forward (according to Peter and Wilson). Peter will test the PF interface using his laptop in substitution for a PI.

## Milestone 2 Deliverables

### 1. Video Stream Pt. 1

We need a successful implementation of the data flow from the camera output &rarr; PI &rarr; output somewhere. The output of this system could be as simple as an HDMI screen.

### 2. Video Stream Pt. 2

We need a successful implementation of PI serving a client device (laptop) via WiFi. The served content should stream a video. Refer to [webserver section](#hosting-webserver) for details, but the gist is to have some JavaScript to plays the video on the client side.

### 3. Bidirectional Ethernet Communication

We need a successful implementation of a bidirectional ethernet communication between the FPGA board and a computer device (either PI or a laptop). A sample setup could be using ethernet to turn on LEDs on the FPGA or have a loop-back.

### 4. Updated Documents

We need to have a draft document for all the documents listed in the *proposal - deliverables* section.

#### Requirements Document

We have updated requirements from Mieszko. So this document should be drafted according to that. Essentially:

- Machine learning model no longer a top-priority requirement.
- Flying over people and pedestrian detection no longer a requirement.

Some **functional-requirements** to research and add:

- Power requirements of the payload: all of computing equipment.

Some **non-functional-requirements** to research and add:

- Safety requirements regarding:
  - Battery & battery charging
  - Motors & propellers
  - Indoor flying
  - Drone pilot practice and training

#### Verification Document

Basically everything we’re prototyping at this moment are experiments and tests (i.e. Ethernet tests, PI WiFI tests) used to verify part of our system design. 

Also part of the verification is the Excel sheet Muchen created to analyze the flight performance and electro-mechanics of the drone parameters.

Include the above content into the verification document draft.

#### Operations Document

Muchen will start a very rough draft on drone operations.

## Update Risks

With the above information, update the risk matrix accordingly. Add / remove / modify risk details if necessary.

## Record Everything

To aid the final deliverable (demonstration video), verification document, and for archiving purposes. Please use your camera to log/record all the tests/experiments/progress. 

This allows better progress tracking and we can use it later as evidence to justify design decisions.

For now, just keep the recorded footage on your devices (phones, cameras, etc.). Make sure to label the video by starting the video with date, time, and purpose. 

We could have a cloud drive if we need a place to store an archive of large files like these.