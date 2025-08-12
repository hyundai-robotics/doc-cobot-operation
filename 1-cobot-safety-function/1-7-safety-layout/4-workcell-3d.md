# 1.7.4WorkCell 3D

This directly monitors the parameters specified in the safety layout by using WorkCell 3D. WorkCell 3D can 3D visualize the safety spaces, tool models, and robot models specified in the safety layout so that the operator can view the settings. In addition, the robot’s position is identified in real time so that the operator can check whether the robot violates any safety spaces.

You can enable the WorkCell 3D function on the panel selection window of the operation program for the working space.

1\. Click the **\[+]** button that is at the top-right part of the panel stack of the working space.

![](<../../_assets/image_47.png>)

2\. On the panel selection window, select **\[WorkCell]**. Then, the robot’s current posture will appear on the 3D window.

![](<../../_assets/image_12.png>)

{% hint style="info" %}
* On the panel selection window, all the items that can be monitored will appear.
* The items that can be monitored will vary depending on controller settings.
{% endhint %}

3\. Check the settings of the working space (![](../../_assets/1.png)), tool space (![](../../_assets/2.png)), tool orientation limiting (![](../../_assets/3.png)), robot elbow space (![](../../_assets/4.png)), and limiting space (![](../../_assets/5.png)).

![](<../../_assets/image_33.png>)

* To adjust the camera, select the **\[Expand/Shrink]** icon (![](../../_assets/image44.png)), the **\[Move]** icon (![](../../_assets/image45.png)), or the **\[Rotate]** icon (![](../../_assets/image46.png)), and drag the screen.
* To modify the setting and apply the set values, close and reopen the WorkCell window.

{% hint style="warning" %}
**\[Caution]**: Compare the robot’s WorkCell simulation position and its actual position, and identify any adjacent obstacles in operating the robot safely.
{% endhint %}
