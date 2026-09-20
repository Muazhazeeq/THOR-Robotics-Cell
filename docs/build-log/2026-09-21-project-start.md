\# Build Log — 21 September 2026



\## Objective



Establish the THOR Robotics Cell project and begin understanding the mechanical design before purchasing hardware.



\## Work Completed



\- Created the THOR Robotics Cell Git repository.

\- Published the repository to GitHub.

\- Selected AngelLM/Thor as the mechanical baseline.

\- Recorded the exact upstream revision:



&#x20; `286b081fe6f056d87c379b884781ef77ff6a0159`



\- Created the initial project bill of materials.

\- Downloaded a frozen copy of the upstream THOR repository.

\- Began inspecting the base and Joint 1 components.



\## Joint 1 Investigation



Files inspected:



\- `BaseBot.stl`

\- `BaseTop.stl`

\- `BaseBearingFix.stl`

\- `Art1Bot.stl`

\- `Art1Body.stl`

\- `Art1GearMotor.stl`



\### Current Understanding



Joint 1 provides rotation around the robot's vertical axis.



The base remains stationary while the Art1 assembly and the rest of the robot rotate.



The small `Art1GearMotor` pinion appears to drive the internal gear structure in `Art1Bot`, providing a reduction between the stepper motor and the rotating robot structure.



The Joint 1 load should primarily be supported by the bearing system rather than directly by the motor shaft.



\## Questions Still To Verify



\- Exact Joint 1 bearing specification

\- Exact stepper motor specification

\- Gear tooth counts

\- Gear reduction ratio

\- Bearing stack arrangement

\- Joint 1 homing method

\- Required fasteners



\## Lessons Learned



\- Git commits provide traceability for engineering decisions.

\- A Git commit hash can freeze an exact upstream design revision.

\- STL files show printable geometry, while the original CAD files will be more useful for understanding assemblies and dimensions.

\- Motor torque generation and structural load support should be treated as separate mechanical functions.



\## Next Step



Inspect the original CAD assembly and verify the Joint 1 mechanism before adding components to the BOM.

