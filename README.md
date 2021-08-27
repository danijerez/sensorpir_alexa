# Sensor Pir 🎅 Pápa Noel / 🧙‍🧙🏼‍♂️🧙 Reyes Magos 

### ¿Necesitas que alexa te avise cuando Papa Noel ha llegado? Monta un sensor de movimiento con arduino que envia notificaciones por Alexa. También vale para los reyes magos, y bueno, para los intrusos...

# 🖖 [![Twitter Follow](https://img.shields.io/twitter/follow/d4nijerez?style=social)](https://twitter.com/d4nijerez) ![GitHub Followers](https://img.shields.io/github/followers/danijerez?style=social)

<img src="img/photos/papanoel.png" width="100%"/> 

## 🙋 ¿Que es un sensor Pir?

<table style="width:100%">
  <tr>
    <td>
    <img src="img/arduino/sensor-pir.png"/> 
	</td>
        <td>
Los sensores infrarrojos pasivos (PIR) son dispositivos para la detección de movimiento. Son baratos, pequeños, de baja potencia, y fáciles de usar. Por esta razón son frecuentemente usados en juguetes, aplicaciones domóticas o sistemas de seguridad. Si te interesa saber mas, te dejo en la documentación un enlace donde lo explican en profundidad.
	</td>
  </tr>
</table>

## 🗺️ Diagrama

<table style="width:100%">
  <tr>
    <td>
<img src="img/arduino/circuito.png" /> 
	</td>
        <td>
          Sensor Pir
<img src="img/arduino/pir-back.png" /> 
	</td>
  </tr>
</table>




## 🧩 Componentes

<table style="width:100%">
  <tr>
    <td>
      Wemos D1 Mini
    <img width="80%"  src="img/arduino/wemos_d1_mini.jpg" href="https://www.amazon.es/AZDelivery-D1-Mini-desarrollo-compatible/dp/B0754N794H"/>
	</td>
    <td>
      Sensor Pir
    <img  src="img/arduino/pir.jpg" href="https://es.aliexpress.com/item/32849387755.html"/>
	</td>
   <td>
      Interruptor
    <img width="80%" src="img/arduino/interruptor.jpg" href="https://es.aliexpress.com/item/32859210037.html?spm=a2g0s.9042311.0.0.542363c0Y6L3aV"/>
	</td>
  </tr>
</table>

## 💿 Programas
[![Source](https://img.shields.io/badge/arduino_ide-008184?style=for-the-badge&logo=cplusplus&logoColor=white&labelColor=101010)](https://www.arduino.cc/en/software)
[![Source](https://img.shields.io/badge/Librería_PubSubClient-008184?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/knolleary/pubsubclient)

## 💾 Código
[![Source](https://img.shields.io/badge/flash_doorbell.ino_with_arduino_ide-999999?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/danijerez/doorbell_alexa/tree/master/doorbell)

## 🎨 Preparación
|#|   |   |
|---|---|---|
|  0 | <img src="img/icos/smartnest.png" width="30%"/>  | Recomiendo ver el video tutorial de un ejemplo parecido: https://www.youtube.com/watch?v=cgfVXPfCgkc  |
|  1 | <img src="img/icos/smartnest.png" width="30%"/>  | Nos registramos en <a href="https://www.smartnest.cz/index/ES">Smartnest</a> y creamos un dispositivo Timbre  |
|  2 | <img src="img/icos/alexa.png" width="30%"/>  | Desde la configuracion de Alexa (App movil o web) vinculamos nuestra cuenta Smartnest y elegimos el dispositivo que notificará |
|  3 | <img src="https://www.arduino.cc/en/pub/skins/arduinoWide/img/ArduinoAPP-01.svg" width="30%"/>  | Con las credenciales generadas de Smartnest, y nuestra configuración de Wifi, modificamos en el codigo la siguiente sección:|

``` #define SSID_NAME "Wifi-name"               // Your Wifi Network name
#define SSID_PASSWORD "Wifi-password"           // Your Wifi network password
#define MQTT_BROKER "smartnest.cz"              // Broker host
#define MQTT_PORT 1883                          // Broker port
#define MQTT_USERNAME "username"                // Username from Smartnest
#define MQTT_PASSWORD "password"                // Password from Smartnest (or API key)
#define MQTT_CLIENT "device-Id"                 // Device Id from smartnest 
``` 

## 🧰 Tutorial

|#|   |   |
|---|---|---|
|  1 | <img src="https://www.arduino.cc/en/pub/skins/arduinoWide/img/ArduinoAPP-01.svg" width="30%"/>  | Instalar la libreria PubSubClient en el IDE - <a href="https://github.com/knolleary/pubsubclient">ver codigo</a> .  |
|  2 | <img src="https://www.arduino.cc/en/pub/skins/arduinoWide/img/ArduinoAPP-01.svg" width="30%"/>  | Flashear el codigo en el arduino nano - <a href="https://github.com/danijerez/sensorpir_alexa/blob/master/pir/pir.ino">ver codigo</a> .  |


## 🖼️ Resultado
<img src="img/photos/resultado.png" width="30%"/> 


## 🧪 Testing
[![YouTube](https://img.shields.io/badge/sample_1-FF0000?style=for-the-badge&logo=youtube&logoColor=white&labelColor=101010)](https://youtu.be/XkGclKIlED0)

## 💡 Documentación
* https://www.youtube.com/watch?v=cgfVXPfCgkc
* https://www.smartnest.cz
* https://github.com/knolleary/pubsubclient
* https://www.luisllamas.es/detector-de-movimiento-con-arduino-y-sensor-pir
