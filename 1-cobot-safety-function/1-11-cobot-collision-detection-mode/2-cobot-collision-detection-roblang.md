# 1.11.2 충돌검지 로봇 명령어(cobot_coldet)

### 설명

협동로봇의 충돌검지 민감도를 설정합니다.

해당 충돌검지 기능은 Hi6 제어기에서 검지하게 됩니다. 

로봇언어를 사용하기 전에 반드시 cobot_coldet 모듈을 import 해야합니다.

### 문법

&lt;cobot_coldet&gt;.on &lt;dr1, dr2, dr3, dr4, dr5, dr6&gt;</br>
&lt;cobot_coldet&gt;.off 

### 파라미터

<table>
  <thead>
    <tr>
      <th style="text-align:left">항목</th>
      <th style="text-align:left">의미</th>
      <th style="text-align:left">범위</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>dr1~dr6</td>
      <td>
        각 축별 충돌 검지 민감도 (%)
      </td>
      <td>25~500</td>
    </tr>
    
  </tbody>
</table>


### 사용 예

```python
import cobot_coldet
cobot_coldet.on 100,25,500,150,100,300
cobot_coldet.off
```



