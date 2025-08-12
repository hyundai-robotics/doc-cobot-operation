# 1.10.5.2 Recovery in case of robot speed violations

Robot speed violations are situations in which the robot’s speed exceeds a safety limit, and these include TCP speed, joint speed, power, and momentum monitoring violations. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1.  &#x20;**** On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.


2.  On the safety condition monitoring window, check if the status of each space is displayed as SAFE.


3. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the error, make sure to recheck all speed-related safety parameters and the speed displayed on the operating program.
* After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}
