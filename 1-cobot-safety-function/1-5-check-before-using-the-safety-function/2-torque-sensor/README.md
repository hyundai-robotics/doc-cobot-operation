# 1.5.2 Checking the torque sensor

You must set torque sensor offsets because the diagnosis of force/power, among the safety functions of the collaborative robot, is conducted based on the torque sensors attached to the axes. Although torque sensor offsets were set before the robot is delivered, you should set the torque sensor offsets if the current offset values are not correct.

1\. **** After recording and modifying the step positions, run the program, and move the robot axes to a position that does not allow them to be affected by gravity (**0, 90 -90, 90, 0, 0** \[deg]).

*   The position unaffected by gravity varies depending on installation angles.

    The position unaffected by gravity is (**0, 90, -90, 90, 0, 0** \[deg]) if the robot is installed flat on the ground. Modify the angle of axis 1 if the installation angle is sloped so that the lower frame matches the direction of the slope.

![Figure 1 Robot position when installed flat on the ground (0, 90, -90, 90, 0, 0 \[deg\])](../../../_assets/image.png)

![Figure 2 Robot position when it is wall-mounted (90, 90, -90, 90, 0, 0 \[deg\])](<../../../_assets/image_1.png>)

* In recovery mode, move each axis with the jog if a stop occurs because of a safety function violation. For more details on recovery mode, see “[**1.10.5 Recovery mode**.](../../1-10-safety-condition-monitoring/5-recovery-mode/)”

{% hint style="info" %}
For more details on step position recording and modification, see “[**2.3.2 Step position recording and modification**](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/2-operation/2-3-step/step-pose-modify)” of the “[**Operation Manual for Hi6 Controllers**.](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/)”
{% endhint %}

**2.** In the **\[Joint limit]** tab of **\[Set up > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 1: Safety condition**] menu, check the current value of the joint torque limit.

![](<../../../_assets/image_50.png>)

3\. Close the menu if the current torque sensor data value is smaller than 1 in the absolute value. Otherwise, carry out torque sensor offset if it is larger than 1.
