
[__SOURCE](README.md)
# Safety Function Manual for Collaborative Robot

{% hint style="warning" %}
The information presented in this manual is the property of Hyundai Robotics.

The manual may neither be copied, in part or in full, nor redistributed without prior written consent from Hyundai Robotics.

It may neither be provided to any third party nor used for any other purposes.



Hyundai Robotics reserves the right to modify this document without prior notification.



**Copyright ⓒ 2020 by Hyundai Robotics**
{% endhint %}

[__SOURCE](0-about-this-manual/README.md)
# About the Manual

[__SOURCE](0-about-this-manual/precautions.md)
# Precautions

{% include file="en/precautions.md" %}

[__SOURCE](0-about-this-manual/safety-notice.md)
# Safety Cautions

{% include file="en/safety-notice.md" %}

[__SOURCE](1-cobot-safety-function/README.md)
# 1. Safety functions of the collaborative robot


[__SOURCE](1-cobot-safety-function/1-1-description-term.md)
# 1.1 Description of terms

### <mark style="color:green;"> Collision detection </mark>&#xD;

If an external impact exceeding the set threshold is applied while the robot is in operation, it stops to ensure user safety.

*   **Threshold**

    The reference value used to determine whether an external impact has occurred.

### <mark style="color:green;"> Direct teaching </mark>&#xD;

This is a teaching method in which an operator manually moves the robot to a desired path and pose.

*   **Constrained Motion**

    A feature of collaborative robot direct teaching where movement is restricted to specific directions or axes within the Cartesian coordinate system during the teaching process.

*   **Cockpit**

    Buttons used to operate the collaborative robot without relying on a UI.

*   **Cartesian**

    Refers to the Cartesian coordinate system (rectangular coordinate system); a method of expressing the robot's position and movement based on X, Y, and Z coordinates.

*   **Enable Switch**

    Refers to an enabling switch. It serves as a safety switch when operating the robot via a teach pendant in manual mode.
    Positions 1 and 3: Robot operation stops. In the case of Position 3, the switch returns directly to Position 1 without passing through Position 2.
    Position 2: Robot operation is enabled.

### <mark style="color:green;"> Mastering </mark>&#xD;

It refers to the process of aligning the robot's actual joint angles with the joint angles perceived by the controller.
[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/README.md)
# 1.2 Collaborative operation mode

ISO 10218-1 and ISO/TS 15066 describe four operating modes so that operators can practice work safety without being exposed to risks. The collaborative operation should meet a least one of these requirements, and a visual display should show that the system is in collaborative operation when it is in operation.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/1-safety-rated-monitored-stop.md)
# 1.2.1 Safety-rated monitored stop


The robot stops operating when a person enters the workspace. Either install an external monitoring device and connect it to the Safety Control Module (SCM) or use the radar sensor installed on the robot.

* When an external device is connected to the safety input, the stop modes (Stop0, Stop1, and Stop2) should be set in the safety input/output (I/O) signal setting.
* When a safeguard and an external emergency stop device are connected, the stop modes must meet the requirements of the international or local regulations.

The reference information on the setting of the related functions is as follows:

* For detailed information on radar module settings, please refer to the([Configuration procedure](https://github.com/hyundai-robotics/doc-Object-Detection-System/tree/english?cont_model=${cont_model)) section of the ([User Manual ](https://github.com/hyundai-robotics/doc-Object-Detection-System/tree/english?cont_model=${cont_model})).
* For detailed information on safety I/O signal settings, please refer to ([3.3.4 Safety Input/Output](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/4-safety-io/README?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
* For details on configuring the safe stop function, please refer to ([3.3.1.2 Stop Settings](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/1-general-condition/2-safe-stop?cont_model=Hi7?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/2-speed-separation-monitoring.md)
# 1.2.2 Speed and separation monitoring

The robot operates within specified distance and speed limits.

The speed and position monitoring mode controls the robot's operating speed based on the distance between the robot and a person by utilizing sensors capable of detecting the person's position and speed; external distance-sensing sensors or radar sensors mounted on the robot can be used for this purpose.

Reference information regarding the use of the speed and position monitoring mode is provided below.

* For detailed information on radar module settings, please refer to the([Configuration procedure](https://github.com/hyundai-robotics/doc-Object-Detection-System/tree/english?cont_model=${cont_model)) section of the ([User Manual ](https://github.com/hyundai-robotics/doc-Object-Detection-System/tree/english?cont_model=${cont_model})).
* For details on robot safety condition settings, please refer to "([3.3.2.6 Re plan Setting](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/2-robot-safety-condition/6-re-plan?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
* For details on safety I/O signal settings, please refer to ([3.3.4 Safety Input/Output](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/4-safety-io/README?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/3-power-force-limit.md)
# 1.2.3 Power and force limiting

In the event of contact, the system limits the impact force exerted on the human body. Collision detection and TCP force limiting functions serve to restrict the impact on the operator during contact between the operator and the robot.

The collision detection function identifies collisions based on user-defined contact zones, while the TCP force limiting function restricts the external force (N) applied to the TCP. Additionally, the robot's power output can be limited by configuring parameters for power (W) and momentum (kg·m/s).

* For details regarding power and momentum monitoring and power limiting when configuring robot safety conditions, please refer to ([3.3.2 Robot Monitoring Function](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/2-robot-safety-condition/README?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model} )) in ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
* For details on the collision detection function, please refer to **(1.3 Collaborative robot collision detection mode)**.
[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/4-hand-guid.md)
# 1.2.4 Hand guiding

This is a manual operation mode that allows an operator to directly move the robot by hand to teach positions or paths. By utilizing the robot's force control function, the system detects the force applied by the human and moves the robot smoothly in that direction. This enables task setup without the need for complex programming.

In the following description, the terms "hand-guiding" and "direct teaching of collaborative robots" are used interchangeably.

* For more information on hand guiding, please refer to **(1.4 Collaborative robot direct teaching mode)**.

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/README.md)
# 1.3 Collaborative robot collision detection mode

The collision detection function serves as a safety mechanism when the robot operates under abnormal conditions or exhibits irregular behavior. You can configure the detection mode and run auto-tuning to automatically set the optimal collision detection sensitivity for the current task.

Configuration methods include controller settings and robot language commands:
1. Controller settings: Basic settings that are always applied (default).
2. Robot language commands: Robot language commands are used to configure whether collision detection is active for specific segments during robot program execution.

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/1-cobot-collision-detection-setup.md)
# 1.3.1 Collision Detection Controller Settings

1.  Please set the driving mode to manual.

2.  **\[system]** Button > **\[11: Cobot System  > Collision Detection]** Please touch the menu.

3. After configuring the settings and options for the collaborative robot's collision detection function, touch the **\[OK]**  button.
![](../../_assets/image64.jpg)

* **\[Collision detection]**: Configure whether to use the collision detection function.
* **\[Body parts for collision detection]**: Select the body part to apply the robot's maximum speed capable of guaranteeing minimum safety against injury upon collision detection.
* **\[Collision detection reaction]**: Select whether to execute an avoidance maneuver after a collision is detected.

{% hint style="warning" %}
**\[Warning]**

* If there is a significant discrepancy between the tool data and actual values, collisions may be incorrectly detected. Please accurately configure tool-related information, such as length, weight, and the center of gravity. Additionally, be sure to verify the robot's installation angle and the direction of gravity. If false detections persist despite accurate tool data configuration, please inspect the encoders and acceleration sensors.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/2-cobot-collision-detection-roblang.md)

# 1.3.2 Collision-detection robot command(cobot_coldet)

### explanation

Configure whether the collaborative robot performs collision detection.

Collision detection is handled by the Hi7 controller.

### grammar

&lt;cobot_coldet&gt;.on </br>
&lt;cobot_coldet&gt;.off 


### example

cobot_coldet.on</br>
cobot_coldet.off
[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/3-cobot-collision-detection-autotune.md)
# 1.3.3 Collaborative Robot Collision Detection Auto-Tuning Mode

1.  Please set the driving mode to manual.

2.  **\[system]** Button  > **\[11: Cobot System  > 5: Collision Dectection Threshold]** Please touch the menu.

3.  **\[Threshold Init]**  Please touch the button.

4. After configuring whether to enable the automatic tuning function for the collaborative robot's collision detection threshold and setting the number of execution cycles, touch the **\[Save]** button.

![](../../_assets/image65.jpg)

* **\[Auto tuning]**: Configure whether to enable the collision detection auto-tuning function.
* **\[Tuning count]**: Set the number of job executions for performing automatic collision detection tuning.
* **\[Threshold Init]**: Resets the collision detection threshold.
* **\[Factory Reset]**: Resets the collision detection threshold to the factory default value.

{% hint style="warning" %}
**\[warning]**

* Ensure that the robot is not subjected to external impacts while the auto-tuning function is running. If an external impact occurs during execution, please reset and restart the auto-tuning process. 
If the number of auto-tuning iterations is set too low, the process may finish before optimization is complete, potentially leading to frequent false detections; conversely, if the number is set too high, the process may take an excessive amount of time to complete, depending on the execution job's duration. We recommend setting the number of iterations between 100 and 200 for a job with a one-minute execution time. 
Please note that this function operates only in Auto mode; in Manual mode, the collision detection function operates using factory default settings.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-4-cobot-direct-teaching-mode/README.md)
# 1.4 Collaborative robot direct teaching mode

Direct teaching is an intuitive method that allows users without specialized robot programming knowledge to teach a robot desired movements by manually manipulating it. Instead of using a complex teach pendant, the operator directly guides the robot's end-effector to define the work path and positions.

Configuration methods include controller settings and cockpit button settings:
1. Controller settings: Basic settings applied by default.
2. Cockpit button: Activates the direct teaching mode configured on the robot's teach pendant (TP).

[__SOURCE](1-cobot-safety-function/1-4-cobot-direct-teaching-mode/1-cobot-direct-teaching-setup.md)
# 1.4.1 Direct Teaching Controller Configuration

1.  Please set the driving mode to manual.

2.  **\[System]** Button > **\[11: Cbbot System > Direct Teaching]** Please touch the menu.


3. After configuring the settings and options for the collaborative robot's direct teaching function, touch the **[OK]** button.

![](../../_assets/image57.png)

* **Direct Teaching On**: The system operates in direct teaching mode immediately upon motor activation (SHIFT + MOT. ON + Enable Switch). Motor activation and direct teaching operation require the enable switch to be pressed. To switch back to Jog or Auto mode, the 'Direct Teaching On' setting must be turned off.
* **Constraint Motion**: Determines the default mode when direct teaching is active. Selecting 'None' activates FREE mode; while the mode cannot be changed during motor activation in this setting, mode switching is possible during direct teaching in other modes.

![](../../_assets/image60.png) 

4. The image above illustrates the cockpit buttons attached to the HDC series of collaborative robots. Please refer to this image when reading the cockpit settings below.
* **Cockpit setting**: Determines the cockpit button mode.
- Each of the 'Cockpit A, B, and C buttons' can be assigned one of the functions listed below.
    - 'XYZ' = Changes the direct teaching mode to Cartesian constrained motion excluding X, Y, and Z (available only during Cartesian constrained motion).
    - 'XY'  = Changes the direct teaching mode to Cartesian constrained motion excluding X and Y (available only during Cartesian constrained motion).
    - 'X'   = Changes the direct teaching mode to Cartesian constrained motion excluding X (available only during Cartesian constrained motion).
    - 'Y'   = Changes the direct teaching mode to Cartesian constrained motion excluding Y (available only during Cartesian constrained motion).
    - 'Z'   = Changes the direct teaching mode to Cartesian constrained motion excluding Z (available only during Cartesian constrained motion).
    - 'Rx'  = Changes the direct teaching mode to Cartesian constrained motion excluding Rx (available only during Cartesian constrained motion).
    - 'Ry'  = Changes the direct teaching mode to Cartesian constrained motion excluding Ry (available only during Cartesian constrained motion).
    - 'Rz'  = Changes the direct teaching mode to Cartesian constrained motion excluding Rz (available only during Cartesian constrained motion).
    - 'None' = No change occurs when pressed.

- The 'Cockpit M Button' features the menu shown below.
    - 'Save Pose' = Records the robot's current position into the job file currently open on the TP.


* **Joint Direct Teaching Axis Activate**:The selected axis can be driven only when activated during autonomous direct teaching.

{% hint style="warning" %}
**\[warning]**

* Direct teaching may not execute if there is a significant discrepancy between the tool data and actual values. If direct teaching fails to run, please stop the robot and verify the tool data input values.
* To initiate direct teaching, simultaneously press the Motor On button, the Enable Switch, and the Shift key.
* You must keep the Enable Switch pressed after turning on the motor to maintain direct teaching mode.
* Direct teaching will stop if you turn off 'Direct teaching On' or release the Enable Switch while the function is active.
* Please check for nearby objects or people before operating the robot during direct teaching.
* If two or more buttons are pressed simultaneously, only the first button pressed is recognized.
* If you attempt to move the robot automatically using the TP during direct teaching, the robot will stop immediately. This constitutes an emergency stop and poses a safety risk.

{% endhint %}

[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/README.md)
# 1.5 Simple Encoder Offset

This section describes the simple encoder offset mastering function using a device built into the robot.
This function consists of two main parts:
- Simple Mastering Position Setting
- Simple mastering

[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/1-update-mastering-position.md)
# 1.5.1 Simple Mastering Position Setting

The robot requires mastering at a specific position; this section explains how to designate that position. Since the robot moves when the mastering position is set, care must be taken to avoid collisions with people or objects in the vicinity. Note that while there are various possible mastering positions, the system selects a position close to the robot's current posture.

-  **\[system]** Button > **\[11: Cobot System > 11: Simple Encoder Offest ]** Please touch the menu.
- The 'Mastering Position' section displays 'Secondary Encoder' and 'Primary Encoder' values, representing the encoder readings for each joint when the robot is at the mastering position.
- To register a new mastering position, touch the 'Move to New Position' button at the bottom.
    - When the button is touched, the robot moves from its current location to the mastering position.
    - Keep touching the button until the movement is complete; the robot will stop if you release it.
    - Once the movement is complete, touch the 'Update Position' button.
    - Touch the 'Save' button.


    ![](../../_assets/simple_encoder_offset_1.png)

{% hint style="warning" %}

**\[Warning]**
* Tapping the 'Update Position' button without moving to the mastering position will not update the mastering position.
* You must move to the mastering position, tap the 'Update Position' button, and save the setting to establish the new mastering position.
* You must set a new mastering position in the following cases. Using the previously registered mastering position may result in improper mastering or accidents.
    - Secondary encoder replacement
    - Encoder initialization in the  **\[system]** > **\[3: Robot Parameters]** > **\[4: Encoder Offset]** menu
{% endhint %}
[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/2-update-encoder-offset.md)
# 1.5.2 Simple Mastering

This section explains how to initialize (master) the encoder offset after the robot moves to the designated mastering position. Since the robot moves to the mastering position, take care to avoid collisions with people or objects in the surrounding area.

- **\[system]** Button > **\[11: Cobot System  > 11: Simple Encoder Offest ]** Please touch the menu.
- The 'Current Position' section displays the 'Secondary Encoder' and 'Primary Encoder' values ​​for each joint at the robot's current location.
- Touch the 'Move to Position' button at the bottom to move the robot to the mastering position.
    - The robot moves to the mastering position when the button is touched.
    - Keep touching the button until the movement is complete; the robot will stop if you release it.
    - Once the movement is complete, touch the 'Full Reset' button.
    - Touch the 'Save' button.
    - Reboot the controller.

    ![](../../_assets/simple_encoder_offset_1.png)

{% hint style="warning" %}
**\[Warning]**
* A mastering position must be registered to use the simple Mastering function.
* Touching the 'Reset All' button without moving to the mastering position will not reset the encoder offset.
* You must save the settings after performing the encoder offset to update it.
* Frequent use of the simple Encoder Offset function degrades mastering performance; please use it only when necessary.
{% endhint %}    

[__SOURCE](attachment/rules-criteria-and-public-notice.md)
# The Rules on the Criteria for Occupational Safety and Health, and the Public Notice of Safety Inspec

"[Rules on Industrial Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/en/README)"

[__SOURCE](warranty.md)
# Warranty

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/en/README)"