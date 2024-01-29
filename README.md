
# Homekit_Air_Conditioner_Remote
[![Release](https://img.shields.io/github/v/tag/LouisLee985/Homekit-Air-Conditioner-Remote?color=red&label=release)](https://github.com/LouisLee985/Homekit-Air-Conditioner-Remote/releases/latest)

<p align="center">
<img src="/image/HomeApp_Icon_2.svg" width="10%"/>
</p>

<br>
<div align="center">
<br><img src="/image/homekit1.jpg"  width="80%"/>
</div>


### WiFi


1. Dopo l'accensione quando ESP8266 non è connesso ad una rete, il LED lampeggerà 2/S
2. In questa fase viene creata una rete AP ESP_XXXXXX，dove XXXXXX è il MAC del dispositivo.
3. Connetti il tuo dispositivo all' AP，attendendo l'apertura della pagina di configurazione. In caso contrario aprire il browser e digitare l'indirizzo 192.168.4.1
4. Configurazione del WiFi，Scegliere la rete WiFi a cui collegare il dispositivo，inserire la password e premere Save，
5. Una volta stabilita la connessione, uscirà automaticamente dalla modalità di configurazione di rete e si chiuderà la rete AP ESP_XXXXXX.

<div align="center">
<br><img src="/image/WiFi_Configure.jpg"  width="80%"/>
</div>

### Aggiungere l'accessorio a HomeKit

* Codice per il pairing Homekit：985-21-985。
   
<div align="center">
<br><img src="/image/qrcode.jpg"  width="20%"/>
</div>

   　
* Come aggiungere accessori all'app CASA (https://support.apple.com/zh-cn/HT204893) ３modalità：
<!-- 
https://support.apple.com/en-us/HT204893 
-->


 <br>
　　１．Con la fotocamera dell'iPhone o iPad. Usare la fotocamera per scansionare il codice QR dell'accessorio.
<br>
　　２．Oppure aprendo app Casa e toccando Aggiungi; Poi toccare Aggiungi accessorio. Con la fotocamera inquadrare il codice QR.

<div align="center">
<br><img src="/image/IMG_3209.jpg"  width="80%"/>
</div>
<br>
 
　　３．In alternativa si può inserire il codice manualmente.

<div align="center">
<br><img src="/image/Add_accessories3.jpg"  width="80%"/>
</div>

<!-- 
<div align="center">
<br><img src="/image/Add_accessories1.jpg"  width="90%"/>
<br><img src="/image/Add_accessories2.jpg"  width="80%"/>
</div>
-->
<br>

### Funzione Aria Condizionata

1. Funzioni disponibili dell'aria condizionata in App Casa: accensione, spegnimento, raffreddamento, riscaldamento, velocità del vento, visualizzazione della temperatura ambiente attuale e dell'umidità.
<br>Per maggori informazioni [HomeKit Accessory Protocol Specification(Noncommercial Version) Release R2](https://developers.apple.com/homekit/faq) ,*"Questo accessorio non è stato certificato per funzionare con Homekit, pertanto alcune funzionalità potrebbero non essere disponibili."*.
2. Per controllare gli accessori HomeKit da remoto, occorre configurare HomePod, HomePod mini, Apple TV o iPad come hub domestico.](https://support.apple.com/zh-cn/HT207057)
3.Feedback del segnale a infrarossi: quando il telecomando del climatizzatore esegue azioni supportate dal protocollo Apple Homekit, come accensione, spegnimento, raffreddamento, riscaldamento, velocità ventole, ecc., app CASA aggiornerà lo stato in modo sincrono.


<div align="center">
<br><img src="/image/HAP-Specification-Non-Commercial-Version.jpg"  width="60%"/>
<br><img src="/image/Add_accessories3.PNG"  width="80%"/>
</div>

### Pulsante connesso alla GPIO IO0
1. Premere e tenere premuto il pulsante IO0 per 5-10 S, il LED 2/S lampeggerà
2. Rilasciare ora il pulsante.
3. Identificazione del telecomando del condizionatore d'aria: entro 15 S, puntare il telecomando del climatizzatore verso il ricevitore del blaster (IR_R).
4. Premere il pulsante e attendere che il LED smetta di lampeggiare.
5. RESET DEL DISPOSITIVO: Tenere premuto il pulsante IO0 per 10-15 S, il LED 2/S lampeggia, 4/S lampeggia
6. Rilasciare ora il pulsante. Saranno resettate tutte le impostazioni: reset Homekit ID, connessione Wi-Fi, protocollo del telecomando climatizzatore. 



# Thanks
* [HomeKit Accessory Protocol Specification(Noncommercial Version) Release R2](https://developers.apple.com/homekit/faq)
* [arduino-sht](https://github.com/Sensirion/arduino-sht) 
* [WiFiManager](https://github.com/tzapu/WiFiManager)
* [IRremoteESP8266](https://github.com/crankyoldgit/IRremoteESP8266) 
* [Arduino-HomeKit-ESP8266](https://github.com/Mixiaoxiao/Arduino-HomeKit-ESP8266) 
* [arduino-button-long-press-short-press](https://arduinogetstarted.com/tutorials/arduino-button-long-press-short-press)
*  https://github.com/openscopeproject/InteractiveHtmlBom
*  https://github.com/yanranxiaoxi/InteractiveHtmlBom

<div align="center">  
<img src="https://myoctocat.com/assets/images/base-octocat.svg"  width="10%"/> 
</div>

