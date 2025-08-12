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
