# 1.10.5.3 Recovery in case of robot force violations

Robot force violations are situations in which external force is applied on the robot or in which the amount of the force used by the robot internally exceeds a safety limit, and these include TCP force, collision detection, joint torque, power, and momentum monitoring violations. You can clear errors depending on the causes of the violations.

#### <mark style="color:green;">Violation caused by external force applied on the robot</mark>&#xD;

1. Remove the external factor that is applying force on the robot.
2. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
3. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
4. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**: After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}

#### &#xD;<mark style="color:green;">Violation caused by the amount of force used by the robot internally exceeding a safety limit</mark>&#xD;

1. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
2. &#x20;**** Turn on the motor using the enabling switch on the teach pendant.
3. Use the teaching device to move the robot to a low-load posture.
4. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
5. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the recovery mode, recheck the robot’s safety condition setting, tool data, the teaching position of the operating program, and the torque sensor offset.
* If the error is not cleared, check the tool data, tool number, safety condition setting, and torque sensor offset, and repeat procedures 1 through 5.
{% endhint %}
