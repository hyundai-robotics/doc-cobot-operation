
[__SOURCE](README.md)
# Safety Function Manual for Collaborative Robot

{% hint style="warning" %}
The information presented in this manual is the property of Hyundai Robotics.

The manual may neither be copied, in part or in full, nor redistributed without prior written consent from Hyundai Robotics.

It may neither be provided to any third party nor used for any other purposes.



Hyundai Robotics reserves the right to modify this document without prior notification.



**Copyright ⓒ 2020 by Hyundai Robotics**
{% endhint %}

[__SOURCE](about-this-manual/README.md)
# About this manual

이 설명서는 현대로보틱스 협동로봇의 안전 기능에 대해 설명합니다.

제품을 사용하기 전에 반드시 설명서의 내용을 충분히 숙지하시기 바랍니다. 또한 필요할 때 언제든 볼 수 있도록 설명서를 가까운 장소에 보관하십시오.

이 설명서는 현대로보틱스 제품을 구매한 고객에게 참조용으로 제공되거나 교육을 위한 내부 교육 자료로 제공되어 사용될 수 있습니다.

이 설명서는 표준 사양을 기준으로 작성되었으므로 구입하신 제품의 모델에 따라 일부 내용이 다를 수 있습니다. 또한 이 설명서의 내용과 사양은 제품의 성능 향상을 위해 예고 없이 변경될 수 있으며 부정확한 내용이나 오탈자로 인해 발생하는 상황에 대해서 현대로보틱스는 책임이 없습니다. 개정에 관한 상세한 정보는 당사의 인터넷 웹사이트([www.hyundai-robotics.com](https://www.hyundai-robotics.com))를 방문하여 확인하시기 바랍니다.


[__SOURCE](about-this-manual/copyright.md)
# Copyright

All the programs, files, and contents relating to this product and manual are protected by the Copyright Act and a confidentiality agreement. Any use, reproduction, and disclosure or distribution of this manual to third parties not explicitly permitted by Hyundai Robotics are strictly prohibited.

Copyright ⓒ 2020 HYUNDAI ROBOTICS. All rights reserved.

[__SOURCE](about-this-manual/notation.md)
# Notation rules

This manual utilizes the following expression rules and safety directions for easy understanding.

### <mark style="color:green;">Description by figures</mark>

Figures are used for a better understanding of how to operate the product and for describing screens. When a description is made by a figure, the pertaining part is marked with the figure number that describes the part, as shown in the following figure:

![](../_assets/image\_explan.png)

### <mark style="color:green;">GUI (Graphical User Interface)</mark>

Regarding GUI, any menu name or button name will be in brackets (**\[ ]**) and in **bold type**. When multiple menus need to be selected in the listed order, the menu names will be separated by the symbol (>).

* Menu having a title: On the initial screen of the manual or automatic mode, click the **\[Menu]** button.
* Multiple menus: In the initial screen of the manual mode, select the **\[Setting]** button > **\[5: Reset > 7: Unit Setting]** menu.

### <mark style="color:green;">Manipulation key notation method</mark>

Any key to be pressed in the functional manipulation area of the teach pendant will be in angle brackets (**< >**) and in **bold type**.

* Pressing the **\<Start>** key will initiate the automatic execution of the sequence programmed into the robot.

### <mark style="color:green;">Cross-references</mark>

This provides the shortcut to the related information in the manual. Cross-references will be in quotation marks and in **bold type**.

* For details of making changes in date and time information, see “**4.5 Date and time setting**.” of “**Operation Manual for Hi6 Controller**” &#x20;

### <mark style="color:green;">References</mark>

Useful or additional information on using the product will be provided as follows:

{% hint style="info" %}
The blinking of the![](../_assets/engineer.png) icon in the status bar indicates the engineer mode.
{% endhint %}

[__SOURCE](about-this-manual/safety-notice.md)
# Safety precautions

To ensure proper product use and user safety and to prevent property damages, make sure to read and fully understand the following precautions before using the product.

### <mark style="color:green;">Danger</mark>

{% hint style="danger" %}
**\[Danger] impending risk**: If not conformed to, operator deaths or severe injuries may occur.
{% endhint %}

*   Perform a risk assessment on the entire system, not the individual devices. Connecting other devices to the product may increase the risk level of the product or create new risks. If the devices of the integrated robot system have different risk levels, prepare safety devices based on the device with the highest risk level in preparedness for risks.


*   In installing the robot product and other devices, make sure to read, fully understand, and conform to the product installation instructions described in the manual.


*   In case of any issues of the product, such as faults and damages, stop using the product immediately and contact our Customer Support Team.



### <mark style="color:green;">Warning</mark>

{% hint style="warning" %}
**\[Warning] Potential risk**: If not conformed to, operator injuries or property damages, including serious product damages, may occur.
{% endhint %}

*   Take adequate safety measures according to the result of risk assessment, and accurately assign the safe range of robot installation. During the robot operation, product damages or user injuries may occur.


*   Persons who manufacture robot application systems or use the robot must read and fully understand the manual and undergo training in robot operation.


*   For the safety of operators and users, prepare adequate safety facilities such as safety fences before installing the product.


*   Secure sufficient space so that the robot arm can move freely. During the robot operation, product damages or user injuries may occur.

    Fasten locking bolts to the specified torque according to the specification sheet. Loose bolts may lead to damages of the robot because of falling from the installation position.


*   Pay attention to the product connections (power and cables) so that no conductive substances, such as liquid, dust, and metal particles, could infiltrate. Do not poke the connection with sharp objects or apply excessive force during cable connection. Corrosion or temporary short circuits of connectors may lead to product explosion or fires.


*   Check the wiring specification and connect devices with terminals that are suitable for the device types. Make sure to connect safety devices to dedicated terminals because connecting them to general terminals does not guarantee safety functions.


*   Never use damaged cables and do not disconnect cables while the product is in use. Doing so may lead to electric shocks, fires, faults, and injuries.


*   Long-time use of the product may lead to overheating and cause injuries such as burns. In the event it is necessary to touch the product, cool down the product sufficiently by powering it off and leaving it for at least one hour.


*   Never arbitrarily install, modify, disassemble, or repair the product. This may lead to faults and accidents. Hyundai Robotics will not take responsibility for product damages caused by such arbitrary actions.



### <mark style="color:green;">Caution</mark>

{% hint style="warning" %}
**\[Caution] Minor risk**: If not conformed to, minor operator injuries or property damages, including product damages, may occur.
{% endhint %}

*   Do not arbitrarily install, modify, disassemble, or repair the product. It is prohibited for persons other than experts from Hyundai Robotics to modify or attach parts to the product. Product faults caused by it will void free-of-charge services and warranty services.


*   In the event it is necessary to install or repair the product, contact our Customer Support Team to consign the work to experts.


*   Do not install or use the product at a place filled with dust or dirt. Dust or foreign matters may lead to product faults or malfunctions.


*   Do not install or use the product at a place of magnetism, a place which is affected by magnetism, or a place of electromagnetic interferences. Magnetism may lead to product damages or malfunction.


*   In operating the product, do not wear loose clothes or accessories. If you have long hair, you should tie it at the back of your head so it will not entangle between joints and the like of the robot.


*   While the product is in operation, do not enter its operating range or touch the robot. Doing so may lead to injuries.


*   Transport the product as it is packaged to prevent product damages, and store it at a dry and low-humidity place. Storing it at a humid place may lead to product damages or faults caused by moisture infiltration.


*   Store the product at a place that is clean, cool, dry, and free from high variation in temperature and humidity.


*   The product should be moved by two or more persons, and the correct posture should be maintained. If not, the persons may be subject to physical injuries in the waist, arms, legs, and the like.


*   In moving the product using lifting equipment, conform to the local and national safety regulations and the instructions for equipment use.


* Before moving the product, read and conform to the moving instructions specified in the manual. Hyundai Robotics will not take responsibility for product damages caused during transportation by the customer.

[__SOURCE](1-cobot-safety-function/README.md)
# 1. Safety functions of the collaborative robot


[__SOURCE](1-cobot-safety-function/1-1-description-term.md)
# 1.1 Description of terms

### <mark style="color:green;">Robot limiting parameters</mark>&#xD;

These are the parameters that constitute the criteria for monitoring the speed, force, and momentum of the robot.

*   **Tool center point (TCP) position monitoring**

    This monitors whether the safety tool model violates the safety space. In cases when the safety space is intruded into, the safety stop set by the user will be actuated.
*   **TCP orientation monitoring**

    This monitors whether the tool orientation is out of the specified range. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **TCP speed monitoring**

    This monitors the speed of the tool tip. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **TCP force monitoring**

    This monitors the force of the tool tip. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **Power monitoring**

    This monitors the power of the robot. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **Momentum monitoring**

    This monitors the momentum of the robot. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **Collision detection**

    In cases when the allowable value is exceeded because of an external force applied to the robot, the safety stop set by the user will be actuated.
*   **Safe operating stop (SOS) monitoring**

    This monitors whether the robot stops without any slips. In cases when the specified value is exceeded, Stop0 will be actuated. Meanwhile, when a stop condition is met while the robot is in the automatic mode, this function will be actuated automatically.

### <mark style="color:green;">Joint limiting parameters</mark>&#xD;

These are the parameters that form the reference for monitoring the position, speed, and torque of each robot joint.

*   **Joint angle monitoring**

    This monitors the position of each axial joint. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **Joint speed monitoring**

    This monitors the speed of each axial joint. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
*   **Joint torque monitoring**

    This monitors the torque of each axial joint. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.



### <mark style="color:green;">Safety layout</mark>&#xD;

These are the parameters for the safe space and the tool space that form the criteria for monitoring the TCP position and orientation.

*   **Safety space**

    This refers to the working space and the protected space of the tool.
*   **Working space**

    This refers to the space in which the robot carries out work. If the tool or the robot’s elbow model goes out of the working space, the safety stop function will be actuated.
*   **Protected space**

    This refers to the space where the operator should be safeguarded from the robot. If the tool or the robot’s elbow model goes out of the protected space, the safety stop function will be actuated.
*   **Safety tool modeling**

    The tool attached to the robot is modeled in spheres and cones to monitor the TCP position and orientation.
*   **Safety robot modeling**

    The robot’s elbow is modeled in spheres to monitor its distance from the safety space.



### <mark style="color:green;">Safety space</mark>&#xD;

This is the function that stops the robot if any safety conditions are violated. There are three methods for the safety stop. For more details on the methods, refer to ISO 13850 or IEC 60204-1.

*   **Stop0**

    The power of the motors of all the joint modules will disconnect immediately, and the motors will stop (uncontrolled stop).
*   **Stop1**

    The motors of all the joint modules will decelerate and stop, and the power of the motors will disconnect (controlled stop). The robot will decelerate as it continues to move along the programmed path, and then it will stop. As soon as the robot stops, its power will be disconnected.
*   **Stop2**

    The motors of all the joint modules will decelerate, and the safe operating stop (SOS) will take effect. The power supply status of all the motors will be retained.

### <mark style="color:green;">Recovery mode</mark>&#xD;

When the robot stops because of the safety function, you can clear the error and position the robot in the safe space while it is in recovery mode. However, when the safety board is in the FAULT state, the error cannot be cleared in recovery mode, and the system should be rebooted.



### <mark style="color:green;">Direct teaching</mark>&#xD;

This is a method in which teaching is performed by moving the robot directly. This function is actuated by a switch that is mounted on the robot.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/README.md)
# 1.2 Collaborative operation mode

ISO 10218-1 and ISO/TS 15066 describe four operating modes so that operators can practice work safety without being exposed to risks. The collaborative operation should meet a least one of these requirements, and a visual display should show that the system is in collaborative operation when it is in operation.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/1-safety-rated-monitored-stop.md)
# 1.2.1 Safety-rated monitored stop

