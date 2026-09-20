\# THOR Robotics Cell — Bill of Materials



\## BOM Status



This BOM is under development.



Parts must not be purchased until compatibility with the selected THOR revision has been verified.



Baseline THOR revision:



`286b081fe6f056d87c379b884781ef77ff6a0159`



\## Status Definitions



\- REQUIRED — Needed for the core robot

\- VERIFY — Specification still needs confirmation

\- PURCHASED — Already obtained

\- OPTIONAL — Not required for initial operation

\- DEFERRED — Intentionally postponed



\## Mechanical Components



| Subsystem | Part | Qty | Specification | Status | Source | Cost | Notes |

|---|---|---:|---|---|---|---:|---|

| Base | TBD | TBD | TBD | VERIFY | | | |

| Joint 1 | Motor pinion | 1 | 10T, module 2, 20° pressure angle, beta -32° | REQUIRED | 3D printed | | Part: `Art1GearMotor` |
| Joint 1 | Driven gear | 1 | 50T internal gear, module 2, 20° pressure angle, beta -32° | REQUIRED | 3D printed | | Integrated into `Art1Bot`; 5:1 reduction |

| Joint 2 | TBD | TBD | TBD | VERIFY | | | |

| Joint 3 | TBD | TBD | TBD | VERIFY | | | |

| Joint 4 | TBD | TBD | TBD | VERIFY | | | |

| Joint 5 | TBD | TBD | TBD | VERIFY | | | |

| Joint 6 | TBD | TBD | TBD | VERIFY | | | |

| Gripper | TBD | TBD | TBD | VERIFY | | | |



\## Actuation



| Part | Qty | Specification | Status | Source | Cost | Notes |

|---|---:|---|---|---|---:|---|

| Joint 1 stepper motor | 1 | NEMA 17, approximately 40 mm body length | REQUIRED | TBD | | Identified in `AssemblyBase` CAD |

| Motor drivers | TBD | TBD | VERIFY | | | |

| Belts | TBD | TBD | VERIFY | | | |

| Pulleys | TBD | TBD | VERIFY | | | |



\## Bearings and Shafts



| Part | Qty | Specification | Status | Source | Cost | Notes |

|---|---:|---|---|---|---:|---|

| Joint 1 main bearing | 1 | 16014ZZ | REQUIRED | TBD | | Identified in `AssemblyBase` CAD |

| Shafts / rods | TBD | TBD | VERIFY | | | |



\## Fasteners



| Part | Qty | Specification | Status | Source | Cost | Notes |

|---|---:|---|---|---|---:|---|

| Screws | TBD | TBD | VERIFY | | | |

| Nuts | TBD | TBD | VERIFY | | | |

| Washers | TBD | TBD | VERIFY | | | |



\## Electronics



| Part | Qty | Specification | Status | Source | Cost | Notes |

|---|---:|---|---|---|---:|---|

| Low-level controller | 1 | ESP32 candidate | VERIFY | | | Custom control architecture planned |

| Joint 1 home sensor | 1 | Optical switch / optosensor | VERIFY | TBD | | `AssemblyBase` contains `OptoSwitch002`; exact commercial part not yet verified |

| Power supply | 1 | TBD | VERIFY | | | |

| Emergency stop | 1 | TBD | VERIFY | | | |

| Wiring / connectors | TBD | TBD | VERIFY | | | |



\## Already Owned



| Item | Quantity | Notes |

|---|---:|---|

| 3D printer | 1 | Available |

| PLA filament | TBD | Available |



\## Verified Joint 1 Transmission



Motor pinion:



\- 10 teeth

\- Module 2.00 mm

\- 20° pressure angle

\- Beta -32°

\- 20 mm pitch diameter

\- 12 mm gear height



Driven internal gear:



\- 50 teeth

\- Module 2.00 mm

\- 20° pressure angle

\- Beta -32°

\- 100 mm pitch diameter

\- 15 mm gear height



Calculated transmission ratio:



`50 / 10 = 5:1`



Approximate gear-center offset based on pitch diameters:



`(100 mm - 20 mm) / 2 = 40 mm`



This value should later be checked against the actual motor mounting geometry.



\## Budget



Initial purchase budget: RM500



\### Current Committed Spend



RM0



\### Remaining Initial Budget



RM500

