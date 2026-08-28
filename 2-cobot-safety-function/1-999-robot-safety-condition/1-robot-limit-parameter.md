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
