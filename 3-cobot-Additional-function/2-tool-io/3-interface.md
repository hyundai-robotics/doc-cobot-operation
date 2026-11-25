### 3.2.3 Tool IO Interface

This function configures the interface of the collaborative robot's Tool IO system device.

<br>

{% hint style="info" %}
   - If you are using Modbus RTU communication with the Tool IO device, please refer to the following manual.

   - "[Hi7 Controller Function Manual - Modbus](https://hrbook-hrc.web.app/#/view/doc-modbus/en/4-modbus-master/1-roblang?cont_model=Hi7)"
{% endhint %}


**1. Touch the menu to enter the settings screen.**

<br>

**\[System > 11: Cobot System > 2: Tool IO Settings > 2: Tool IO Interface Settings]**

<br>

![[Figure 3.2.3-1 Tool IO Interface Settings]](<../../_assets/3-cobot-Additional-function/2-tool-io/3-interface/image1.png>) 

<br>

{% hint style="info" %}
   [Output Power Settings]   
   - 24V Power: External output power setting   
      - OFF   
      - 24V   
   - I/O Type: Tool IO digital input/output type setting   
      - PNP   
      - NPN   

   [Serial Communication Settings]   
   - Configures the serial communication parameters of the Tool IO system RS485 connector.   

   - Serial: Enable/disable communication   
      - OFF   
      - ON   
   - Baud Rate: Serial communication speed setting   
      - 9600bps ~ 2.5Mbps   
   - Parity Bit: Parity bit setting   
      - None   
      - Odd   
      - Even   
   - Stop Bit: Stop bit setting   
      - 1 Bit   
      - 2 Bit   
   - Data Length: Data bit length setting   
      - 7 Bit   
      - 8 Bit   
      
{% endhint %}

<br>

![[Figure 3.2.3-2 Tool IO Interface Settings]](<../../_assets/3-cobot-Additional-function/2-tool-io/3-interface/image2.png>) 

<br>

{% hint style="info" %}
   [Power Status]   
   - 24V Power: ON/OFF operation status of external output power   
   - I/O Type: Currently applied I/O type   
   - Voltage 24V: External output voltage measurement value   
   - Current 24V: External output current measurement value   

   [Serial Status]   
   - Serial Operation: ON/OFF operation status of serial communication   
   - Baud Rate: Currently applied baud rate   
   - Parity Bit: Currently applied parity bit   
   - Stop Bit: Currently applied stop bit   
   - Data Length: Currently applied data length   
      
{% endhint %}
