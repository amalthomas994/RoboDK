---
description: Follow these instructions to create a new station and load assets.
---

# Create Station

1. Create a new station
2. Create a new World Reference Frame reference frame.
3. Import the **Table.stl** 3D into the station.
4. Create a "Table Workspace Reference Frame".
5. Set the X, Y, Z coordinates of this reference frame to the following: <img src="../.gitbook/assets/image (9).png" alt="" data-size="line">
6. Import the **Fanuc-LR-Mate-200iC.robot** file into RoboDK.
7. Reposition the robot on top of the table by setting the Z coordinate of the Fanuc Base Reference frame to 1098.350 mm.
8. Set the X and Y coordinate of the same frame to X = 450.00 mm, Y = 0.00 mm.
9. Import the **Drill.stl** tool and attach it to the robot. Ensure the tool is the active tool.
10. Fix the orientation of the tool such that the drill bit is vertically opposite to it's current orientation.
11. Adjust the location of the TCP of the drill so that the Z axis of the TCP forward, parallel to the drill bit. Refer to the Drill.pdf document for the measurements of the drill.
12. Create a new reference frame and name it "Part Reference Frame".
13. Import the Part1.stl file into RoboDK and make it the child of the "Part Reference Frame".
14. Move the Part Reference Frame such that it is in the same plane as the Table Workspace Reference Frame.
15. Move Part1 to a location where it is fully reachable by the robot tool. The tool workspace can be visualised by clicking on the "Workspace" -> Show for current tool" option in the robot panel.
16. Point the TCP of the tool downwards (i.e Z axis will face straight down) by changing the joint angle of joint 5 such that the Z axis of the TCP is pointing roughly straight down.
17. Click on the "Align" button on the Joint axis jog control panel so that the Z axis is aligned perfectly vertically downwards.

\






