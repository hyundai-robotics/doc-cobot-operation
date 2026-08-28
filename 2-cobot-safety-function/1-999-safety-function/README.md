# 1.3 Safety functions

The purpose of the safety functions of the collaborative robot is to reduce the impact on the operator in the case of a collision between the operator and the robot during collaborative operation.

The safety functions include the “axis limiting function,” which restricts the motion of the robot’s joints, and the “robot limiting function,” which restricts the robot’s motion in the safety space. These functions can be configured in the setting menu and are used as measures to respond to the risks selected in the risk assessment performed by the operator.

In executing the safety functions, the following items should be configured:

*   **Safety space**: Set the working space and the protected space to restrict the robot’s motion.


*   **Tool modeling**: This is used to check whether the robot’s tool position intrudes or exceeds specific spaces.


*   **Robot modeling**: This is used to check whether the robot’s elbow position intrudes or exceeds specific spaces.


* **Safety limiting conditions**: Set monitoring criteria value for the safety functions.

One safety condition can be configured for each safety space; if not configured, Level1 (default setting mode) will be set as the default condition. You can add up to 5 limiting conditions, 16 tools, and 12 safety spaces. You can set, modify, or enable the parameters relating to the safety function only when the motors are turned off in the manual mode.
