# 1.12.1 협동로봇 직접교시 제어기 설정

1.  운전 방식을 수동 모드로 설정하십시오.


2.  **\[설정]** 버튼 > **\[4: 응용 파라미터 > 21: 협동로봇 설정 > 직접교시]** 메뉴를 터치하십시오.


3. 협동로봇의 직접교시 기능의 사용 여부와 옵션을 설정한 후 **\[OK]** 버튼을 터치하십시오.

![](../../_assets/image57.png)

* **직접 교시(Direct teaching On/ Off)**: 직접교시 기능의 사용여부를 결정합니다.
* **직접 교시 상시 활성화(Direct teaching always-on mode)**: 모터온 시 바로 직접교시로 동작합니다.(SHIFT + MOT. ON + deadman switch)
* **구속 모션(Constraint motion)**: '직접 교시 상시 활성화'나 '콕핏 M 버튼 '가 직접교시 모드에서 버튼 클릭시 실행되는 모드를 결정합니다. 
![](../../_assets/image57.png) 
* **콕핏 설정(Cockpit setting)**: Cockpit버튼의 모드를 결정합니다. 각 '콕핏 A, B, C 버튼'은 아래의 보기중 하나의 기능을 가질 수 있습니다.
'XYZ' = X, Y, Z 제외 cartesian 구속 모션 실행합니다.
'XY'  = X, Y 제외 cartesian 구속 모션 실행합니다.
'X'   = X 제외 cartesian 구속 모션 실행합니다.
'Y'   = Y 제외 cartesian 구속 모션 실행합니다.
'Z'   = Z 제외 cartesian 구속 모션 실행합니다.
'Rx'  = Rx 제외 cartesian 구속 모션 실행합니다.
'Ry'  = Ry 제외 cartesian 구속 모션 실행합니다.
'Rz'  = Rz 제외 cartesian 구속 모션 실행합니다.
'None'= 눌러도 변화가 없습니다.
'콕핏 M 버튼' 다른 버튼과는 다른 보기를 갖습니다.
'포즈 저장' = 로봇의 현재 위치를 저장합니다.
'직접 교시' = 직접교시를 실행합니다. 실행 모드는 '구속 모션'에서 설정한 모드입니다.
* **축 잠금(Axis locked)**:조인트 모션에서 특정 축의 가동을 막을 수 있음 - 활성화시 축 구동

{% hint style="warning" %}
**\[주의]**

* 툴 데이터가 실제 값과 오차가 클 경우 직접교시가 실행되지 않을 수 있습니다. 직접교시가 계속 실행되지 않을 경우 로봇을 멈추고 툴 데이터 입력값을 확인하기 바랍니다.
* 'Direct teaching always-on mode'이 On인 경우 motor on/deadman switch/shift를 동시에 눌러주시기 바랍니다.
* 'Direct teaching always-on mode'를 이용하여 직접교시를 실행한 경우 motor off를 원하시면 'Direct teaching always-on mode' 버튼을 off로 변경하시면 됩니다. 
* 직접교시 실행시 로봇 주변 사물이나 사람을 확인후 동작해주시기 바랍니다.
* 두개 이상의 버튼이 동시에 눌러질 경우 처음 누른 버튼만 인식합니다.
* 
{% endhint %}