When a person enters the working space, the robot operation will stop. Install an external monitoring device, and use it while connected to the safety control module (SCM).

* When an external device is connected to the safety input, the stop modes (Stop0, Stop1, and Stop2) should be set in the safety input/output (I/O) signal setting.
* When a safeguard and an external emergency stop device are connected, the stop modes must meet the requirements of the international or local regulations.

The reference information on the setting of the related functions is as follows:

* For more details on the setting of safety I/O signals, see “[1.8 Safety I/O signals.](../1.8-safety-io-signal.md)”
* For more details on the setting of safety stop functions, see “[1.9 Safety Stop Function.](../1-9-safety-stop-function.md)”

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/2-hand-guide.md)
# 1.2.2 Hand guiding

This is a method in which the operator holds and directly controls the robot’s manipulator. This method is available in the automatic operation mode.

To move the robot’s manipulator directly in the manual mode, you can use free motion and specific constraint motion by direct teaching with an external switch. For more details on direct teaching, see “[2. Direct teaching.](../../2-direct-teaching/)”

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/3-speed-separation-monitoring.md)
# 1.2.3 Speed and separation monitoring

The robot operates within a specified distance and speed.

In the speed and separation monitoring mode, the driving speed of the robot is controlled in proportion to the distance and the relative speed between the robot and the operator, utilizing sensors that can detect the operator’s position and speed. You can use the deceleration mode for the inputs of the external sensors that detect distance.

