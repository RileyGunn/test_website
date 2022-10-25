---
layout: default
title: Commissioning HS3
parent: Getting Started Guide
nav_order: 2
permalink: docs/Getting_Started_Guide/Commissioning_HS3
---

# Commissioning HS3
{: .no_toc }

The intention of this section is to provide guidance to those who are opening their new Pantheon HS3 machine for the first time and want to commission the machine.
{: .fs-6 .fw-300 }

If you have not already done so, please read the contents of the [Safety Page]({{ site.baseurl }}{% link docs/Getting Started Guide/Safety.md %}) in its entirety before continuing.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Installation

Caution
{: .label .label-yellow }
Failure to completely follow the instructions in this section may result in operator injury or damage to the machine. Do not begin the installation procedure unless all preparations for installation are taken or completed. Read the entirety of each instruction before beginning the task. Only perform the tasks in the order they are listed.
{: .fw-500 }

## General Machine Requirements
- Allow yourself ample space to unbox and install the machine.
- The machine alone weighs approximately 65 kg and thus requires two people to lift or move.
- The machine should be operated indoors within the nominal temperature range of 10-35℃.
- The machine should be placed on a rigid and level surface.
- The recommended space requirements for the machine are 100 cm by 70 cm with at least 120 cm height to allow for the enclosure lid to open. If placed on a table or work surface, the surface should be able to support 65 kg.
- The machine is powered from a standard 120VAC 15A wall outlet.
- A strong and secured wireless network is recommended.

## Installation Steps

Caution
{: .label .label-yellow }
Use protective gloves when removing the machine from the shipping box.
{: .fw-500 }

1. Open the shipping box with a flathead screwdriver to bend back the tabs at the edges and bottom of the crate.
2. Remove the tape securing the door and lid of the machine.
3. Remove the protective plastic film from the machine
4. Remove the shipping straps securing the machine to the crate base
5. Remove the Wooden braces surrounding the machine base
6. Remove the tape securing the contents of the machine work area and remove them from the machine.
7. Confirm all contents of the machine are accounted for. A list is included in the crate.
    - HS3 Machine
    - 6’ Power Cable
    - Door and lid handles
    - HEPA filter shroud
    - Tools
    - Consumables
8. Inspect for any damage that may have occurred during shipping.

Caution
{: .label .label-yellow }
Two or more people are required to move or lift the machine. Do not attempt to move the machine yourself. Use of a wheeled cart to move significant distances is recommended.
{: .fw-500 }

9. Lift the machine from below the base plate and place it in its intended operation position. 
10. Locate a suitable electrical outlet and ensure the power switch on HS3 is in the OFF position. Plug the machine into mains power using the provided electrical cable.

Notice
{: .label .label-blue }
If the distance from an electrical outlet to the machine is further than the provided cable, either relocate the machine or use an extension cable with at least 16 AWG conductors. Tie the extension cord to the provided cable to ensure the connection won’t come undone accidentally. 
{: .fw-500 }

11. Flip the power switch of HS3 to the ON position. The switch should illuminate. The servo motors of the machine will energize and an audible “clunk” may be heard. This is not a concern.
12. 
13. 
14. 

Caution
{: .label .label-yellow }
Ensure there are no persons or objects within the enclosure of HS3 before performing the next steps. Several pinch and crush points exist on this machine which can cause moderate injury. The axes of HS3 can also move rapidly and in unexpected directions which can cause moderate injury. 
{: .fw-500 }

15. Ensure there are no objects or persons within the enclosure of HS3 before proceeding. If the sheet metal print surface has been removed or is mis-aligned, place it on the PCB heatbed using the alignment pins. Close the lid and door of the enclosure.
16. Click the “HOME ALL” button in the “Machine Movement” panel. HS3 will perform a homing routine for each axis. At the end of the homing routine in the “Status” panel under “Tool Position” the value for X and Y should be 0.0, and the value for Z should be 15.0.

The axes of HS3 are now homes and the warning message show before should be gone.

Caution
{: .label .label-yellow }
Certain components of HS3 can reach temperatures from 60℃ - 350℃ and can cause severe burns if the proper precautions are not taken.
{: .fw-500 }

