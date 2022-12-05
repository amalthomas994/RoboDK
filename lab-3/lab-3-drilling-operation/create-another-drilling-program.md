---
description: Create another drilling program on Part2.
---

# Create Another Drilling Program

1. Ensure the robot is at the "Home" target position.
2. Move the robot end effector 230mm to the right relative to the current location.
3. Create a new reference frame and name it "Part2 Reference Frame".
4. Import Part2.sld and make it the child of this reference frame.
5. Move the part somewhere directly right of Part1.
6. Ensure the part is still in the robot tool workspace.
7. Make "Part2 Reference Frame" the current active frame.
8. Create a new target at the current position of the robot and name it "Home 2".
9. Open the Part2.jpg file.
10. Create a program to trace the path shown in the black outline.
11. Start at location (X: 0, Y: 0) and trace the path. You will need to create a circular movement to trace the corners as explained in Lab 2. You will need to find out the intermediary points at the corners.
12. The program needs to start at the "Home 2" target location, trace the path and return to the "Home 2" target location.&#x20;
13. Rename this program to "Trace Part 2"
14. Create another program to drill holes in the part. Reference the Part2.jpg file to find the location of the holes.
15. The program needs to start from "Home 2" and end at the same target. Movements between holes must be linear moves. Drilling movements must be linear as well.
16. Name this program "Drill Part 2"
17. Test the program to make sure all holes are made.

