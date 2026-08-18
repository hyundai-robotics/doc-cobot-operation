# 1.10.5.4 Recovery in cases of safe operating stop (SOS) violations

SOS violations are situations in which the robot’s motion is detected while its motor is on and is supposed to be in a stop state. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1. Remove the external factor that is applying force on the robot.
2. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
3. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
4. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the recovery mode, turn on the motor in the automatic mode and check if the error does not persist.
* If the same error recurs, check the driving module of the pertaining axis.
{% endhint %}
