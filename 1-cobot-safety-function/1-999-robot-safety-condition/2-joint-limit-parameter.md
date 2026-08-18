# 1.6.2 Joint limiting parameters

These parameters are the limit values for monitoring the safety functions relating to the space in which the robot’s joints move. If a joint limiting parameter is enabled in a Cartesian space, monitoring will be done at all times, and if the deceleration mode is enabled, monitoring will be done based on Condition0. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[Joint limit]** tab of the **\[Set up > 4: Application parameter > 21: Cobot setup > 1: Cobot Safety Function > 1: Safety condition]** menu.

![Figure 4 An example of joint limiting setting (S-axis)](<../../_assets/image_20.png>)

![Figure 5 Window for setting joint limiting parameters](<../../_assets/image_27.png>)

|    **Parameter**   | 　　　　　　　　**Description**                                              |              **Default setting value**             |
| :----------------: | -------------------------------------------------------------------- | :------------------------------------------------: |
|  Joint angle limit | <p>The angle limit value of a joint </p><p>(-360.0°–360.0°)</p>      |       It is identical to a robot soft limit.       |
|  Joint speed limit | <p>The angular speed limit value of a joint </p><p>(1.0°–500.0°)</p> |  It is identical to the highest speed of the axis. |
| Joint torque limit | <p>The torque limit value of a joint </p><p>(-500.0–500.0 Nm)</p>    | It is identical to the highest torque of the axis. |

{% hint style="warning" %}
**\[Caution]**: In configuring a speed limit, you must consider the STOP reaction time and put a cover on the target to prevent collisions and injuries.
{% endhint %}