The reference information on the use of the speed and separation monitoring mode is as follows:

* For more details on the setting of the robot’s safety condition level 0 (deceleration mode), see “[1.6 Robot safety conditions.](../1-6-robot-safety-condition/)”
* For more details on the setting of safety I/O signals, see “[1.8 Safety I/O signals.](../1.8-safety-io-signal.md)”.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/4-power-force-limit.md)
# 1.2.4 Power and force limiting

This limits the impact on the human body in case of a collision. The collision detection function and the TCP force limiting function can limit the impact on the operator in case of a collision between the operator and the robot.

The collision detection function detects collisions according to the set sensitivity (%), while the TCP force limiting function restricts external force (N) applied to the TCP. You can also restrict the robot’s driving power by setting the electric power (W) and momentum (kg·m/s).

For more details on the setting of the robot’s safety conditions, see “[1.6 Robot safety conditions.](../1-6-robot-safety-condition/)”

[__SOURCE](1-cobot-safety-function/1-3-safety-function/README.md)
# 1.3 Safety functions

The purpose of the safety functions of the collaborative robot is to reduce the impact on the operator in the case of a collision between the operator and the robot during collaborative operation.

The safety functions include the “axis limiting function,” which restricts the motion of the robot’s joints, and the “robot limiting function,” which restricts the robot’s motion in the safety space. These functions can be configured in the setting menu and are used as measures to respond to the risks selected in the risk assessment performed by the operator.

In executing the safety functions, the following items should be configured:

*   **Safety space**: Set the working space and the protected space to restrict the robot’s motion.


*   **Tool modeling**: This is used to check whether the robot’s tool position intrudes or exceeds specific spaces.


*   **Robot modeling**: This is used to check whether the robot’s elbow position intrudes or exceeds specific spaces.


* **Safety limiting conditions**: Set monitoring criteria value for the safety functions.

One safety condition can be configured for each safety space; if not configured, Level1 (default setting mode) will be set as the default condition. You can add up to 5 limiting conditions, 16 tools, and 12 safety spaces. You can set, modify, or enable the parameters relating to the safety function only when the motors are turned off in the manual mode.

[__SOURCE](1-cobot-safety-function/1-3-safety-function/1-robot-limit-function.md)
# 1.3.1 Robot limit functions

The robot limiting functions, which restrict the robot’s motion in the safety space, include the following:

*   **TCP position**: This restricts the tool or the elbow shapes of the robot modeled in spheres from intruding or exceeding a set space.

    ****
*   **TCP orientation**: This restricts the orientation of the robot’s end effector and the tool from deviating from a set orientation.

    ****
*   **TCP speed**: This restricts the robot’s speed to a low speed so that the operator can escape in case of a collision with the robot (the robot moves at a maximum speed of 250 mm/s in the manual mode and the direct teaching mode).

    ****
*   **TCP force, power, and collision detection**: This limits the force and pressure in case of a collision between the robot and the operator.

    ****
* **Momentum**: This limits the energy and impact load in case of a collision between the robot and the operator.

[__SOURCE](1-cobot-safety-function/1-3-safety-function/2-joint-limit-function.md)
# 1.3.2 Joint limit functions

The joint limiting functions, which restrict the robot’s motion in the joint space, include the following:

* **Joint position**: This limits the robot’s joint positions so that its axes can move only within the specified ranges.
* **Joint speed**: This limits the robot’s momentum so that its axes cannot move beyond the specified speeds.
* **Joint torque**: This limits the robot’s power and force by restricting the torques of the axes to reduce the force and pressure applied on the operator in case of a collision with the robot.

{% hint style="warning" %}
**\[Caution]** : To ensure the safety of personnel and equipment around the robot, operators and users should perform a risk assessment before configuring the robot’s safety function and set the following details according to the assessment result:

* Set passwords and the like so that the safety configuration cannot be modified by unauthorized persons.
* Set safety-related functions and interfaces.
* Check if the settings are correct before running the robot.
* Check if all the safety functions are configured and if the settings conform to the result of the risk assessment.
{% endhint %}


[__SOURCE](1-cobot-safety-function/1-4-check-replacing-safety-devices.md)
# 1.4 Matters to be checked upon replacing safety devices

When the robot, controller, working tool, or an external device used for operating the collaborative robot is replaced, you should check the current settings and modify them as necessary. The safety functions that must be checked upon the replacement of a device include the following:

|                                   Device                                  | Matters to be checked                                                                                                                                        | Reference                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| :-----------------------------------------------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                                 **Device**                                | 　　**Matters to be checked**                                                                                                                                  | 　　　　　**Reference**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| All the axial modules of the robot (motors, encoders, and torque sensors) | <ul><li>Reconfiguration of encoder options</li><li>Reconfiguration of torque sensor offsets</li></ul>                                                        | <ul><li><strong></strong><a href="1-5-check-before-using-the-safety-function/1-encoder-offset.md"><strong>1.5.1</strong> <strong>Encoder offset</strong></a><strong></strong></li><li><strong></strong><a href="1-5-check-before-using-the-safety-function/2-torque-sensor/"><strong>1.5.2 Checking the torque sensor</strong></a><strong></strong></li></ul>                                                                                                                                            |
|                      Main controller (microcomputer)                      | <ul><li>System resetting</li><li>Reconfiguration of all safety-related functions</li></ul>                                                                   | User manual                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|                               Working tools                               | <ul><li>Checking of tool data</li><li>Checking of safety tool modeling</li><li>Checking of axial load weights</li><li>Checking of tool I/O setting</li></ul> | <ul><li><strong></strong><a href="1-5-check-before-using-the-safety-function/3-tool-data-setting.md"><strong>1.5.3</strong> <strong>Setting of tool data</strong></a><strong></strong></li><li><strong></strong><a href="1-7-safety-layout/2-safety-tool-modeling.md"><strong>1.7.2 Safety tool modeling</strong></a><strong></strong></li><li>User manual</li><li><strong></strong><a href="../3-io-setting/3-2-tool-io/"><strong>3.2</strong> <strong>Tool I/O</strong></a><strong></strong></li></ul> |
|                           External input devices                          | Checking of safety I/O setting                                                                                                                               | 1.8 Safety I/O signals                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

{% hint style="warning" %}
**\[Caution]**: Check if the settings are correct before running the robot.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/README.md)
# 1.5 Matters to be checked before using the safety functions


