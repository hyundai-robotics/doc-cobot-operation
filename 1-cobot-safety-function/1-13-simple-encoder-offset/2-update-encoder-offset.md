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
*  A mastering position must be registered to use the simple Mastering function.
* Touching the 'Reset All' button without moving to the mastering position will not reset the encoder offset.
* You must save the settings after performing the encoder offset to update it.
* Frequent use of the simple Encoder Offset function degrades mastering performance; please use it only when necessary.
{% endhint %}    

{% hint style="warning" %}
**\[Warning]**
* Une position de mastering doit être enregistrée pour utiliser la fonction de mastering simple.
* Appuyer sur le bouton « Réinitialiser tout » sans se placer au préalable sur la position de mastering ne réinitialisera pas le décalage de l'encodeur.
* Vous devez enregistrer les paramètres après avoir effectué le réglage du décalage de l'encodeur pour le mettre à jour.
* Une utilisation fréquente de la fonction simple de décalage de l'encodeur dégrade les performances de mastering ; veuillez ne l'utiliser qu'en cas de nécessité.
{% endhint %}    