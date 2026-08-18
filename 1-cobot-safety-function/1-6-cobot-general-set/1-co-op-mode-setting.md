# 1.6.1 Co-op Mode Settings

What is collaborative mode? It is a mode that limits the maximum speed to ensure safety in the event of a collision between a collaborative robot and a human. If you wish to operate the robot at speeds exceeding this limit, you can disable collaborative mode after conducting a risk assessment based on industrial robot standards.

- `[F2: system] - 11: Cobot System - Cobot General Settings` Tap the menu.
- Check if Collaborative Mode is enabled (Default: ON).
- Configure the collaborative robot's collaborative mode and maximum speed, then click "Apply to All" to save the settings.
    ![](../../_assets/image61.png) 
    - Co-op Mode On: Sets whether collaborative mode is enabled.
    - Set the Co-op mode Max Speed(mm/s): The maximum speed for collaborative mode entered by the user. Values ​​between 250 and 1000 mm/s can be entered (Default: 800 mm/s).
    - Applied co-op Mode Max Speed(mm/s): Displays the current maximum speed of the collaborative robot. This value represents the final maximum speed, incorporating settings related to collision detection and safety motion.
    - Changes are saved only after clicking "Apply All" and entering the correct password.

{% hint style="warning" %}
**\[warning]**
* Be sure to conduct a risk assessment based on industrial robot standards before disabling this mode.
* The maximum speed resulting from deceleration due to radar detection is not reflected in the "set maximum speed for collaborative mode."
{% endhint %}