[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/1-encoder-offset.md)
# 1.5.1 Encoder offset

The accuracy of encoder data is important because the safety functions of the collaborative robot detect the robot’s position and speed based on the data transmitted by the encoders attached to the axes. Therefore, before using the safety functions, check whether the encoder values match the actual values.

1\. **** Check the zero mark of each axis of the robot and move the axes.

In recovery mode, move each axis with the jog if a stop occurs because of a safety function violation. For more details on recovery mode, see “[**1.10.5 Recovery mode**.](../1-10-safety-condition-monitoring/5-recovery-mode/)”

2\. **** In the pose information window on the workspace, check whether the axial coordinate values of the robot are displayed at the reference pose (**0, 90 0, 0, 0, 0** \[deg]).

![](<../../_assets/image_35.png>)



* Click the **\[+]** button at the top right part of the panel stack if the pose information window does not appear on the workspace. Then, click **\[Pose]** in the panel selection window.

![](<../../_assets/image_43.png>)

3\. Proceed to the next step if the difference of the angular value is no larger than 0.01. Otherwise, carry out the encoder offset if it is larger than 0.01.

4\. Reboot the system.

{% hint style="info" %}
For more details on the encoder offset, see “[7.4.4 Encoder offsets](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/7-setting/7-4-robot-parameter/encoder-offset)” of the “[Operation Manual for Hi6 Controllers.](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/)”
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/2-torque-sensor/README.md)
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

[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/2-torque-sensor/2-1-torque-sensor-offset.md)
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

[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/3-tool-data-setting.md)
# 1.5.3 Setting of tool data

The safety functions of the collaborative robot monitor the entire robot system including the tool attached to the robot’s tool flange. Therefore, the smaller the difference between the tool data and its actual value, the more accurately the safety functions will work. Set the length and angle of the tool based on the flange coordinate system and input the information on the weight, center of gravity, and inertia of the tool in the applicable units.

1. Set the operating mode to the manual mode.
2. Disconnect the power of the motor by pressing the emergency stop button.
3. Select the **\[Configure]** > **\[3: Robot parameter > 1: Tool data]** menu.
4. Check the data of each axis, set the weight, center of gravity, and inertia of the tool, and save the values by clicking the **\[OK]** button.

![](<../../_assets/image_39.png>)

* To easily create new tool data from scratch utilizing the current program, click the \[Auto calibration] button.
* To correct the tool angle, click the \[Angle calibration] button.
* To add a new user coordinate system or delete one, use the \[+] or \[-] buttons, respectively.
* To view and edit the detailed information of tool data, select a tool data name to be viewed and edited.
* To copy the information on tool data and paste it to that of another, use the \[Copy page] and \[Paste page] buttons, respectively.

{% hint style="info" %}
* When there is no information on the weight and center of gravity of a tool, you can estimate the values using the load estimation function. For more details, see “[**Operation Manual for Hi6 Controllers.**](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/)”
* For more details on tool data setting, see “[**Operation Manual for Hi6 Controllers.**](https://hyundai-robotics.gitbook.io/hi6-operation-manual/v/op-english/)”
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-5-check-before-using-the-safety-function/4-password-setting.md)
# 1.5.4 Password setting

The parameters for the safety functions of the collaborative robot must be set and managed by a designated person. A user designated as the administrator will be given the administrator authority and password for system setting. The password for system setting should be input when setting the parameters for the safety functions. When a wrong password is input, the administrator cannot modify or set the parameters.

1. Select the **\[Configure]** button > **\[5: Initialize > 11: system password setting]** menu. The password setting window will appear.
2. Enter the password, and click the **\[OK]** button.

![](<../../_assets/image_34.png>)

* In setting the parameters of the safety functions, the system setting password must be input for saving changes.

![](<../../_assets/image_29.png>)

[__SOURCE](1-cobot-safety-function/1-6-robot-safety-condition/README.md)
# 1.6 Robot safety conditions

The robot safety conditions, which are the limit values for monitoring the safety functions, consist of the robot limiting parameters and the joint limiting parameters.

You can enable the desired safety conditions for each safe space. In a space for which no specific conditions are designated or a space that is not enabled, the monitoring will be done based on Condition1 (default setting mode). When the deceleration mode is enabled, the monitoring will be done based on Condition0.

The method for setting safety conditions is as follows:

1\. Select the **\[Configure]** button > **\[4: Application parameter > 21: Cobot setup > 1: Cobot Safety function > 1: Safety condition]** menu. The safety condition setting window will appear.

2\. Check and set the parameter values of the safety conditions, and save them by clicking the **\[Apply]** button.


****
_assets
![](<../../.gitbook/assets/image_49.png>)

|              **No.**              | 　　　　　　　　　　**Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| :---------_assets-------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![](../../_assets/1.png)  | <p>These are the details of the safety condition. You can view and set the condition name and the parameter values.</p><ul><li><strong>[Name]/[Description]</strong>: These are the name and description of the safety condition.</li><li><strong>[Robot limit]</strong>: This is the setting information on the robot limiting parameters of the safety condition. For more details, see “1.6.1 Robot limiting parameters”</li><li><strong>[Joint limit]</strong>: This is the setting information on the joint limiting parameters of the safety condition. For more details, see “1.6.2 Joint limiting parameters.”</li></ul>                                                                                                                                                                                                                    |
| ![](../../.gitbook/assets/2.png)  | <ul><li><strong>[Apply]</strong>: This saves changes.</li><li><strong>[+]/[-]</strong>: “+” adds a new safety condition, and “-” deletes an existing safety condition. You can add up to five safety conditions.</li><li>This is the list of safety conditions. If you select a condition name, you can view and modify its details.</li><li><p><strong>[Copy page]/[Paste page]</strong>: “Copy page” copies the information on a safety condition, and “Paste page” pastes it to another.</p><p>In the list of safety conditions, select the name of a condition, click the <strong>[Copy page]</strong> button, select the name of another condition to which the condition will be applied, and click the <strong>[Paste page]</strong> button.</p></li><li><strong>[Reset all]</strong>: This initializes all the safety conditions.</li></ul> |

3\. After checking the parameter values, finish the setting by clicking the **\[X]** button or by clicking the **\<esc>** key of the teach pendant.

[__SOURCE](1-cobot-safety-function/1-6-robot-safety-condition/1-robot-limit-parameter.md)
# 1.6.1 Robot limiting parameters

