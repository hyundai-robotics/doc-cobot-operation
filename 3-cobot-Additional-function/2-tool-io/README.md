## 3.2 Tool IO 설정

<br>

이 장에서는 협동로봇의 6축 끝에 위치한 Tool IO 시스템에 대해 기술합니다.

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**전원 공급 사양**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>출력 전압</td>
		<td>24V</td>
	</tr>
	<tr>
		<td>정격 전류</td>
		<td>3A</td>
	</tr>
	<tr>
		<td>최대 Peak 전류</td>
		<td>4.5A</td>
	</tr>
</tbody>
</table>
<br>

**디지털 I/O 사양**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>커넥터</td>
		<td>TOOL IO <br> M8, A-code, 8Pin, Female</td>
	</tr>
	<tr>
		<td colspan=2>I/O 타입</td>
		<td>PNP / NPN</td>
	</tr>
	<tr>
		<td colspan=2>기준 전압</td>
		<td>24V</td>
	</tr>
	<tr>
		<td rowspan=2>채널 수</td>
		<td>디지털 입력</td>
		<td>2</td>
	</tr>
	<tr>
		<td>디지털 출력</td>
		<td>2</td>
	</tr>
	<tr>
		<td rowspan=4>디지털 입력</td>
		<td>OFF 상태 전압</td>
		<td>? ~ ?, @ 25°C</td>
	</tr>
	<tr>
		<td>ON 상태 전압</td>
		<td>? ~ ?, @ 25°C</td>
	</tr>
	<tr>
		<td>ON 상태 전류</td>
		<td>? ~ ?, @ 25°C</td>
	</tr>
	<tr>
		<td>입력 신호 필터 시간</td>
		<td>5ms</td>
	</tr>
	<tr>
		<td>디지털 출력</td>
		<td>ON 상태 전류</td>
		<td>? ~ ?, @ 25°C</td>
	</tr>
</tbody>
</table>
<br>

**아날로그 I/O 사양**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>커넥터</td>
		<td>TOOL IO <br> M8, A-code, 8Pin, Female</td>
	</tr>
	<tr>
		<td>채널 수</td>
		<td>2</td>
	</tr>
	<tr>
		<td>입력 전압 범위</td>
		<td>0 ~ 10V</td>
	</tr>
	<tr>
		<td>데이터 형식</td>
		<td>12bits (0 ~ 4095)</td>
	</tr>
	<tr>
		<td>입력 신호 필터</td>
		<td>이동 평균 필터 (50ms 평균 입력)</td>
	</tr>
	<tr>
		<td>오차 범위</td>
		<td>±0.5% Full Scale @ 25°C</td>
	</tr>
</tbody>
</table>
<br>

**시리얼 통신 사양 (RS485)**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>통신 방식</td>
		<td>RS485</td>
	</tr>
	<tr>
		<td>커넥터</td>
		<td>RS485 <br> M8, A-code, 8Pin, Female</td>
	</tr>
	<tr>
		<td>통신 속도</td>
		<td>9600bps<br>19200bps<br>38400bps<br>57600bps<br>115200bps<br>230400bps<br>460800bps<br>500Kbps<br>625Kbps<br>1Mbps<br>2.5Mbps</td>
	</tr>
	<tr>
		<td>패리티</td>
		<td>없음 / 홀수 / 짝수</td>
	</tr>
	<tr>
		<td>종료 비트</td>
		<td>1 Bit / 2 Bit</td>
	</tr>
	<tr>
		<td>데이터 길이</td>
		<td>7 Bit / 8 Bit</td>
	</tr>
</tbody>
</table>
<br>