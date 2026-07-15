# 1.3.3 Collaborative Robot Collision Detection Auto-Tuning Mode

1.  Please set the driving mode to manual.

2.  **\[system]** Button > **\[11: Cobot System  > Collision Dectection Threshold]** Please touch the menu.

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
{% hint style="warning" %}
**\[warning]**
* Veillez à ce que le robot ne subisse aucun choc extérieur pendant l'exécution de la fonction de réglage automatique (auto-tuning). Si un choc extérieur survient en cours d'exécution, veuillez réinitialiser et relancer le processus de réglage automatique. 
Si le nombre d'itérations de réglage automatique est trop faible, le processus risque de s'achever avant que l'optimisation ne soit complète, ce qui peut entraîner de fréquentes fausses détections ; à l'inverse, si ce nombre est trop élevé, le processus peut prendre un temps excessif, selon la durée de la tâche d'exécution. Nous recommandons de régler le nombre d'itérations entre 100 et 200 pour une tâche d'une durée d'exécution d'une minute. 
Veuillez noter que cette fonction ne s'active qu'en mode Auto ; en mode Manuel, la fonction de détection de collision utilise les paramètres par défaut définis en usine.
{% endhint %}