These parameters are the limit values for monitoring the safety functions relating to the robot’s driving in the safety space. If a robot limiting parameter is enabled in a Cartesian space, monitoring will be done at all times, and if the deceleration mode is enabled, monitoring will be done based on Condition0. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set parameter values in the **\[Robot limit]** tab of the **\[Set up > 4: Application parameter > 21: Cobot setup > 1: Cobot Safety Function > 1: Safety condition]** menu.

![](<../../_assets/image_24.png>)

|    **Parameter**    | 　　　　　　　　　**Description**                                                                               | **Default setting value** |
| :-----------------: | ------------------------------------------------------------------------------------------------------ | :-----------------------: |
|      TCP speed      | The TCP speed limiting value in the robot’s coordinate system (1–5,000 mm/s)                           |         1,500 mm/s        |
|      TCP force      | <p>The force limiting value applied to the TCP </p><p>(50–1,000 N)</p>                                 |           150 N           |
|        Power        | The mechanical power limiting value of the robot (80–1,000 W)                                          |           350 W           |
|       Momentum      | The momentum limiting value of the robot (excluding payload) (50–1,000 kg·m/s)                         |         50 kg·m/s         |
| Collision detection | The sensitivity of the collision detection function (0%–200%)                                          |            100%           |
| Reduced speed ratio | The reduced speed ratio of the speeds (TCP and joint speeds) set in the deceleration mode (Condition0) |            20%            |

{% hint style="warning" %}
**\[Caution]**&#x20;

* In configuring a speed limit, you must consider the stop reaction time and put a cover on the target to prevent collisions and injuries.
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-6-robot-safety-condition/2-joint-limit-parameter.md)
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

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/README.md)
# 1.7 Safety layout

This sets the safety space, safety tools, and safety robot elbow.

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/1-safety-space-setting/README.md)
# 1.7.1 Safety space setting

The safety space is a working space or a protected space in which the range of the tool or the robot elbow is monitored. The working space is a limited space where the monitoring target can move freely but cannot exceed. In contrast, the protected space is a limited space in which the monitoring target cannot move when it intrudes into the space. If the safety space is a working space, you can enable it by assigning a safety condition number. In the working space, if the monitoring target moves and exceeds the limit value of a safety condition, a functional safety stop will be actuated.

![Figure 6 Safety space: Working space](<../../../_assets/image_36.png>)

![Figure 7 Safety space: Protected space](<../../../_assets/image_32.png>)

A safety space should be configured by setting the position and length of the zero point based on the robot coordinate system, including a stopping distance. You can add up to 12 spaces, each of a cuboid shape. The safety space is enabled by setting parameters or safety I/O signals.

The method for setting safety spaces is as follows:

1\. Click the **\[Configure]** button > **\[4: Application parameter > 21: Cobot setup > 1: Cobot Safety Function > 2: Safety layout]** menu.

2\. Select the type of safety space, set the parameter values, and save them by clicking the **\[Apply]** button.



![](<../../../_assets/image_17.png>)

|                **No.**               | 　　　　　　　　　　**Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| :----------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  ![](../../../_assets/1.png) | These are the details of the safety space. You can view and set the space name and the parameter values. For more details on the setting, see “[**1.7.1.1 Setting information on safety space parameters.**](1-1-safety-space-parameter-setting-info.md)”                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|  ![](../../../_assets/2.png) | <ul><li><strong>[Tool]</strong>: This sets the parameter values of the tool used for safety space monitoring. For more details, see “<a href="../2-safety-tool-modeling.md"><strong>1.7.2 Safety tool modeling</strong>.</a>”</li><li><strong>[Robot]</strong>: This sets the parameter values of the robot model used for safety space monitoring. For more details, see “<a href="../3-safety-robot-modeling.md"><strong>1.7.3 Safety robot modeling.</strong></a>”</li></ul>                                                                                                                                                                                                                                           |
|  ![](../../../_assets/3.png) | <ul><li><strong>[Apply]</strong>: This saves changes.</li><li><strong>[+]/[-]</strong>: “+” adds a new safety space, and “-” deletes an existing safety space. You can add up to 12 safety spaces.</li><li>This is the list of safety spaces. If you select a space name, you can view and modify its details.</li><li><p><strong>[Copy page]/[Paste page]</strong>: “Copy page” copies the information on a safety space, and “Paste page” pastes it to another.</p><p>In the list of safety spaces, select the name of an space, click the <strong>[Copy page]</strong> button, select the name of another space to which the values will be applied, and click the <strong>[Paste page]</strong> button.</p></li></ul> |

3\. After checking the parameter values, finish the setting by clicking the **\[X]** button or by clicking the **\[esc]** key of the teach pendant.

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/1-safety-space-setting/1-1-safety-space-parameter-setting-info.md)
# 1.7.1.1 Setting information on safety space parameters

![](<../../../_assets/image_22.png>)

{% hint style="warning" %}
**\[Caution]**

* The robot monitoring function is carried out based on the configured spaces and modeled tools. The spaces and tools should include all the components including distance.
* Put a cover on the robot to prevent collisions and injuries.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/2-safety-tool-modeling.md)
# 1.7.2 Safety tool modeling

Safety space monitoring detects whether the tool modeled in spheres intrudes into the safety spaces or exceeds the working space. You can set up to 16 safety tools and model a safety tool with a maximum of 6 spheres.

Because a safety tool is enabled by a number that is set on the teach pendant, you should model a safety tool based on the tool data set in the **\[Setting > 3: Robot parameter > 1: Tool data**] menu. Refer to the TCP position information displayed at the top of the tool data setting window.

Each sphere used for safety tool modeling is set by its center and radius. Set the center position of the sphere for the modeling based on the robot flange coordinate system (Xf, Yf, and Zf), and set the radius of the sphere, including the tool size and the stopping distance, at the maximum TCP speed.

![Figure 8 Tool modeling](../../_assets/image33.png)

![Figure 9 Robot flange coordinate system](../../_assets/image34.png)

To use the TCP orientation limiting function in safety tool modeling, you can set cones for monitoring by setting rotation and deviation angles in creating the reference vector.

You can model a cone (![](../../_assets/2.png)) that is formed with generator lines spread by the deviation angle (![](../../_assets/4.png)) from the reference vector (![](../../_assets/3.png)), which is set by the rotation of the Z-direction vector of the robot coordinate system (![](../../_assets/1.png)) at a specified angle. The vertex (![](../../_assets/5.png)) of the cone is located at the TCP, and if the Z-direction vector (![](../../_assets/6.png)) of the TCP exceeds the monitoring cone, a violation error of the TCP position limiting function will occur.

_assets
![Figure 10 TCP orientation limiting function](../../.gitbook/assets/image38.png)