17. Under the “Tools + Extra” panel, set the temperature for the Extruder (Heater 1) to 60℃ using the drop-down menu or by typing it in, and click on “Heater 1” to activate the heater. Heater 1 should now be active at heating up.
18. Confirm that the extruder is heating up by the feedback value under “Current” in the same panel, or by looking at the Temperature Chart. The cooling fan for the extruder motor should also turn on around 45℃. Confirm that the fan is on.
19. Under “Fan Control”, select “PART FAN” and drag the slider to 100% and confirm that the part cooling fans are on and operational. Return the slider to 0.
20. Click on “Heater 1” twice to go from “active” to “standby” to “off”.
21. Set the temperature for the Bed (Heater 0) to 60℃ using the drop-down menu or by typing it in, and click on “Heater 0” to activate the heater. The Bed should now be active and heating up.
22. Confirm the bed is heating up by the feedback value under “Current” in the same panel, or by looking at the temperature chart. There is also a light on the Bed in the top left corner to signify if the bed is powered or not.
23. Click on “Heater 2” twice to go from “active” to “standby” to “off”.

Caution
{: .label .label-yellow }
The following steps require the sheet metal print surface to be installed. Ensure there are no objects or persons in the machine or on the print surface. To perform the bed mesh compensation macro, HS3 will move rapidly in a grid pattern to measure the flatness of the print surface.
{: .fw-500 }

24. In the drop down menu labeled “Compensation and Calibration” in the “Machine Movement” panel, select the “True Bed Levelling (G32)” option. HS3 will measure the height of the print surface in a grid pattern.
25. Navigate to the “Height Map” tab to view the measured grid. An expected height map should be a flat plane with no tall hills or deep valleys. The height map may be tilted compared to the X-Y plane or well above or below the plane. This is acceptable as long as the measured height map is a flat plane. The images below show an acceptable and an unacceptable height map. If the height map exhibits unacceptable characteristics like those shown in the image below, lower the Z-axis to remove the bed, wipe the surface of the PCB bed as well as both surfaces of the metal print surface. Replace the bed into the machine and return to step 23. Even the smallest amount of debris can interfere with the bed mesh compensation. 

Caution
{: .label .label-yellow }
Certain components of HS3 can reach temperatures from 60℃ - 350℃ and can cause severe burns if the proper precautions are not taken.
{: .fw-500 }

26. Return to the “Dashboard” tab and in the “Macros” panel, click on the “Park Head for Cleaning” macro. This will move the machine to a suitable location for cleaning or loading filament.
27. To load filament into the extruder, set the temperature of “Heater 1” to 255℃ and set it to active. Wait for the temperature to stabilize at 255℃.
28. Once the temperature has stabilized, feed filament into the filament port until it is visible at the extruder inlet. Open the lid of the enclosure and feed the filament into the extruder by pressing back the lever and pushing filament into the top of the extruder. Push filament into the extruder until bottomed or until molten plastic is extruded from the nozzle. Release the lever. If the filament bottomed within the extruder, make sure the extruder has a firm grip of the filament by giving the filament a tug in the upwards direction. If you are able to pull it out, then you need to feed the filament further into the extruder.
29. Using provided or equivalent lint-free wipes, wipe any filament from the nozzle.
30. Remove the sheet metal print surface and clean with isopropyl alcohol. Once the print surface is clean, apply the release agent to the entire surface. Replace the print surface onto the heated bed using the alignment pins. The printer should now be ready to start its first print. Be sure that there is no debris under the print surface.
31. Navigate to the “Jobs” tab in the Web Control Interface and start the “XYZ_Calibration_Cube” job. HS3 will begin to heat up the bed and extruder. Once the heaters stabilize at the set temperatures HS3 will perform a homing routine, another bed mesh compensation, and pressurize the nozzle before starting the print.
32. Once the print is complete, wait for the bed and part to cool to below 40℃ before removing the print surface. Flex the print surface to release the part.

Congratulations, your HS3 is now ready to print 1000’s of parts for you!
{: .fs-6 .fw-300 }

For further details on how to use the Pantheon HS3 Additive Manufacturing System to its full potential, please refer to the User Manual.

[HS3 User Manual](In-Depth_Guide/HS3_User_Manual){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }



