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
