# 1.6.2 LED Settings

This indicates the LED brightness settings and the meaning of each LED color. The colors cannot be changed; only the brightness is adjustable.

- `[F2: system] - 11: Cobot System- Cobot General Settings` Tap the menu.
- Enter the LED settings and click "Apply to All" to save.
    ![](../../_assets/image62.png) 
    - Base LED Brightness (%): Adjusts the brightness of the LED mounted on Axis 1. (Default: 10%)
    - Flange LED Brightness (%): Adjusts the brightness of the LED mounted on Axis 6. (Default: 10%)
    - Settings are saved only after clicking "Apply All" and entering the correct password. 

    

{% hint style="warning" %}
**\[warning]**
* Keeping the LED on at 100% continuously may result in performance degradation.

{% endhint %}

The robot status by LED color is as follows:
<table>
  <thead>
    <tr>
      <th style="text-align: center;">Color</th>
      <th style="text-align: center;">Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center;">RED</td>
      <td>Error, emergency stop, or robot stop by radar</td>
    </tr>
    <tr>
      <td style="text-align: center;">Green</td>
      <td>Auto mode</td>
    </tr>
    <tr>
      <td style="text-align: center;">Blue</td>
      <td>Manual mode(motor on)</td>
    </tr>
    <tr>
      <td style="text-align: center;">White</td>
      <td>Manual mode(motor off)</td>
    </tr>
    <tr>
      <td style="text-align: center;">Blue blink</td>
      <td>Direct teaching mode</td>
    </tr>
    <tr>
      <td style="text-align: center;">Yellow blink</td>
      <td>Warning, robot deceleration by radar</td>
    </tr>
  </tbody>
</table>