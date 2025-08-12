# 1.9Safety Stop Function

Set an adequate safety stop type for each safety stop function. The safety stop functions, which stop the robot under a safe condition in case of a safety violation, include the following three types. All types of safety stop functions meet the requirements of Clause 4.2.2.4 of IEC 61800-5-2.

* **Stop0**: The power of the motors of all the joint modules will disconnect immediately, and the motors will stop.
* **Stop1**: The power of the motors of all the joint modules will decelerate, and the motors will stop. Then, the power of the motors will be disconnected.
* **Stop2**: The motors of all the joint modules will decelerate, and the safe operating stop (SOS) function will take effect. The power supply status of all the motors will be retained.

The method for setting the safety stop types of the safety functions is as follows:

1\. Select the **\[Configure]** button > **\[4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 4: Safety Stop Function]** menu.

2\. Click the drop-down menu, set the stop type, and click the **\[Apply]** button.

![](<../_assets/image_44.png>)

| **No.** |               **Safety function**               |              **Stop function**             |
| :-----: | :---------------------------------------------: | :----------------------------------------: |
|    1    |                       SOS                       | Default setting value: Stop0 (fixed value) |
|    2    | TCP position violation (safety space violation) |        Default setting value: Stop0        |
|    3    |             Joint position violation            |        Default setting value: Stop0        |
|    4    |               TCP speed violation               |        Default setting value: Stop0        |
|    5    |              Joint speed violation              |        Default setting value: Stop0        |
|    6    |              Joint torque violation             |        Default setting value: Stop0        |
|    7    |               TCP force violation               |        Default setting value: Stop0        |
|    8    |            TCP orientation violation            |        Default setting value: Stop0        |
|    9    |                 Power violation                 |        Default setting value: Stop0        |
|    10   |                Momentum violation               |        Default setting value: Stop0        |
|    11   |               Collision detection               |        Default setting value: Stop0        |
|    12   |                  Emergency stop                 |        Default setting value: Stop0        |
|    13   |             External emergency stop             |        Default setting value: Stop0        |
|    14   |                  Safeguard stop                 | Default setting value: Stop1 (fixed value) |

3\. After checking the parameter values, finish the setting by clicking the **\[X]** button or by clicking the **\<esc>** key of the teach pendant.

{% hint style="warning" %}
**\[Caution]**: You should set an adequate stopping method for each function based on the result of the risk assessment.
{% endhint %}
