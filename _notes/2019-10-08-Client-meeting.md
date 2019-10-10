---
date: 2019-10-08
title: Client meeting
---



The top priority of the three objectives are:

1. Integration of electronics with the drone is the most important because we need the understand how much we can do on a drone – exploration rather than a specific package
2. Video transmission because it is something that’s needed
3. Machine learning model

Ultimate plan: directly compiling machine learning model into a FPGA hardware. We are not worried about the machine learning model, but we’re more concerned about a **compute platform** that has programmable hardware that is compact and light.

We need the biggest FPGA we can find that can be reprogrammed for future purposes.

Updated goal for flight time to 5-10 minutes. 

We need an easy way to reprogram the FPGA while the device is on board.

Quality goals:

- Durability depends on the drone
- (Repeat) flight time is at least 50% of the un-attached flight time
- Accuracy of ML model is not as important
- Performance - real time processing and transmission is preferred
- Accuracy - the intersection of the bounding box with the image

Todo:

- make a budget and selection spreadsheet on potential FPGAs.
- Find the most complex and riskiest part of the project and try to tackle that first. In my (Muchen’s) opinion, given that the system integration is the top-priority requirement, I would start getting a DE1-SoC with some computationally heavy design running and computing the power requirements. Having a WiFi modem onboard and interfacing with them is also important.
- Ask ICICIS for a drone (for research) - loan it to Mieszko Lis. If none is available, propose a spreadsheet of product selection of FPGA + drone combos.