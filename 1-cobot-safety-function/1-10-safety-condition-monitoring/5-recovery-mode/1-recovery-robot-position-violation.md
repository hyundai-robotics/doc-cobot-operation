# 1.10.5.1 Recovery in case of robot position violations

Robot position violations are situations in which the robot’s position exceeds a safety space, and these include TCP position, TCP orientation, and joint monitoring violations. When a robot position violation occurs, you can only clear the error by moving the robot’s physical position.

1.  On the safety condition monitoring window, click the \[Status Recovery] button to enter recovery mode.


2.  Turn on the motor by using the enabling switch on the teach pendant.


3.  Use the teaching device to move the robot back to a safety space.


4.  On the safety condition monitoring window, check if the status of each space is displayed as SAFE.


5. After the recovery is completed, click the \[Status Recovery] button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**: After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}
