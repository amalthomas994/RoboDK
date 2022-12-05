---
description: Create targets to drill holes in Part1.
---

# Create Targets

1. Open the Part1.pdf document to view the measurements of the cutting sheet.
2. In RoboDK, ensure that the active reference frame in the robot panel is the "Part Reference Frame" with respect to the robot base.
3. In the station tree, right click on the "Part Reference Frame" and ensure that it is set to "Active Reference Frame".
4. Create a new target at the current location of the robot. Rename this target as "Home".
5. The height of Part1 is 25mm. Set a new target above the first hole of Part1. (X: 25mm, Y: 25mm, Z: 25mm)
6. Create a new target here. Rename the target to "Above Hole 1"
7. Create a new target at (X: 25mm, Y: 25mm, Z: 0mm) so that the robot can drill a hole at this location. Rename it to "Drill Hole 1".
8. Create another target at the top of hole 2. Rename it to "Above Hole 2"
9. Create a target so that the robot drills through hole 2. Rename it to "Drill Hole 2"
10. Repeat this procedure for all the holes.

