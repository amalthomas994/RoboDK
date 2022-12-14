# Create Pick and Place Program

1. Delete the Detach and Attach object programs.
2. Make the box object a child of Box Reference Frame A again.
3. Change the location of the box so that the reference frame is to the bottom right of the box.
4. Make the table workspace reference frame the active reference frame.
5. Move the robot to it's home position by clicking on "Home" on the joint axis jog.
6. Create a target here and call it "Home".
7. Create a new program and rename it "Go Home".
8. Create a joint move to the "Home" target.
9. Change the active reference frame to "Box Reference Frame A"
10. Ensure the robot end effector is facing vertically down.
11. Right click on the box object and select get with robot.
12. The gripper should be perfectly around the box now.
13. Move the gripper vertically upward by 200mm.
14. Create a new target here and rename it to "ApproachA".
15. Move the gripper vertically downwards such that the Z coordinate of the TCP is 90 mm with respect to Box Reference Frame A.
16. Create a new target here and call it "PickA".
17. Create a new program and call it "PickA Program".
18. Click on the ApproachA target and create a joint move to it.
19. Then create a linear move to the PickA target.
20. Create an attach object simulation event. This will create a simulation event inside the PickA Program.
21. Create a linear move back up to the ApproachA target.
22. Make Box Reference Frame B the active reference frame.
23. Create a target called "ApproachB" directly above the reference frame.
24. Create a target called "PickB" such that the box is placed exactly in a location where the Box Reference Frame B is to the bottom right of the box.
25. Create a new program and name it "PlaceB Program".
26. Create a program similar to the PickA program but this time detach the box object to the "Box Reference Frame B" reference frame.
27. Duplicate (CTRL+C, CTRL+V) the PickA and PlaceB programs and rename the new programs to PickB Program and PlaceA Program respectively.
28. Change the reference frame of the PickB program to "Box Reference Frame B" by expanding the program in the station tree, right clicking on "Set Ref", selecting "Set Reference Link" and choosing the Frame B reference.
29. In the PickB Program, right click on the MoveJ (ApproacA) move and change the target linked to "ApproachB". Change the target link for "MoveL (PickA)" to PickB. Move the last linear motion in this program to link to target "ApproachB".
30. Reverse the above steps for the PlaceA program and change all the targets to Frame A targets.
31. Right click on the Detach event of the PlaceA and click modify. Change the "Attach to parent:"  reference frame to "Box Reference Frame A"
32. Combine the programs by creating a new program and calling it "Main".
33. Open the program call instruction dialog and call the programs in the following order:
    1. Go Home
    2. PickA Program
    3. PlaceB Program
    4. PickB Program
    5. PlaceA Program
    6. Go Home
34. Double click the main program to run it.
35. The robot should go from its home location to pick the object from the A position and drop it off in the B position, then pick it from the B position and drop it off in the A position and then return home.
