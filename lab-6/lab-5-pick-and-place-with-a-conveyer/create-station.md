# Create Station

1. Open the PickandScan.rdk file in RoboDK.
2. You will see a UR10e robot on a base with two conveyers and bottles on the conveyers. You will also notice a camera facing the robot.
3. Your task is to create a program which will pick a bottle from the left conveyer and scan it with the camera and then place that bottle on the other conveyer. When a bottle is picked and placed, the conveyers will move to bring in the next bottle.
4. Start by creating the GoHome program.
5. The Home target can be found in the World reference frame in the station tree. Create a joint movement to the home target.
6. Next, create the scan program.
7. Create a joint move to the scan target.
8. Ensure the Scan reference frame is the active reference frame.

