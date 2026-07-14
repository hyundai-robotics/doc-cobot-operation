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
{% hint style="warning" %}
**\[warning]**

* L'apprentissage direct peut ne pas s'exécuter en cas d'écart important entre les données de l'outil et les valeurs réelles. Si l'apprentissage direct ne se lance pas, veuillez arrêter le robot et vérifier les valeurs saisies pour les données de l'outil.
* Pour lancer l'apprentissage direct, appuyez simultanément sur le bouton « Motor On » (Moteur activé), le dispositif d'homme mort (Enable Switch) et la touche « Shift ».
* Vous devez maintenir le dispositif d'homme mort enfoncé après la mise en marche du moteur pour conserver le mode d'apprentissage direct.
* L'apprentissage direct s'arrête si vous désactivez la fonction (« Direct teaching On ») ou si vous relâchez le dispositif d'homme mort alors que la fonction est active.
* Veuillez vérifier la présence d'objets ou de personnes à proximité avant de faire fonctionner le robot en mode d'apprentissage direct.
* Si plusieurs boutons sont enfoncés simultanément, seul le premier bouton actionné est pris en compte.
* Si vous tentez de déplacer le robot automatiquement à l'aide de la TP (console d'apprentissage) pendant l'apprentissage direct, le robot s'arrêtera immédiatement. Cela constitue un arrêt d'urgence et présente un risque pour la sécurité.
{% endhint %}