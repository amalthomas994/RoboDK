# Wrist Singularity

Open the **Singularities.rdk** file in RoboDK.

1. Wrist singularities happen when Joint 4 and Joint 6 are aligned. Most of the time when this happens Joint 5 = 0.
2. When Joint 4 and Joint 6 are aligned, there are an infinite number of solutions to get to a given coordinate.
3. Run the **Kuka\_Wrist\_Singularity** program.
4. You will see that RoboDK complains about Joint 5 being too close to a singularity.
5. Open the Kuka's robot panel and pay attentiion to the joint angles.
6. Run the program again and notice that when the robot reaches singularity, Joint 4 and Joint 6 have the same angle of 89.94, and thus Joint 5 approaches 0.
7. Find 2 new targets approximately similar to the first program such that singularity can be avoided. Fill in the "Kuka\_No\_Wrist\_Singularity" program with a linear movement between these two new targets.
8. Ensure the Weld gun tool is visible and make it the active tool. Run the **Kuka\_Wrist\_Singularity\_Infinit** program to visualize the infinite solutions possible when a wrist sigularity occurs. Notice that the end effector coordinate remains the same as the wrist rotates. In the robot panel, you will also notice that the Joint 4 and Joint 6 angles are equivalent, as well as Joint 5 = 0.
9. Repeat the same procedure for the UR5e robot and create a program to solve the wrist singularity.

