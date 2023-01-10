# Pick and Scan

1. Fill in the **PickAndScan** program. The program should first move the robot to the home position, then get the bottle, scan it and then place it on the second conveyor.&#x20;
2. Fill in the **Init** program which will call the Replace\_Object program and calls GoHome after. The Init program will also call the **InitConvPosition** python program under the "Conveyors Programs" folder. You can call this program by following the same procedure as calling regular programs. Reorder the programs such that the **InitConvPosition** program gets called first.
3. In order to move the conveyor belt after a bottle has been picked, we can run the "NextPart\_In" python program. You can view the contents of this program by right clicking on it and selecting  "Edit Python Script". Python programming in RoboDK will not be covered in the labs. However, you can reference RoboDK documentation to understand how it works.
4. In the **PickAndScan** program, add the NextPart\_In program after the Get\_Bottle\_In program call so that the conveyor moves after the first bottle is picked.
5. Add the NextPart\_Out program after the Put\_Bottle\_Out program call in the PickAndScan program to move the other conveyor once a bottle has been placed.
