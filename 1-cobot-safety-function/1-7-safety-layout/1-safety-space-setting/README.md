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
