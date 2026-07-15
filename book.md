
[__SOURCE](README.md)
# 협동로봇 안전 기능 설명서

{% hint style="warning" %}
본 제품 설명서에서 제공되는 정보는 현대로보틱스의 자산입니다.

현대로보틱스의 서면에 의한 동의 없이 전부 또는 일부를 무단 전재 및 재배포할 수 없으며, 제3자에게 제공되거나 다른 목적에 사용할 수 없습니다.



본 설명서는 사전 예고 없이 변경될 수 있습니다.



**Copyright ⓒ 2020 by Hyundai Robotics Co., Ltd**
{% endhint %}

[__SOURCE](0-about-this-manual/README.md)
# 이 설명서에 대하여

[__SOURCE](0-about-this-manual/precautions.md)
# 사전 주의사항

{% include file="ko/precautions.md" %}

[__SOURCE](0-about-this-manual/safety-notice.md)
# 안전 주의 사항

{% include file="ko/safety-notice.md" %}

[__SOURCE](1-cobot-safety-function/README.md)
# 1. 협동로봇 안전 기능


[__SOURCE](1-cobot-safety-function/1-1-description-term.md)
# 1.1 용어 설명

### <mark style="color:green;">충돌감지</mark>&#xD;

로봇이 동작 중 외부로부터 충격이 가해져 설정된 임계 값을 초과하는 경우 사용자 안전을 위해 정지합니다.

*   **임계값**

    외부로부터 충격이 가해졌다고 판단되는 기준 값입니다.

### <mark style="color:green;">직접교시</mark>&#xD;

작업자가 로봇을 손으로 직접 움직여 원하는 경로와 자세로 이동하여 교시하는 방식입니다.

*   **구속 모션**

    협동로봇의 직접교시 기능 중 하나로, 로봇이 직교 좌표계의 특정 방향이나 특정 축으로만 움직이도록 제한한 상태에서 교시하는 기능입니다.

*   **콕핏**

    협동로봇을 UI를 사용하지 않은 상태에서 조작하기 위한 버튼 

*   **cartesian**

    직교좌표계(직각좌표계)를 의미하는 용어, X, Y, Z 좌표를 기준으로 로봇의 위치와 움직임을 표현하는 방식을 의미합니다.

*   **Enable Switch**

    인에이블링 스위치를 의미합니다. 수동 모드에서 티치 펜던트로 로봇 조작 시, 안전 스위치로 사용합니다.
    1단, 3단: 로봇 운전이 정지됩니다. 3단일 경우, 2단을 거치지 않고 1단으로 복귀합니다.
    2단: 로봇을 조작할 수 있습니다.

  

### <mark style="color:green;">마스터링</mark>&#xD;

로봇의 실제 관절 각도와 제어기가 인식하는 관절 각도를 일치시키는 작업을 의미합니다.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/README.md)
# 1.2 협동 운전 모드

ISO 10218-1과 ISO/TS 15066에서는 작업자가 위험에 노출되지 않고 안전하게 작업할 수 있도록 4 개의 운전 모드에 대해 설명하고 있습니다. 협동 운전은 이 중 최소 한 가지 요구 사항을 충족해야 하고 운전 중에는 반드시 협동 운전 중임을 시각적으로 표시하여 알려야 합니다.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/1-safety-rated-monitored-stop.md)
# 1.2.1 안전 정격 감시 정지

사람이 작업 공간 내 진입 시 로봇의 작동이 정지합니다. 외부 감시 장치를 설치하고 이를 안전 제어 모듈(SCM: Safety Control Module)에 연결하거나 로봇에 설치된 레이더 센서를 사용하십시오.

* 외부 장치에 안전 입력을 연결할 경우에는 안전 I/O신호 설정에서 정지 방법(정지 0, 정지 1, 정지 2)을 설정해야 합니다.
* 안전 가드 및 외부 비상정지를 연결한 경우에는 국제 또는 해당 지역 규제에 부합하는 정지 방법을 설정해야 합니다.

관련 기능 설정에 대한 참조 정보는 다음과 같습니다.

