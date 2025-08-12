# 1.5.2.1 Torque sensor offset

1\. **** After recording and modifying the step positions, run the program, and move the robot axes to a position that does not allow them to be affected by gravity.

In recovery mode, move each axis with the jog if a stop occurs because of a safety function violation. For more details on recovery mode, see “[**1.10.5 Recovery mode**.](../../1-10-safety-condition-monitoring/5-recovery-mode/)”

{% hint style="info" %}
For more details on step position recording and modification, see “[**2.3.2 Step position recording and modification**](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/2-operation/2-3-step/step-pose-modify)” of the “[**Operation Manual for Hi6 Controllers**.](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/)”
{% endhint %}

2\. **** Click the **\[Favorites]** button on the bottom right part of the Hi6 teach pendant window, enter “**314”** in the input box of the favorites window, and click the **\[OK]** button.

![](<../../../_assets/image_48.png>)

{% hint style="warning" %}
**\[Caution]**

* In Engineer Mode, the engineer mode icon (![](../../../_assets/engineer.png)) will blink on the status bar.
* Be careful as a wrong setting in Engineer Mode may lead to a severe problem in the robot system.
{% endhint %}

3\. Click the **\[Set up]** button > **\[3: Robot parameter > 8: Torque sensor offset]** menu.

4\. Check the position of each axis, click the **\[Reset one]** or **\[Reset all]** button, and observe whether the torque sensor offset value has been changed.

![](<../../../_assets/image_14.png>)

* To set the torque sensor offset of an axis, click the \[Reset one] button.
* To set the torque sensor offsets of all the axes, click the \[Reset all] button.

5\. Check if the corrected torque sensor data value is close to 0, and save it by clicking the **\[OK]** button.

6\. Reboot the system.