You can set parameter values by clicking the **\[Tool]** button in the **\[Set up > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 2: Safety layout]** menu.
_assets
![Figure 11 Safety tool modeling setting window](<../../.gitbook/assets/image_26.png>)
_assets
![](<../../.gitbook/assets/image_16.png>)

{% hint style="info" %}
If you use the **\[Copy TCP]** button, the rotational angle values that can be set as the Z-direction vector of the current TCP will be applied to the reference vector, which facilitates the setting of the reference vector.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**

* Before changing a tool data, check if the parameters set in the tool modeling are correct. The tool data number and the safety tool modeling number of a tool should be equal to each other.
* Because the definition of a robot layout setting applies to the elbow, the other parts of the robot may intrude into a safety space even if a safety space is set.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/3-safety-robot-modeling.md)
# 1.7.3 Safety robot modeling

This is the robot model used for safety space monitoring. There is only one safety robot model, and the model consists of a sphere.

The sphere used for safety robot modeling is specified by its center and radius. The sphere center of the model is the position of the robot’s elbow (axis 3: V axis), and the radius should be large enough to include the current size of the elbow and its stopping distance at the maximum TCP speed.

To set the parameter values, click the **\[Robot]** button in the **\[Configure > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 2: Safety layout]** menu.



![Figure 12 Safety robot modeling setting window](<../../_assets/image_11.png>)

|   Parameter   | Description                                                                         |   Default setting value   |
| :-----------: | ----------------------------------------------------------------------------------- | :-----------------------: |
| **Parameter** | 　　　　　　　　**Description**                                                             | **Default setting value** |
|      Name     | The name of the selected safety robot model (name character string, not modifiable) |           Robot           |
|     On/Off    | <p>Whether to enable monitoring </p><p>(Off = no monitoring, On = monitoring)</p>   |            Off            |
|     Radius    | Radius of the sphere (0–10,000 mm)                                                  |            0 mm           |

[__SOURCE](1-cobot-safety-function/1-7-safety-layout/4-workcell-3d.md)
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

[__SOURCE](1-cobot-safety-function/1.8-safety-io-signal.md)
# 1.8 Safety I/O signals

This assigns safety I/Os in using the collaborative robot. Each safety I/O is of a dual channel. You can set up to four signals each for input and output.

1\. Select the **\[Configure]** button > **\[4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 3: Cobot Safety I/O]** menu.

2\. Click the drop-down menu, configure I/O signals, and click the **\[Apply]** button.



![](<../_assets/image_23.png>)

#### <mark style="color:green;">Input signal assignment</mark>

| **Parameter** | 　　　　　　　　**Description**                                                                                                                                                                                                                                    |
| :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    IN0–IN3    | <p>Activation signal assignment </p><p>(up to 4 signals, 0–22)</p><ul><li>0 = None</li><li>1 = Stop 0</li><li>2 = Stop 1</li><li>3 = Stop 2</li><li>4 = SOS</li><li>5 = Reduced mode</li><li>7 = Motor on</li><li>11–22 = Safety spaces #1 - #12</li></ul> |

#### <mark style="color:green;">output signal assignment</mark>

| **Parameter** | 　　　　　　　　　**Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| :-----------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   OUT0–OUT3   | <p>Monitoring signal assignment </p><p>(up to 4 signals, 0–43)</p><ul><li>0 = None </li><li>1 = STO activation status </li><li>2 = SOS activation status </li><li>3 = Reduced mode activation status </li><li>4 = Not reduced mode </li><li>5 = Robot moving </li><li>7 = Mode switch – manual </li><li>8 = Mode switch – auto</li><li>9 = Mode switch – remote </li><li>10–21 = Safety spaces #1 - #12 </li><li>22 = Violation alarm </li><li>23 = TCP speed violation </li><li>24 = TCP orientation violation </li><li>25 = TCP force violation </li><li>26 = Collision detection </li><li>27 = Momentum violation </li><li>28 = Power violation </li><li>29 = SOS violation </li><li>30 = Joint position violation </li><li>31 = Joint speed violation </li><li>32 = Joint torque violation </li><li>33-43 = Safety space violation #1 - #12</li></ul> |

3\. After checking the parameter values, finish the setting by clicking the **\[X]** button or by clicking the **\<esc>** key of the teach pendant.

[__SOURCE](1-cobot-safety-function/1-9-safety-stop-function.md)
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

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/README.md)
# 1.10 Safety condition monitoring

This monitors safety function violations and the status of the SCM board. You can view the statuses of the robot limiting functions, joint limiting functions, and the SCM board.

1. &#x20;**** Select the **\[Configure]** button > **\[4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 5: Cobot Safety Status]** menu.
2. Check the safety conditions and the statuses of the safety functions of the collaborative robot.

![](<../../_assets/image_41.png>)

|                No.                | Description                                                                                                                                                                                                                                                                                                             |
| :-------------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|              **No.**              | 　　　　　　　　　**Description**                                                                                                                                                                                                                                                                                                |
|  ![](../../_assets/1.png) | View the safety conditions of the collaborative robot.                                                                                                                                                                                                                                                                  |
|  ![](../../_assets/2.png) | <p>Select the Safety Functions tab, and view the statuses of the safety functions.</p><ul><li><strong>OFF</strong>: Safety space disabled </li><li><strong>SAFE</strong>: Safety function observed</li><li><strong>UNSAFE</strong>: Safety function violated</li><li><strong>ERROR</strong>: SCM status error</li></ul> |
| ![](../../_assets/3.png)  | <ul><li><strong>[I/O]</strong>: You can view the statuses of the safety I/Os.</li><li><strong>[Status Recovery]</strong>: In case of safety violations during monitoring, you can clear errors and recover the status.</li></ul>                                                                                        |

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/1-robot-limit-parameter-monitoring.md)
# 1.10.1 Robot limiting parameter monitoring

Select the **\[Robot limit]** tab of **\[Configure > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 5: Cobot Safety Status]** to view the statuses of the robot limiting functions.

![Figure 13 Safety conditions of the collaborative robot: Robot limiting](<../../_assets/image_40.png>)

*   **\[Status]**: You can view the safety conditions.

    You can monitor the statuses of the safety functions of the collaborative robot. In a normal condition, Normal will be displayed. If an error or violation of a safety function occurs, the pertaining error code will be displayed.


