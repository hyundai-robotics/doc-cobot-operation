# 1.3.1 Robot limit functions

The robot limiting functions, which restrict the robot’s motion in the safety space, include the following:

*   **TCP position**: This restricts the tool or the elbow shapes of the robot modeled in spheres from intruding or exceeding a set space.

    ****
*   **TCP orientation**: This restricts the orientation of the robot’s end effector and the tool from deviating from a set orientation.

    ****
*   **TCP speed**: This restricts the robot’s speed to a low speed so that the operator can escape in case of a collision with the robot (the robot moves at a maximum speed of 250 mm/s in the manual mode and the direct teaching mode).

    ****
*   **TCP force, power, and collision detection**: This limits the force and pressure in case of a collision between the robot and the operator.

    ****
* **Momentum**: This limits the energy and impact load in case of a collision between the robot and the operator.
