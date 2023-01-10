# Pick and Place Bottles

1. Create a simulation event in the Pick\_Bottle program to attach a bottle to the closed gripper of the robot. Ensure the closed gripper is the active tool.
2. Create a simulation event in the Drop\_Bottle program to detach a bottle from the closed gripper of the robot. Ensure the closed gripper is the active tool. Ensure the "Attach to Parent" is set to the "Conveyer Object Out".
3. Create a new "Replace\_Object" program which runs a simulation event which runs a "Set object position (relative)" action on all the objects in the scene. This program will reset all the objects in the scene when needed. Select all objects from the "Scan" object to the last bottle object.
4. Fill in the "Get\_Bottle\_In" program. Ensure the "Conveyer In Base" is the Active Reference Frame. The program should go to the "App\_Pick" target and then perform a linear motion to the "Pick" target and then run the Pick\_Bottle program to attach the bottle. It should then run a linear motion to the "Retract\_Pick" target.
5. Fill in the "Put\_Bottle\_Out" program to place the bottle on the other conveyer. The program must call the "App\_Drop", "Drop", and "Retract\_Drop" targets and detatch the bottle on the Conveyor Our Base reference frame.
