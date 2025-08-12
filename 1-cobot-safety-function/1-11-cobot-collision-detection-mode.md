# 1.11 Collaborative robot collision detection mode

The collision detection function is a safety mechanism for situations in which the robot operates in an abnormal condition or malfunctions. You can adjust the level of reaction to collisions by setting the detection mode and sensitivity.

1.  Set the operating mode to the manual mode.


2.  Select the **\[Configure]** button > **\[4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 6: (Main) Cobot Collision Detection Mode]** menu.


3. Set whether to use the collaborative robot’s collision detection function, configure the options, and click the **\[OK]** button.

![](<../_assets/image_28.png>)

* **\[Collision detection]**: Set whether to use the collision detection function.
* **\[Detection mode]**: Select the detection mode for collision detection.
* **\[Sensitivity]**: Set the sensitivity for collision detection. The larger the value, the higher the sensitivity to impacts.

{% hint style="warning" %}
**\[Caution]**

* False detection of collision may occur if the difference between the tool data and the actual value is large. In addition, make sure to check the installation angle and gravity direction of the robot. Then, check the encoder and torque sensor if false detection occurs after the correct setting of the tool data.
* Setting the sensitivity value of collision detection at an overlarge value may lead to false detection. Therefore, set it at a proper value suitable for ensuring worker safety.
{% endhint %}
