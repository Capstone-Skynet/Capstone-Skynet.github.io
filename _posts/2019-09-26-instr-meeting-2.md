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

- Any flying object need to be registered with Transport Canada.
- Drone is piloted, so the pilots need license and training.
- This project involves flying drones close (less than 30m radius) to people, and thus require additional licensing from Transport Canada.
- Video transmission on certain frequencies require license.



## Project Proposal Progress

**Arthur + Muchen**:

- Created the skeleton for the document in LaTeX
- Version tracked using GitHub