* You can view the statuses of the robot limiting functions.
  * **\[TCP position]**: This indicates the statuses of the Cartesian spaces (nos. 1–12) and whether a TCP position violation has occurred during the monitoring.
  * **\[TCP speed]**: This indicates whether a TCP speed violation has occurred during the monitoring.
  * **\[TCP force]**: This indicates whether a TCP force violation has occurred during the monitoring.
  * **\[TCP orientation]**: This indicates whether a TCP orientation violation has occurred during the monitoring.
  * **\[Power]**: This indicates whether a power violation has occurred during the monitoring.
  * **\[Momentum]**: This indicates whether a momentum violation has occurred during the monitoring.
  * **\[Collision]**: This indicates whether a collision has been detected during the monitoring.
  * **\[SOS]** (Safe operating stop monitoring): This indicates whether an SOS violation has occurred during the monitoring.

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/2-joint-limit-function-monitoring.md)
# 1.10.2Joint limiting function monitoring

Select the **\[Joint limit]** tab of **\[Configure > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 5: Cobot Safety Status]** to view the statuses of the joint limiting functions.

![Figure 14 Safety conditions of the collaborative robot: Joint limiting](<../../_assets/image_38.png>)

*   **\[Status]**: You can view the safety conditions.

    You can monitor the statuses of the safety functions of the collaborative robot. In a normal condition, Normal will be displayed. If an error or violation of a safety function occurs, the pertaining error code will be displayed.


* You can view the statuses of the joint limiting functions.
  * **\[Position]**: This indicates whether an axial joint position violation has occurred during the monitoring.
  * **\[Speed]**: This indicates whether an axial joint speed violation has occurred during the monitoring.
  * **\[Torque]**: This indicates whether an axial joint torque violation has occurred during the monitoring.

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/3-scm-board-status-monitoring.md)
# 1.10.3 SCM board status monitoring

Select the **\[SCM Status]** tab of **\[Configure > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 5: Cobot Safety Status]** to view the status of the SCM board.

![Figure 15 Safety conditions of the collaborative robot: SCM status](<../../_assets/image_19.png>)

*   **\[Status]**: You can view the safety conditions.

    You can monitor the statuses of the safety functions of the collaborative robot. In a normal condition, Normal will be displayed. If an error or violation of a safety function occurs, the pertaining error code will be displayed.


* You can view the status of the SCM board.
  *   **\[Main]**: This is a status display of the dual MCUs (MCU A, MCU B).

      POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[Encoder]**: This is a status display of the axial dual encoders (Normal, Error, Off).
  * **\[Joint torque sensor]**: This is a status display of the axial dual JTSs (Normal, Error, Off).

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/4-safety-io-status-monitoring.md)
# 1.10.4 Safety I/O status monitoring

Select the **\[I/O]** button at the right side of the window of **\[Configure > 4: Application parameter > 21: Cobot Setup > 1: Cobot Safety Function > 5: Cobot Safety Status]** to view the statuses of the safety I/Os.

![Figure 16 Safety conditions of the collaborative robot: Safety I/O](<../../_assets/image_25.png>)

* **\[Input signal assignment]**: This displays the statuses of assignment and activation (On/Off) of the input signals (nos. 11–14)
* **\[Output signal assignment]**: This displays the statuses of assignment and activation (On/Off) of the output signals (nos. 11–14)

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/5-recovery-mode/README.md)
# 1.10.5 Recovery mode

In recovery mode, you can clear errors that occur because of the safety function violations during monitoring. Because position detection is temporarily disabled in recovery mode, you can drive the robot and adjust its angle and position without violating the safety functions.

If a safety function monitoring is violated, the robot will activate a safety stop immediately and stop moving. In addition, the safety stop notice window will appear on the operating program window.

1 .Set the operating mode to the manual mode.

2\. On the safety stop notice window, click the **\[ENTER]** button. Then, the safety condition monitoring window will appear.

![](../../../_assets/image66.jpeg)

3\. Click the **\[Status Recovery]** button. Then, the **\[Status Recovery]** button will turn green, and the system will enter recovery mode.

4\. In recovery mode, adjust the robot’s angle and position to clear errors.



![](<../../../_assets/image_13.png>)

5\. After the recovery is completed, click the **\[Status Recovery]** button. Then, the **\[Status Recovery]** will turn into the previous color, and the recovery mode will be cleared.

* You can also clear the recovery mode by clicking the **\[X]** button at the upper-right corner of the safety condition monitoring window.

{% hint style="warning" %}
**\[Caution]**: After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/5-recovery-mode/1-recovery-robot-position-violation.md)
# 1.10.5.1 Recovery in case of robot position violations

Robot position violations are situations in which the robot’s position exceeds a safety space, and these include TCP position, TCP orientation, and joint monitoring violations. When a robot position violation occurs, you can only clear the error by moving the robot’s physical position.

1.  On the safety condition monitoring window, click the \[Status Recovery] button to enter recovery mode.


2.  Turn on the motor by using the enabling switch on the teach pendant.


3.  Use the teaching device to move the robot back to a safety space.


4.  On the safety condition monitoring window, check if the status of each space is displayed as SAFE.


5. After the recovery is completed, click the \[Status Recovery] button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**: After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/5-recovery-mode/2-recovery-robot-speed-violation.md)
# 1.10.5.2 Recovery in case of robot speed violations

Robot speed violations are situations in which the robot’s speed exceeds a safety limit, and these include TCP speed, joint speed, power, and momentum monitoring violations. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1.  &#x20;**** On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.


2.  On the safety condition monitoring window, check if the status of each space is displayed as SAFE.


3. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the error, make sure to recheck all speed-related safety parameters and the speed displayed on the operating program.
* After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/5-recovery-mode/3-recovery-robot-force-violation.md)
# 1.10.5.3 Recovery in case of robot force violations

Robot force violations are situations in which external force is applied on the robot or in which the amount of the force used by the robot internally exceeds a safety limit, and these include TCP force, collision detection, joint torque, power, and momentum monitoring violations. You can clear errors depending on the causes of the violations.

#### <mark style="color:green;">Violation caused by external force applied on the robot</mark>&#xD;

1. Remove the external factor that is applying force on the robot.
2. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
3. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
4. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**: After clearing the recovery mode, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}

#### &#xD;<mark style="color:green;">Violation caused by the amount of force used by the robot internally exceeding a safety limit</mark>&#xD;

1. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
2. &#x20;**** Turn on the motor using the enabling switch on the teach pendant.
3. Use the teaching device to move the robot to a low-load posture.
4. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
5. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the recovery mode, recheck the robot’s safety condition setting, tool data, the teaching position of the operating program, and the torque sensor offset.
* If the error is not cleared, check the tool data, tool number, safety condition setting, and torque sensor offset, and repeat procedures 1 through 5.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-10-safety-condition-monitoring/5-recovery-mode/4-recovery-sos-violation.md)
# 1.10.5.4 Recovery in cases of safe operating stop (SOS) violations

