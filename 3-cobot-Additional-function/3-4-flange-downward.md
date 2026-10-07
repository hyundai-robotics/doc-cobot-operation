# 3.4 Flange Downward Orientation

<mark style="color:green;">This function is available only for the HDC50-17.</mark><br>
For the HDC50-17, the angle between the flange Z-axis and the vertical direction of the ground must be maintained within 15°. 
If the angle exceeds 15°, the robot will stop.

![](../_assets/Flange_angle_HDC50.png) 

If the robot stops because the angle exceeds 15°, jogging may be restricted.
In this case, operate the robot according to the procedure below to bring the angle between the flange Z-axis and the vertical direction of the ground within 15°.

- In engineer mode, select the `[F2: system] - 3: Robot Parameter - 3: Soft Limit` menu.
- Turn the motor on and jog the robot until the angle between the flange Z-axis and the vertical direction of the ground is within 15°.

{% hint style="warning" %}
**\[Warning]**
* After entering the `Soft Limit` menu, ensure that the angle between the flange Z-axis and the vertical direction of the ground does not exceed 15°.
{% endhint %}