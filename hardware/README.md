# AC_IR_Homekit_USB_TYPE_A
* PCB doppia faccia

<div align="center">
<br><img src="/image/AC_IR_Homekit_USB_TYPE_A1.jpg"  width="60%" alt="AC_IR_Homekit_USB_TYPE_A1"/>
<br>
<br><img src="/image/AC_IR_Homekit_USB_TYPE_A2.jpg"  width="60%" alt="AC_IR_Homekit_USB_TYPE_A2"/>
<br>
<br><img src="/image/AC_IR_Homekit_USB_TYPE_A3.jpg"  width="60%" alt="AC_IR_Homekit_USB_TYPE_A3"/>
<br> 
<br><img src="/image/IMG_3366.JPG"  width="60%"/>
<br>
</div>
<br>

* <a href='http://htmlpreview.github.io/?https://github.com/LouisLee985/Homekit-Air-Conditioner-Remote/blob/main/image/BOM_AC_IR_Homekit_USB_TYPE_A.html'>InteractiveHtmlBom表</a>

* [Air_Conditioner_Remote_1.6.0.bin](/firware_bin)

* A proposito di temperatura e umidità：
<br>Poiché il PCB è troppo compatto, il sensore di temperatura e umidità sul PCB *`SHTC3`* di *`ESP-01F`* A causa dell'interferenza della dissipazione del calore, la misurazione della temperatura è sempre elevata.
<br>I sensori di temperatura e umidità e i relativi resistori e condensatori non necessitano di saldatura U8,R8,R9,C5，Homekit App La temperatura e l'umidità vengono visualizzate come 0.

* Se è necessaria una temperatura e un'umidità precise, non saldare U8,R8,R9,C5，Dopo aver flashato il firmware，Inoltre, ritira *`Modulo sensore di temperatura e umidità`* ，Tenere lontano da fonti di dissipazione del calore.
<br>SDA,SCL,3V3,GND per l'esterno *"Modulo sensore di temperatura e umidità".* 。

* Moduli esterni del sensore di temperatura e umidità SHT supportati:　SHTC1，SHTC3，SHTW1，SHTW2，SHT3x-DIS (I2C)，SHT3x-ARP (ratiometric analog voltage output)，SHT85，SHT4x，e.g.
<div align="center">
<br><img src="/image/SHT3X.jpg"  width="20%"/>
 </div> 
