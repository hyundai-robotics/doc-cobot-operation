# 1.1 Description of terms

### <mark style="color:green;"> Collision detection </mark>&#xD;

If an external impact exceeding the set threshold is applied while the robot is in operation, it stops to ensure user safety.

*   **Threshold**

    The reference value used to determine whether an external impact has occurred.

### <mark style="color:green;"> Direct teaching </mark>&#xD;

This is a teaching method in which an operator manually moves the robot to a desired path and pose.

*   **Constrained Motion**

    A feature of collaborative robot direct teaching where movement is restricted to specific directions or axes within the Cartesian coordinate system during the teaching process.

*   **Cockpit**

    Buttons used to operate the collaborative robot without relying on a UI.

*   **Cartesian**

    Refers to the Cartesian coordinate system (rectangular coordinate system); a method of expressing the robot's position and movement based on X, Y, and Z coordinates.

*   **Enable Switch**

    Refers to an enabling switch. It serves as a safety switch when operating the robot via a teach pendant in manual mode.
    Positions 1 and 3: Robot operation stops. In the case of Position 3, the switch returns directly to Position 1 without passing through Position 2.
    Position 2: Robot operation is enabled.

### <mark style="color:green;"> Mastering </mark>&#xD;

It refers to the process of aligning the robot's actual joint angles with the joint angles perceived by the controller.