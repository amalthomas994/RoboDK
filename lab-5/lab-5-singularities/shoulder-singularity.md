# Shoulder Singularity

1. Shoulder Singularities occur when the center of the robot's wrist aligns with the axis of joint 1.
2. Hide the Weld gun tool and make the flange the active tool.
3. Make the **Shoulder\_Singularity\_Plane** object under the Kuka robot visible in the station tree.
4. Run the **Kuka\_Shoulder\_Singularity** program and notice the error produced by RoboDK.
5. You will notice that the wrist is centered on the blue plane which is aligned with the Z axis of Joint 1.
6. There are an infinite amount of solutions for the robot to reach the coordinate.
7. In order to visualize the infinite amount of solutions, run the **Kuka\_Shoulder\_Singularity\_Infinit** program.
8. Notice that the robot can spin in a cylindrical area and the end effector stays put on the same coordinate.
9. Find 2 new targets approximately similar to the **Kuka\_Shoulder\_Singularity** program such that singularity can be avoided. Fill in the "Kuka\_No\_Shoulder\_Singularity" program with a linear movement between these two new targets.
10. You will notice that the shoulder of the robot spins at very high speeds in order to pass the singularity point.
11. Repeat the same procedure for the UR5e robot and create a program to solve the shoulder singularity.
