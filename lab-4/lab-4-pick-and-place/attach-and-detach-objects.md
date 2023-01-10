# Attach and Detach Objects

1. Click on the "Simulation Event Instruction" ![](<../../.gitbook/assets/image (1) (2).png>) button to open the "Event Instruction" dialog.
2. Select "Attach object" as the action and ensure that the "RobotiQ 2f-85 Gripper" is the selected tool (TCP).
3. Leave the "measure distance as:" option to "Default".
4. Click OK.
5. This will create a simulation event to a new program in the station tree called "Attact to RobotiQ 2F-85 Gripper". Rename the program (not the simulation event) to "Attach Object".
6. Create a new reference frame and call it "Box Reference Frame B". Place it 600mm to the left of "Box Reference Frame A"
7. Move the robot so that the end effector is roughly around the box object.
8. Double click on the "Attach Object" program to attach the box to the robot. This will simulate the robot picking and holding the box object. In the station tree, you will notice that the box object is now a child of the gripper object. _Note: RoboDK will not animate the gripper closing and holding the object._
9. If you move the robot around, you will notice that the box will be attached to it.
10. Move the robot to a location close to the "Box Reference Frame B" such that the reference frame is at the right corner of the box.
11. Create a new program and rename it "Detach Object"
12. Select the program in the station tree and click on the simulation event instruction tool.
13. Select the action as "Detach object" and ensure the correct gripper is still selected.
14. In the "Attach to parent" dropdown, select the "Box Reference Frame B" reference frame.
15. Click OK.
16. Run the program.
17. You will notice that the box object is now a child to the "Box Reference Frame B" reference frame.&#x20;
18. If you move the arm around again, the box will not be attached to it anymore.
19. A trick to place the gripper perfectly around the box is to right click on the box object in the 3D scene and click on "Get with Robot" and select the KUKA robot. This will move the robot end effector directly around the target object.
20. You can not run the attach program to move the box around with the robot again.
