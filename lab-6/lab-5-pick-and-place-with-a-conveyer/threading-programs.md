---
description: You will run programs in a thread to reduce simulation time.
---

# Threading Programs

1. When the **PickAndPlace** program is called, you will notice a pause where the robot is sitting still while the conveyor moves after the robot has picked a bottle.&#x20;
2. This pause is due to the structure of the program call. Each program in the PickAndScan program gets executed in a linear fashion. Subsequent programs will only be excecuted onces the previous program is complete.
3. The "Call NextPart\_In" program only gets executed once the "Call Get\_Bottle\_In" program finishes it's execution. While the "NextPart\_In" program is running, the robot is wasting time waiting for the conveyor to move.
4. To mitigate this, we can run the "NextPart\_In" subprogram in a separate thread so that it will run in parallel with the "Call Scan" program.
5. To do this, right click on the "Call NextPart\_In" program and click modify.
6. You will notice that "Program Call" is selected in the drop down menu.
7. Change this to "Start Thread"
8. If you run the main program now, you will notice that the Scan program and the conveyor move program executes at the same time, thus making the process more efficient.
9. Follow the same procedure for the "NextPart\_Out" program in the **PickAndScan** program.
