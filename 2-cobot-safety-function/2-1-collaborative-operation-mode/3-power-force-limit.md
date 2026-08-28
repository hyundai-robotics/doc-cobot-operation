# 2.1.3 Power and force limiting


In the event of contact, the system limits the impact force exerted on the human body. Collision detection and TCP force limiting functions serve to restrict the impact on the operator during contact between the operator and the robot.

The collision detection function identifies collisions based on user-defined contact zones, while the TCP force limiting function restricts the external force (N) applied to the TCP. Additionally, the robot's power output can be limited by configuring parameters for power (W) and momentum (kg·m/s).

* For details regarding power and momentum monitoring and power limiting when configuring robot safety conditions, please refer to ([3.3.2 Robot Monitoring Function](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/2-robot-safety-condition/README?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model} )) in ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
* For details on the collision detection function, please refer to **(2.2 Collaborative robot collision detection mode)**.

