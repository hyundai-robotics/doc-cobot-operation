# 1.3.1 Collision Detection Controller Settings

1.  Please set the driving mode to manual.

2.  **\[system]** Button > **\[11: Cobot System > Collision Detection]** Please touch the menu.

3. After configuring the settings and options for the collaborative robot's collision detection function, touch the **\[OK]**  button.
![](../../_assets/image64.jpg)

* **\[Collision detection]**: Configure whether to use the collision detection function.
* **\[Body parts for collision detection]**: Select the body part to apply the robot's maximum speed capable of guaranteeing minimum safety against injury upon collision detection.
* **\[Collision detection reaction]**: Select whether to execute an avoidance maneuver after a collision is detected.

{% hint style="warning" %}
**\[Warning]**

* If there is a significant discrepancy between the tool data and actual values, collisions may be incorrectly detected. Please accurately configure tool-related information, such as length, weight, and the center of gravity. Additionally, be sure to verify the robot's installation angle and the direction of gravity. If false detections persist despite accurate tool data configuration, please inspect the encoders and acceleration sensors.
{% endhint %}
{% hint style="warning" %}
**\[Warning]**
* En cas d'écart important entre les données de l'outil et les valeurs réelles, des collisions pourraient être détectées à tort. Veuillez configurer avec précision les informations relatives à l'outil, telles que la longueur, le poids et le centre de gravité. De plus, veillez à vérifier l'angle d'installation du robot ainsi que la direction de la gravité. Si des détections erronées persistent malgré une configuration précise des données de l'outil, veuillez inspecter les codeurs et les capteurs d'accélération.
{% endhint %}