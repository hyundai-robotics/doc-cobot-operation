### 3.2.3 Tool IO 인터페이스

협동로봇 Tool IO 시스템 장치의 인터페이스를 설정하는 기능입니다.

<br>

{% hint style="info" %}
   - Tool IO 장치를 이용한 Modbus RTU 통신을 사용하는 경우 다음 매뉴얼을 참고해 주십시오.

   - "[Hi7 제어기 기능설명서 - 모드버스](https://hrbook-hrc.web.app/#/view/doc-modbus/ko/4-modbus-master/1-roblang?cont_model=Hi7)"
{% endhint %}


**1. 메뉴를 터치하여 설정 화면으로 진입합니다.**

<br>

**\[시스템 > 11: 협동로봇 시스템 > 2: Tool IO 설정 > 2: Tool IO 인터페이스 설정]**

<br>

![[그림 3.2.3-1 Tool IO 인터페이스 설정]](<../../_assets/3-cobot-Additional-function/2-tool-io/3-interface/image1.png>) 

<br>

{% hint style="info" %}
   [출력 전원 설정]   
   - 24V 전원: 외부 출력 전원 설정   
      - OFF   
      - 24V   
   - I/O 종류: Tool IO 디지털 입출력 방식 설정   
      - PNP   
      - NPN   

   [시리얼 통신 설정]   
   - Tool IO 시스템 RS485 커넥터의 시리얼 통신 파라미터를 설정합니다.   

   - 시리얼: 통신 사용 여부 설정   
      - OFF   
      - ON   
   - 통신 속도: 시리얼 통신 속도 설정   
      - 9600bps ~ 2.5Mbps   
   - 패리티 비트: 패리티 비트 설정   
      - 없음   
      - 홀수   
      - 짝수   
   - 종료 비트: 스톱 비트 설정   
      - 1 Bit   
      - 2 Bit   
   - 데이터 길이: 데이터 비트 길이 설정   
      - 7 Bit   
      - 8 Bit   
      
{% endhint %}

<br>

![[그림 3.2.3-2 Tool IO 인터페이스 설정]](<../../_assets/3-cobot-Additional-function/2-tool-io/3-interface/image2.png>) 

<br>

{% hint style="info" %}
   [전원 상태]   
   - 24V 전원: 외부 출력 전원의 ON/OFF 동작 상태   
   - I/O 종류: 현재 적용된 I/O 종류   
   - 전압 24V: 외부 출력 전압 측정값   
   - 전류 24V: 외부 출력 전류 측정값   

   [시리얼 상태]   
   - 시리얼 동작: 시리얼 통신 ON/OFF 동작 상태   
   - 통신 속도: 현재 적용된 통신 속도   
   - 패리티 비트: 현재 적용된 패리티 비트   
   - 종료 비트: 현재 적용된 종료 비트   
   - 데이터 길이: 현재 적용된 데이터 길이   
      
{% endhint %}