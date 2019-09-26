---
title: Weekly Status Report
date: 2019-09-26
---

## Meeting with the Client

- Established high level goals of the project
  - In alignment with our initial speculated requirements:
    1. Working interface and transmission of video data from the camera to the hardware <!-- excerpt -->
    2. Successful implementation of real-time object tracking acceleration in hardware
    3. Successful transmission of the output of the hardware from the drone to a ground station.
    4. (Priority lowered) Adequate integration of FPGA hardware, electronics, and drone.
  - Some "nice-to-haves" but very-low-priority are :
    - High resolution; this can be a trade off to obtain better processing speed
    - High(er) definition video transmission to ground station; not the top priority if we can transmit low resolution, or just the processed data.
    - Long flight time; because one could always attach the FPGA implementation onto a bigger drone
  - Overall scope is depended on budget; budget is not determined.



## Refined Our Development Process

- Our Trello board is located here: <https://trello.com/b/SvxPAhTo/capstone-2019-2020>
- To-dos are appended to the "Backlog".
- Every **team meeting** (Tuesday afternoon), we do a standup – we describe what we’ve done in the last week (any success, fail, roadblocks, unexpected things, etc).
- After, we select the tasks from the *Backlog* and assign **priority** and **assignee** so that everyone has something todo for that sprint period. The task is now placed in the “Triage” list.
- Team members work on the task, placed in “In Progress”. Once it’s done, it moves to “Review”.
- Lastly, before the next team meeting, the task cards are cleaned up and placed in “Done”.



## Generated a List of Preliminary Potential Risks

From our team meeting notes: <https://capstone-skynet.github.io/notes/2019/09/24/Team-Meeting>.

**Peter + Ardell**:

- Risk management spreadsheet
- Risk probability
- Risk categories
- Top concerned risks



## Regulatory Requirements for Drone and Radio Transmission

**Peter + Wilson**:

- Transport Canada outlines restrictions and regulations regarding drone usage.
- There are two (relevant) drone categories outlined by Transport Canada for flying drones **over 250 grams**:
 - **Basic Operations** - if you are flying in **uncontrolled airspace** and flying more than 30 meters horizontally from bystanders.
  - Requires the operator to pass a basic examination and register the drone with Transport Canada.
 - **Advanced Operations** - if you are flying in controlled airspace, over bystanders, or within 30 meters of bystanders.
  - Requires the operator to pass an advanced examination, register the drone with Transport Canada, and pass an **in-person** flight review.
  - Also requires that the drone has an RPAS safety certification, and an additional waiver if modifications are made.

- As Vancouver/UBC are within restricted airspace envelopes, additional requirements are enforced by Nav Canada.
 - To fly at UBC, we'd need written permission from UBC, provide 48 hours notice to Nav Canada, and restrict access to the ground below the drone.
 - These requirements likely make it too onerous for us to fly at UBC. We might have to fly demo/capture flights in other geographical areas (ex. Abbotsford).

- Peter will liason with the UBC Unmanned Aircraft Systems team for advice regarding navigating regulatory requirements.

- On transmission outside of the 2.4/5GHz bands, an amateur radio certification is required.
 - If we use off-the-shelf WiFi/Bluetooth components this will not be a problem, but a custom transmission solution might require it.
 - During the transmitter's operation *at least one* licence holder must be present, so it's not necessary that the entire team goes through the process.
 - The turn-around time for acquiring a license is low (a few days), so this is a low risk item.



## Project Proposal Progress

**Arthur + Muchen**:

- Created the skeleton for the document in LaTeX
- Version tracked using GitHub



