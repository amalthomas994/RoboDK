---
description: Follow these instructions to create a new station and load assets.
---

# Create Station

1. Create a new station
2. Create a new World Reference Frame reference frame.
3. Import the **Table.stl** 3D into the station.
4. Create a "Table Workspace Reference Frame".
5. Set the X, Y, Z coordinates of this reference frame to the following: <img src="../../.gitbook/assets/image (9).png" alt="" data-size="line">
6. Import the **KUKA-KR-6-R900-sixx.robot** file into RoboDK.
7. Reposition the robot on top of the table by setting the Z coordinate of the Fanuc Base Reference frame to 778.5 mm.
8. Set the X and Y coordinate of the same frame to X = 600.00 mm, Y = 0.00 mm.
9. Import the **RobotiQ-2F-85-Gripper.tool** tool and attach it to the robot. Ensure the tool is the active tool.
10. Create a new reference frame and name it "Box Reference Frame A".
11. Import the box.sld file into RoboDK and make it the child of the "Box Reference Frame A".
12. Adjust the location of the box with respect to the "Box Reference Frame A" by double clicking on the box object in the station tree and adjusting the object position with respect to the correct reference frame. The box dimensions are (100mm x 100mm x 100mm). The "Box Reference Frame A" should be at the bottom corner of the box object.
13. Move the Box Reference Frame such that it is in the same plane as the Table Workspace Reference Frame.
14. Move the box to a location where it is fully reachable by the robot tool. The tool workspace can be visualised by clicking on the "Workspace" -> Show for current tool" option in the robot panel.
15. Point the TCP of the tool downwards (i.e Z axis will face straight down) by changing the joint angles of the robot and aligning it vertically downwards.

\






