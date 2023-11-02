
# ESP32-Weather
esta es la primera version de un sketch que hice para consultar y mostrar datos meteorologicos en el modulo esp32.
todo empezo por un video donde enseñaban a instalar un sketch en el modulo esp8266, el cual mostraba en una pantalla oled
el estado del clima en tu ubicacion, como no tenia ese modudo y solo contaba con el esp32, busqué algo similar, pero los que encontre
eran contados con los dedos, no funcionaban o tenia errores a la hora de compilar el proyecto. decidi hacer mi propia version y
despues de muchos errores, pofin lo hice funcionar, despues ee arreglar varios detalles, decidi hacerle un logo.

# como funciona? 
el proyecto utiliza utiliza la API de openweathermap, la cual obtienes al registrarte y tambien la ID de tu ubicacion,
a partir de ello, el programa obtine unos datos en un archivo de javascript y se encarga de decodificarlos,
de ello obtiene datos, como la ubicacion, la temperatura, viento, etc..., y los almacena en variables que despues seran mostradas 
en la pantalla, cada 10 minutos se actualiza los datos
![20231102_002510](https://github.com/selenium2106/ESP32-Weather/assets/131538899/5d54a187-6a1b-47a4-8368-fdd47faba83e)
ID la ciudad, solo copias los números y lo pegas en el codigo

![20231102_002622](https://github.com/selenium2106/ESP32-Weather/assets/131538899/4c553dba-9aa9-4ba0-a625-f21852fc02ce)
Clave API que te dan por registrarte, también tienes que pegarla en el respectivo campo


Video de demostración
https://github.com/selenium2106/ESP32-Weather/assets/131538899/c30d92ef-5097-4013-870e-9a82f3ccb0ab



# requisitos
requiere las siguientes librerias:

< arduinojson v6

< NTPClient

< las librerias del esp32

< Adafruit SSD1306

< Adafruit GFX 

# dato adicional
este proyecto puede ser usado con baterias, consume alrededor de 100mAh, pretendo mejorarlo 
para que pueda tener un modo de hibernacion, para que consuma lo menos posible.
