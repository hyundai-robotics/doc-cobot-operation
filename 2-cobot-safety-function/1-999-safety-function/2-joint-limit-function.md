# 1.3.2 Joint limit functions

The joint limiting functions, which restrict the robot’s motion in the joint space, include the following:

* **Joint position**: This limits the robot’s joint positions so that its axes can move only within the specified ranges.
* **Joint speed**: This limits the robot’s momentum so that its axes cannot move beyond the specified speeds.
* **Joint torque**: This limits the robot’s power and force by restricting the torques of the axes to reduce the force and pressure applied on the operator in case of a collision with the robot.

{% hint style="warning" %}
**\[Caution]** : To ensure the safety of personnel and equipment around the robot, operators and users should perform a risk assessment before configuring the robot’s safety function and set the following details according to the assessment result:

* Set passwords and the like so that the safety configuration cannot be modified by unauthorized persons.
* Set safety-related functions and interfaces.
* Check if the settings are correct before running the robot.
* Check if all the safety functions are configured and if the settings conform to the result of the risk assessment.
{% endhint %}