* 레이더 모듈 설정에 대한 자세한 내용은 ([사용자 설명서](https://github.com/hyundai-robotics/doc-Object-Detection-System#?cont_model=${cont_model})) 내 ([8.1 구성 절차]( ))를 참조하십시오.
* 안전 I/O 신호 설정에 대한 자세한 내용은 ([Hi7 제어기 기능설명서 - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/README?cont_model=${cont_model})) 내 ([3.3.4 안전 입출력](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/3-safety-function/3-safety-function/4-safety-io/README?cont_model=Hi7?cont_model=${cont_model}))를 참조하십시오.
* 안전 정지 기능 설정에 대한 자세한 내용은 ([Hi7 제어기 기능설명서 - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/README?cont_model=${cont_model})) 내 ([3.3.1.2 정지 설정](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/3-safety-function/3-safety-function/1-general-condition/2-safe-stop?cont_model=Hi7?cont_model=${cont_model}))을 참조하십시오.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/2-speed-separation-monitoring.md)
# 1.2.2 속도 및 위치 감시

로봇은 지정된 거리 및 속도 내에서 작동합니다.

속도 및 위치 감시 모드는 사람의 위치 및 속도를 감지할 수 있는 센서를 이용해 로봇과 사람 간의 거리에 따라 로봇의 구동 속도를 제어하는 모드로, 거리를 감지하는 외부 센서나 로봇에 설치된 레이더 센서를 사용할 수 있습니다.

속도 및 위치 감시 모드 사용을 위한 참조 정보는 다음과 같습니다.

* 레이더 모듈 설정에 대한 자세한 내용은 ([사용자 설명서](https://github.com/hyundai-robotics/doc-Object-Detection-System#?cont_model=${cont_model})) 내 ([8.1 구성 절차]( ))를 참조하십시오.
* 로봇 안전 조건 설정에 대한 자세한 내용은 ([Hi7 제어기 기능설명서 - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/README?cont_model=${cont_model})) 내 ([3.3.2.6 Re plan 설정](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/3-safety-function/3-safety-function/2-robot-safety-condition/6-re-plan?cont_model=Hi7?cont_model=${cont_model}))을 참조하십시오.
* 안전 I/O 신호 설정에 대한 자세한 내용은 ([Hi7 제어기 기능설명서 - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/README?cont_model=${cont_model})) 내 ([3.3.4 안전 입출력](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/3-safety-function/3-safety-function/4-safety-io/README?cont_model=Hi7?cont_model=${cont_model}))를 참조하십시오.

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/3-power-force-limit.md)
# 1.2.3 동력 및 힘 제한

접촉 사고 발생 시, 인체에 가해지는 충격을 제한합니다. 충돌 감지 기능 및 TCP 힘 제한 기능을 통해 작업자와 로봇 간의 접촉 사고 발생 시 작업자의 신체에 가해지는 충격을 제한할 수 있습니다.

충돌 감지 기능의 경우 충돌 부위를 설정하여 충돌을 감지하고, TCP 힘 제한의 경우 TCP에 가해지는 외부 힘(N)을 제한합니다. 또한 파워(W)와 모멘텀(kg·m/s)을 설정하여 로봇의 동력을 제한할 수 있습니다.

* 로봇 안전 조건 설정중 파워와 모멘텀 감시 및 동력 제한에 대한 자세한 내용은 ([Hi7 제어기 기능설명서 - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/README?cont_model=${cont_model} )) 내 ([3.3.2 로봇 감시 기능](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/ko/3-safety-function/3-safety-function/2-robot-safety-condition/README?cont_model=Hi7?cont_model=${cont_model} ))을 참조하십시오.
* 충돌 감지 기능에 대한 자세한 내용은 **(1.3 협동로봇 충돌감지 모드)** 를 참조하십시오

[__SOURCE](1-cobot-safety-function/1-2-collaborative-operation-mode/4-hand-guid.md)
# 1.2.4 핸드가이드

작업자가 로봇을 손으로 직접 움직여 위치나 경로를 교시할 수 있도록 하는 수동 조작 모드입니다. 로봇의 힘 제어 기능을 이용해 사람이 가하는 힘을 감지하고, 그 방향으로 로봇이 부드럽게 움직입니다. 복잡한 프로그래밍 없이도 작업을 설정할 수 있습니다.

하기에 서술할 내용에서 핸드가이드와 협동로봇의 직접교시는 동일한 뜻으로 사용됩니다.

* 핸드 가이드에 대한 자세한 내용은 **(1.4 협동로봇 직접교시 모드)** 를 참조하십시오

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/README.md)
# 1.3 협동로봇 충돌감지 모드

로봇이 비정상적인 조건에서 동작하게 되거나 이상 동작하게 될 때의 안전 장치로 충돌감지 기능이 있습니다. 감지 모드를 설정하고 자동 튜닝을 실행하여 현재 작업에 맞는 최적 충돌 감지 민감도를 자동 설정할 수 있습니다.

설정 방식으로는 제어기 설정과 로봇 언어 명령문 설정이 있습니다. 
1. 제어기 설정: 항상 적용되는 기본적인 설정 (default)
2. 로봇 언어 명령문: 로봇 프로그램 동작 시 구간 별로 충돌감지 실행 여부를 설정하기 위하여 로봇 언어 명령문을 사용. 

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/1-cobot-collision-detection-setup.md)
# 1.3.1 협동로봇 충돌감지 제어기 설정

