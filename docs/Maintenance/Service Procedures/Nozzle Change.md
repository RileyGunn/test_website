---
layout: default
title: Nozzle Change
parent: Service Procedures
grand_parent: Maintenance
nav_order: 1
---

# Nozzle Change
{: .no_toc }

Changing the nozzle is the most common maintenance task. It is required when a nozzle becomes irreparably clogged, damaged from crashing or worn through extended use.
{: .fs-6 .fw-300 }

Find detailed instructions on how to perform a nozzle change on the HS3. Jump to the relevant section depending on the printhead on your HS3.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Pantheon HSD Contact Printhead



## E3D Hemera Extruder Printhead

### Tools
- 7mm socket wrench or nut driver
- Nozzle torque wrench
- Adjustable wrench
- 2mm and 2.5mm allen keys

### Procedure

1. Check temperature of hotend on web interface, ensure the hotend is safe to touch (less than 60°C)
2. Lower the bed to a safe height (approx Z200)
3. Move printhead to the front edge of the printer (approx Y150 X280)
4. Unplug the radial part cooling fans from the print head PCB, they are locking connectors, be sure to release the catch while pulling the connector out. (See below)
5. Remove the part cooling fan and duct by removing the two M3 screws holding it in place with a 2.5mm allen key, and sliding it down and off. (below)
6. Remove the guard plate using the 2mm allen key to remove the 2 M3 flathead screws holding it in place. Be sure not to lose the washers sandwiched between the heat block and the guard plate
7. Heat the nozzle to 260-270°C
8. Hold onto the hotend using the wrench, and remove the nozzle using the 7mm socket

Notice
{: .label .label-blue }
A thermal runaway or heater fault error may occur during this step, it is caused by the wrench rapidly cooling the hot end. If this happens, reset the heater using the gcode console and continue. The gcode to reset it is M562 P0

9. Screw in the nozzle until just seated with the 7mm wrench and allow nozzle temperature to stabilize
10. Using the wrench to hold the hotend in place, torque the nozzle to 3N-m with the supplied nozzle torque wrench. 
11. Cool down the nozzle and install remaining components in reverse order of removal. Part cooling fans may be connected to the print head breakout board in any order.