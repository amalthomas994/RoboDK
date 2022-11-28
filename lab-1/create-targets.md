---
description: Create targets to follow the shape of the cutting sheet.
---

# Create Targets

1. Open the Part.pdf document to view the measurements of the cutting sheet.
2. In RoboDK, ensure that the active reference frame in the robot panel is the "Cutting Sheet Reference Frame" with respect to the robot base.
3. In the station tree, right click on the "Cutting Sheet Reference Frame" and ensure that it is set to "Active Reference Frame". You will see a green sphere in the icon of the reference frame in the station tree if it is set as the active reference frame.
4. Set the coordinates of the TCP to the following in the Robot panel:<img src="../.gitbook/assets/image (12).png" alt="" data-size="line">
5. The tool reference frame will be placed at the starting location of the cutting sheet.
6. Click on the add target icon <img src="../.gitbook/assets/image.png" alt="" data-size="line"> to place a target reference frame at the current position of the end effector TCP.
7. Move the TCP to the next point in the Part.pdf (125.41 mm, -1.00mm).
8. Add another target at this position.
9. Repeat this procedure for all points in the PDF.
