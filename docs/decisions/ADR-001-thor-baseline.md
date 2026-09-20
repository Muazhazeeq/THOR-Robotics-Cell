\# ADR-001 — THOR Mechanical Baseline



\## Status



Accepted



\## Problem



A specific mechanical robot design must be selected before purchasing

components, printing the complete robot, developing electronics, or

building the ROS 2 system.



Changing the mechanical design later could invalidate motor selections,

belt lengths, bearings, electronics placement, calibration models and

software assumptions.



\## Options Considered



1\. Design a new 6-DOF robot arm from scratch.

2\. Use a commercial robot arm kit.

3\. Use the open-source THOR robot arm as the mechanical baseline.



\## Decision



Use AngelLM/Thor as the initial mechanical baseline.



Source:



https://github.com/AngelLM/Thor



Upstream revision:



286b081fe6f056d87c379b884781ef77ff6a0159



\## Reason



THOR provides an existing open-source mechanical design while still

allowing substantial engineering work in:



\- mechanical assembly

\- actuator selection

\- electronics

\- embedded control

\- communication

\- ROS 2 integration

\- motion planning

\- calibration

\- computer vision

\- fault handling

\- performance testing



Using an existing mechanical design prevents excessive project time

from being consumed designing an entire manipulator from zero.



\## Important Constraint



The THOR design is a baseline, not a black box.



Subsystems may be modified when there is a clear engineering reason.



In particular, the project intends to investigate a custom ESP32-based

low-level control architecture rather than blindly copying the original

controller.



\## Trade-offs



Advantages:



\- Proven mechanical starting point

\- Existing printable files

\- Existing documentation

\- Existing ROS ecosystem

\- Lower development cost

\- More time available for controls, robotics and experimentation



Disadvantages:



\- Mechanical design is not completely original

\- Existing THOR solutions could make it tempting to copy implementations

&#x20; without understanding them

\- Some original components may be difficult or expensive to source locally



\## Project Rule



Existing THOR implementations may be studied as references, but important

subsystems must be understood, tested and documented rather than treated

as black boxes.

