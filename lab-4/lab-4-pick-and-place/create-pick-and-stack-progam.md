# Create Pick and Stack Progam

1. Delete the existing programs and reference frames.
2. Import 2 more box objects to the scene so that there are 3 boxes in total.
3. Create a reference frame for each box and make sure the reference frames are at the bottom corner of the box object.
4. Place them in different locations on the table.
5. Using what you have learned, create a program to stack these three boxes on top of each other at a target location of your choosing.
6. The final main program should start from the home position, pick and place each box at the target location with the last picked box directly on top of the second box which will be directly on top of the first box. The robot should return to it's home position once the pick and place tasks are complete. Ensure the robot does not collide with the stacked boxes. You can create as many approach targets as you like.
7. In order to save the initial positions of the boxes so that you do not have to reinput the original positions of the boxes everytime the simualtion needs to be run, follow the below steps:
   1. Initialize the boxes in its original positions as chlidren of the appropriate parent frame.
   2. Create a new program and rename it to "Reset Positions".
   3. Click on the simulation event instruction button.
   4. Select "Set object position (relative)" for the action.
   5. Select the table and all three boxes in the right menu.
   6. Click OK.
   7. Double clicking on the "Reset Position" program will reinitialize the location of the boxes if it has been moved.