SOS violations are situations in which the robot’s motion is detected while its motor is on and is supposed to be in a stop state. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1. Remove the external factor that is applying force on the robot.
2. On the safety condition monitoring window, click the **\[Status Recovery]** button to enter recovery mode.
3. On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.
4. After the recovery is completed, click the **\[Status Recovery]** button to clear the recovery mode.

{% hint style="warning" %}
**\[Caution]**

* After clearing the recovery mode, turn on the motor in the automatic mode and check if the error does not persist.
* If the same error recurs, check the driving module of the pertaining axis.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-11-cobot-collision-detection-mode/README.md)
# 1.11 Collaborative robot collision detection mode

The collision detection function serves as a safety mechanism when the robot operates under abnormal conditions or exhibits irregular behavior. You can configure the detection mode and run auto-tuning to automatically set the optimal collision detection sensitivity for the current task.

Configuration methods include controller settings and robot language commands:
1. Controller settings: Basic settings that are always applied (default).
2. Robot language commands: Robot language commands are used to configure whether collision detection is active for specific segments during robot program execution.

[__SOURCE](1-cobot-safety-function/1-11-cobot-collision-detection-mode/1-cobot-collision-detection-setup.md)
# 1.11.1 Collision Detection Controller Settings

1.  Please set the driving mode to manual.


2.  **\[system]** Button > **\[11: Cobot System ]** > **\[Collision Detection]** Please touch the menu.


3. After configuring the settings and options for the collaborative robot's collision detection function, touch the **\[OK]**  button.
![](../../_assets/image64.jpg)

* **\[Collision detection]**: Configure whether to use the collision detection function.
* **\[Body parts for collision detection]**: Select the body part to apply the robot's maximum speed capable of guaranteeing minimum safety against injury upon collision detection.
* **\[Collision detection reaction]**: Select whether to execute an avoidance maneuver after a collision is detected.


{% hint style="warning" %}
**\[Warning]**

* If there is a significant discrepancy between the tool data and actual values, collisions may be incorrectly detected. Please accurately configure tool-related information, such as length, weight, and the center of gravity. Additionally, be sure to verify the robot's installation angle and the direction of gravity. If false detections persist despite accurate tool data configuration, please inspect the encoders and acceleration sensors.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-11-cobot-collision-detection-mode/2-cobot-collision-detection-roblang.md)
# 1.11.2 Collision-detection robot command(cobot_coldet)

### explanation

Configure whether the collaborative robot performs collision detection.

Collision detection is handled by the Hi7 controller.

### grammar

&lt;cobot_coldet&gt;.on </br>
&lt;cobot_coldet&gt;.off 


### example

cobot_coldet.on
cobot_coldet.off
```
[__SOURCE](1-cobot-safety-function/1-11-cobot-collision-detection-mode/3-cobot-collision-detection-autotune.md)
# 1.11.3 Collaborative Robot Collision Detection Auto-Tuning Mode

1.  Please set the driving mode to manual.


2.  **\[system]**  > **\[11: Cobot System ]** > **\[5: Collision Dectection Threshold]** Please touch the menu.


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

[__SOURCE](1-cobot-safety-function/1-12-cobot-direct-teaching-mode/README.md)
# 1.12 Collaborative robot direct teaching mode

Direct teaching is an intuitive method that allows users without specialized robot programming knowledge to teach a robot desired movements by manually manipulating it. Instead of using a complex teach pendant, the operator directly guides the robot's end-effector to define the work path and positions.

Configuration methods include controller settings and cockpit button settings:
1. Controller settings: Basic settings applied by default.
2. Cockpit button: Activates the direct teaching mode configured on the robot's teach pendant (TP).

[__SOURCE](1-cobot-safety-function/1-12-cobot-direct-teaching-mode/1-cobot-direct-teaching-setup.md)
# 1.12.1 Direct Teaching Controller Configuration

1.  Please set the driving mode to manual.


2.  **\[System]** > **\[11: Cbbot System]** > **\[Direct Teaching]** Please touch the menu.


3. After configuring the settings and options for the collaborative robot's direct teaching function, touch the **[OK]** button.

![](../../_assets/image57.png)

* **Direct teaching On**: Direct teaching mode activates immediately upon motor-on (SHIFT + MOT. ON + Enable Switch). The motor remains on and direct teaching operates only while the Enable Switch is pressed. To switch the robot back to Jog or Auto mode, you must disable the "Direct teaching On" setting.
* **Constraint motion**: Determines the default mode when direct teaching is executed. If 'None' is selected, you cannot switch to another mode; however, switching between other modes is possible while direct teaching is in progress.

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

[__SOURCE](1-cobot-safety-function/1-13-simple-encoder-offset/README.md)
# 1.13 Simple Encoder Offset

This section describes the simple encoder offset mastering function using a device built into the robot.
This function consists of two main parts:
- Simple Mastering Position Setting
- Simple mastering

[__SOURCE](1-cobot-safety-function/1-13-simple-encoder-offset/1-update-mastering-position.md)
# 1.13.1 Simple Mastering Position Setting

The robot requires mastering at a specific position; this section explains how to designate that position. Since the robot moves when the mastering position is set, care must be taken to avoid collisions with people or objects in the vicinity. Note that while there are various possible mastering positions, the system selects a position close to the robot's current posture.

-  **\[system]** > **\[11: Cobot System ]** > **\[11: Simple Encoder Offest ]** Please touch the menu.
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
[__SOURCE](1-cobot-safety-function/1-13-simple-encoder-offset/2-update-encoder-offset.md)
# 1.13.2 Simple Mastering

This section explains how to initialize (master) the encoder offset after the robot moves to the designated mastering position. Since the robot moves to the mastering position, take care to avoid collisions with people or objects in the surrounding area.

- **\[system]** > **\[11: Cobot System ]** > **\[11: Simple Encoder Offest ]** Please touch the menu.
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
[__SOURCE](attachment/README.md)
# Attachment


[__SOURCE](attachment/rules-criteria-and-public-notice.md)
# The Rules on the Criteria for Occupational Safety and Health, and the Public Notice of Safety Inspec

{% embed url="https://hyundai-robotics.gitbook.io/rules-on-occupational-safety-and-health-standards/v/rules-english" %}

[__SOURCE](warranty.md)
# Warranty

{% embed url="https://hyundai-robotics.gitbook.io/quality-assurance/v/qa-english" %}