1.  운전 방식을 수동 모드로 설정하십시오.

2.  **\[시스템]** 버튼 > **\[11: 협동 로봇 시스템 > 충돌감지]** 메뉴를 터치하십시오.

3. 협동로봇의 충돌감지 기능의 사용 여부와 옵션을 설정한 후 **\[OK]** 버튼을 터치하십시오.

![](../../_assets/image64.jpg)

* **\[감지]**: 충돌감지 기능의 사용 여부를 설정합니다.
* **\[충돌 부위]**: 충돌감지 시 상해 최소 안전 보장 가능한 로봇의 최대속도를 적용하기 위한 신체 부위를 선택합니다.
* **\[충돌 감지 리액션]**: 충돌 감지 후 회피 동작 실행 여부를 선택합니다.


{% hint style="warning" %}
**\[주의]**

* 툴 데이터가 실제 값과 오차가 클 경우 충돌을 잘못 감지할 수 있습니다. 길이나 무게, 무게 중심 등의 툴 관련 정보를 정확하게 설정하십시오. 또한 로봇의 설치 각도 및 중력 방향을 반드시 확인하십시오. 툴 데이터를 정확히 설정해도 오감지가 발생한다면 엔코더 및 기속도 센서를 점검하십시오.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/2-cobot-collision-detection-roblang.md)
# 1.3.2 충돌감지 로봇 명령어(cobot_coldet)

### 설명

협동로봇의 충돌감지 수행 여부를 설정합니다.

해당 충돌감지 기능은 Hi7 제어기에서 감지하게 됩니다. 

### 문법

&lt;cobot_coldet&gt;.on </br>
&lt;cobot_coldet&gt;.off 


### 사용 예

cobot_coldet.on </br>
cobot_coldet.off
[__SOURCE](1-cobot-safety-function/1-3-cobot-collision-detection-mode/3-cobot-collision-detection-autotune.md)
# 1.3.3 협동로봇 충돌감지 자동 튜닝 모드

1.  운전 방식을 수동 모드로 설정하십시오.


2.  **\[시스템]** 버튼 > **\[11: 협동 로봇 시스템 > 충돌감지 임계값]** 메뉴를 터치하십시오.


3.  **\[임계 값 초기화]** 버튼을 터치하십시오.

4. 협동로봇의 충돌감지 임계값 자동 튜닝 기능의 실행 여부와 실행 횟수를 설정한 후 **\[저장]** 버튼을 터치하십시오.

![](../../_assets/image65.jpg)

* **\[자동 튜닝]**: 충돌감지 자동 튜닝 기능 실행 여부를 설정합니다.
* **\[튜닝 횟수]**: 충돌감지 자동 튜닝을 수행할 job 실행 횟수를 설정합니다.
* **\[임계값 초기화]**: 충돌 감지 임계값을 초기화 합니다.
* **\[공장값 초기화]**: 충돌 감지 임계값을 공장 출하 값으로 초기화 합니다.


{% hint style="warning" %}
**\[주의]**

* 자동 튜닝 기능 수행 중에는 로봇에 외부적 충격이 가해지지 않도록 주의하십시오. 만약에 기능 실행 중 외부 충격이 가해졌다면 자동 
튜닝을 초기화하여 재실행해주십시오. 
자동 튜닝 횟수를 너무 작게 설정하면 최적화가 완료되기 전 자동 튜닝이 완료되어 오감지가 다발 발생할 수 있으며 반대로 자동 튜닝
횟수를 너무 크게 설정하면 실행 job의 시간에 따라 너무 오랜 시간 자동 튜닝을 실행하여 완료가 늦어질 수 있습니다. 실행 시간이 1분인
job 기준으로 100 ~ 200회 사이로 설정하는 것을 권장합니다. 
이 기능은 자동 모드에 한정하여 수행하며 수동 모드에서는 공장 출하 값으로 충돌감지 기능이 수행됨을 참조 바랍니다. 
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-4-cobot-direct-teaching-mode/README.md)
# 1.4 협동로봇 직접교시 모드

로봇의 직접교시(Direct Teaching)는 로봇 프로그래밍에 대한 전문적인 지식이 없는 사용자도 로봇을 직접 움직여 원하는 동작을 가르칠 수 있는 직관적인 방식입니다. 이는 복잡한 티치 펜던트 조작 대신 작업자가 직접 로봇 팔 끝을 잡고 경로를 안내하여 작업 경로와 위치를 설정하는 것을 의미합니다.

