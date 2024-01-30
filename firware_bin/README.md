# Homekit_Air_Conditioner_Remote

### Flash del dispositivo
<ol>
<li>Utilizzare header 4 poli con passo da 1,27 mm o du-pont ed interfaccia FTDI-->USB.</li>
<li>Tienere premuto il pulsante IO0 durante l'accensione dell' ESP8266.</li>
<li>Rilasciare il pulsante IO0.</li>
<li> <a href="https://www.espressif.com.cn/zh-hans/support/download/other-tools">ESP Flash </a></li>

<br>Homekit_AC_Remote_1.0.0.bin，@0x0
<br>DoNotChgBin is unchecked。
<br>select COM：...，BAUD:115200。
<br>ERASE...
<br>START...
</ol>

<!--
<div align="center">
<br><img src="/image/flash_download.jpg"  width="50%" alt="flash_download"/>
</div>
-->

### ESP8266 PIN 
&emsp;&emsp;[Homekit-Air-Conditioner-Remote](https://github.com/LouisLee985/Homekit-Air-Conditioner-Remote/tree/main/hardware)
<br>&emsp;&emsp;[Air_Conditioner_Remote_1.6.0.bin](/firware_bin)
<div align = "center">

| IR_T(OUT) | Trasmettitore infrarosso |IO14|
| :---: | :---: |:---: |
|**IR_R(IN)** | **Ricevitore infrarosso** |**IO12**|
|**LED** |**Led** |**IO2**|
|**Button**|**Pulsante** |**IO0** |
|**SDA**| |**IO4** |
|**SCL**| |**IO5** |
</div>

### Sparkfun_ir_blaster PIN
&emsp;&emsp;[SparkFun WiFi IR Blaster (ESP8266)](https://github.com/sparkfun/ESP8266_WiFi_IR_Blaster)
<br>&emsp;&emsp;[Air_Conditioner_Remote_1.6.0-sparkfun_ir_blaster.bin](/firware_bin)
<div align = "center">

| IR_T(OUT) | Trasmettitore infrarosso |IO4|
| :---: | :---: |:---: |
|**IR_R(IN)** | **Ricevitore infrarosso** |**IO13**|
|**LED** |**Led** |**IO5**|
|**Button**|**Pulsante** |**IO0** |
|**SDA**| |**IO12** |
|**SCL**| |**IO14** |
</div>

