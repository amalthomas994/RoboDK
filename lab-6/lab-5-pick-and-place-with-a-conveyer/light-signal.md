---
description: >-
  We will create a light signal which will turn from red to green when the
  scanning process on the object is complete.
---

# Light Signal

1. Import the Light.stl object into the station.
2. Create a new reference called "Light Reference Frame" frame for this object.
3. Make sure the object is nested inside the reference frame in the station tree.
4. Place the light reference frame at X: 0, Y: 0, Z: 1540mm with respect to the "Scan" reference frame.
5. Right click on the Light object and click on options.
6. Click on "More Options" and "Change Colors".
7. Change the color of the object to green.
8. Rename this light object to "Light\_Green"
9. Dupilcate the light object and rename it to "Light\_Red".
10. Change the color of this object to red.
11. Duplicate it once again and rename it "Light\_Off"
12. Change the color of this object to grey.
13. All objects should overlay each other (same exact coordinates).
14. Create a new program called "Light Green"
15. This program will contain a simulation event which will hide the red and off lights and show the green light. Repeat this for a "Light Red" and "Light Off" program.
16. Clicking on each respective program should change the color of the light.
17. Modify programs in the station so that the light is red when the object is in front of the scanner/camera for 2 seconds, then turn it green before the robot runs the "Put\_Bottle\_Out" function. You will need to place the different light subprograms in the appropriate programs. You may need to add pause instructions to pause the light animation.

