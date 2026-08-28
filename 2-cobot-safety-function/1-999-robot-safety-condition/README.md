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
