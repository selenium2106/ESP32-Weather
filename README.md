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

# requisitos
requiere las siguientes librerias:

< arduinojson v6

< NTPClient

< las librerias del esp32

# dato adicional
este proyecto puede ser usado con baterias, consume alrededor de 100mAh, pretendo mejorarlo 
para que pueda tener un modo de hibernacion, para que consuma lo menos posible.