설정 방식으로는 제어기 설정과 코핏 버튼 설정이 있습니다. 
1. 제어기 설정: 항상 적용되는 기본적인 설정 (default)
2. 콕핏 버튼: 로봇 TP에서 설정한 직접교시 모드를 실행 

[__SOURCE](1-cobot-safety-function/1-4-cobot-direct-teaching-mode/1-cobot-direct-teaching-setup.md)
# 1.4.1 협동로봇 직접교시 제어기 설정

1.  운전 방식을 수동 모드로 설정하십시오.


2.  **\[설정]** 버튼 > **\[11: 협동로봇 시스템 > 직접교시]** 메뉴를 터치하십시오.


3. 협동로봇의 직접교시 기능의 사용 여부와 옵션을 설정한 후 **\[OK]** 버튼을 터치하십시오.

![](../../_assets/image57.png)

* **직접 교시(Direct teaching On)**: 모터온 시 바로 직접교시로 동작합니다.(SHIFT + MOT. ON + Enable Switch) Enable Switch가 눌러져 있어야만 모터온이며, 직접교시가 구동된다. 다시 조그나 자동으로 로봇을 원할 경우 설정내 '직접교시 ON (Direct teaching On)'를 OFF 해야함 
* **구속 모션(Constraint motion)**: 직접교시가 실행될때 기본 모드를 결정합니다. '없음'을 선택했을 경우 FREE 모드로 실행 되며, 모터온 중 다른 모드로 바꾸지 못하지만 그 외 다른 모드에선 직접교시 실행 중 모드 변경이 가능합니다.

![](../../_assets/image60.png) 

4. 위 사진은 협동로봇 시리즈 HDC에 부착된 콕핏 버튼을 형상황한 그림입니다. 참고하여 아래 콕핏 설정을 읽어주시기 바랍니다.
* **콕핏 설정(Cockpit setting)**: 콕핏 버튼(Cockpit)의 모드를 결정합니다. 
- 각각의 '콕핏 A, B, C 버튼'은 아래의 보기중 하나의 기능을 가질 수 있습니다.
    - 'XYZ' = X, Y, Z 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'XY'  = X, Y 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능) 
    - 'X'   = X 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'Y'   = Y 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'Z'   = Z 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'Rx'  = Rx 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'Ry'  = Ry 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - 'Rz'  = Rz 제외 cartesian 구속 모션으로 직접교시 모드를 변경합니다.(직접교시 구속모션 중에만 가능)
    - '없음(None)'= 눌러도 변화가 없습니다.

- '콕핏 M 버튼'은 아래 보기와 같은 메뉴를 갖습니다.
    - '포즈 저장' = 로봇의 현재 위치를 현재 TP상 열려있는 잡파일에 기록합니다. 


* **자유 직접교시 축 활성화(Joint Direct Teaching Axis Activate)**:자율 직접교시 중 활성화시에만 선택한 축 구동가능

{% hint style="warning" %}
**\[주의]**

* 툴 데이터가 실제 값과 오차가 클 경우 직접교시가 실행되지 않을 수 있습니다. 직접교시가 계속 실행되지 않을 경우 로봇을 멈추고 툴 데이터 입력값을 확인하기 바랍니다.
* 직접교시를 실행하고 할때 motor on/Enable Switch/shift를 동시에 눌러주시기 바랍니다.
* 모터온 후 Enable Switch를 누르고 계셔야만 직접교시가 계속 실행됩니다.
* 직접교시 실행 중 'Direct teaching On'을 off로 변경하시거나 Enable Switch에서 손을 때시면 직접교시가 정지 됩니다.
* 직접교시 실행시 로봇 주변 사물이나 사람을 확인후 동작해주시기 바랍니다.
* 두개 이상의 버튼이 동시에 눌러질 경우 처음 누른 버튼만 인식합니다.
* 직접교시 중 TP를 이용하여 로봇을 자동으로 돌릴 경우 로봇이 바로 정지합니다. 이 경우 긴급 정리이기 때문에 위험합니다.
{% endhint %}

[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/README.md)
# 1.5 간편 엔코더 옵셋

로봇에 내장된 장치로 마스터링하는 간편 엔코더 옵셋을 설명합니다. 
본 기능은 크게 두 가지로 구성되어 있습니다.
- 간편 마스터링 위치 설정
- 간편 마스터링

[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/1-update-mastering-position.md)
# 1.5.1 간편 마스터링 위치 설정

로봇은 특정 위치에서 마스터링을 해야하며, 그 위치를 지정하는 방법을 설명합니다. 마스터링 위치를 지정할 때 로봇이 움직이므로, 로봇 주변에 사람, 물건 등과 충돌하지 않도록 주의해야 합니다. 참고로, 마스터링이 가능한 위치는 다양하게 있는데, 현재 로봇 자세에서 가까운 곳으로 설정됩니다.

- **\[시스템]** 버튼 > **\[11: 협동로봇 시스템 > 간편 엔코더 옵셋]** 메뉴를 터치하십시오.
- '마스터링 위치'에 '2차 엔코더', '1차 엔코더'가 있는데, 로봇이 마스터링 위치에 있을때의 각 관절별 엔코더 값을 나타냅니다.
- 새 마스터링 위치를 등록하기 위해 하단에 있는 '새 위치 이동' 버튼을 터치합니다.
    - 버튼이 터치되었을 때 로봇이 현재 위치에서 가까운 마스터링 위치로 이동합니다. 
    - 이동 완료가 될 때까지 버튼을 계속 터치합니다. 버튼을 터치하지 않으면 로봇은 정지합니다.
    - 이동 완료가 되면 '위치 최신화' 버튼을 터치합니다.
    - '저장하기' 버튼을 터치합니다.

    ![](../../_assets/simple_encoder_offset_1.png)

{% hint style="warning" %}
**\[주의]**
* 마스터링 위치로 이동하지 않고 '위치 최신화' 버튼을 터치하면 마스터링 위치가 갱신되지 않습니다.
* 마스터링 위치로 이동한 후 '위치 최신화' 버튼을 터치하고 저장까지 해야 새 마스터링 위치가 설정됩니다.
* 아래의 경우, 마스터링 위치를 새롭게 설정해야 합니다. 기존에 등록된 마스터링 위치를 그대로 사용할 경우, 정상적으로 마스터링이 되지 않거나 사고가 발생할 수 있습니다.
    - 2차 엔코더 교체
    -  **\[시스템]** > **\[11: 협동로봇 시스템 > 간편 엔코더 옵셋]** 메뉴에서 엔코더 초기화
{% endhint %}
[__SOURCE](1-cobot-safety-function/1-5-simple-encoder-offset/2-update-encoder-offset.md)
# 1.5.2 간편 마스터링

설정된 마스터링 위치로 로봇이 이동한 후 엔코더 옵셋을 초기화(마스터링)하는 방법을 설명합니다. 마스터링 위치로 로봇이 이동하므로, 로봇 주변에 사람, 물건 등과 충돌하지 않도록 주의해야 합니다. 

- **\[시스템]** 버튼 > **\[11: 협동로봇 시스템 > 간편 엔코더 옵셋]** 메뉴를 터치하십시오.
- '현재 위치'에 '2차 엔코더', '1차 엔코더'가 있는데, 현재 로봇 위치에서 각 관절별 엔코더 값을 나타냅니다.
- 로봇이 마스터링 위치로 이동하기 위해 하단에 있는 '위치 이동' 버튼을 터치합니다.
    - 버튼이 터치되었을 때 로봇이 마스터링 위치로 이동합니다. 
    - 이동 완료가 될 때까지 버튼을 계속 터치합니다. 버튼을 터치하지 않으면 로봇은 정지합니다.
    - 이동 완료가 되면 '전체 초기화' 버튼을 터치합니다.
    - 저장하기 버튼을 터치합니다.
    - 제어기를 재부팅합니다.

    ![](../../_assets/simple_encoder_offset_1.png)

{% hint style="warning" %}
**\[주의]**
* 등록된 마스터링 위치가 있어야 간편 마스터링 기능을 사용할 수 있습니다.
* 마스터링 위치로 이동하지 않고 '전체 초기화' 버튼을 터치하면 엔코더 옵셋이 초기화되지 않습니다.
* 엔코더 옵셋 후 저장까지 해야 엔코더 옵셋이 최신화됩니다.
* 간편 엔코더 옵셋 기능을 빈번하게 사용하면 마스터링 성능이 저하됩니다. 필요한 경우에만 사용하시기 바랍니다.
{% endhint %}
[__SOURCE](attachment/rules-criteria-and-public-notice.md)
# 산업안전보건기준에 관한 규칙 및 안전검사 고시

"[산업안전보건기준에 관한 규칙](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/ko/README)"

[__SOURCE](warranty.md)
# 품질 보증

"[품질보증](https://hrbook-hrc.web.app/#/view/quality-assurance/ko/README)"
