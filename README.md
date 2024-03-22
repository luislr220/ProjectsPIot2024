# Estación meteorologica
## Integrantes

- Luis Armando Largo Ramirez
- Omar Zuñiga Abundis

## Objetivo general
Este proyecto tiene la finalidad de poder medir la humedad, presion atmosferica y humedad, para funcionar como una estación portatil
de clima. Esto tiene el objetivo de poder tener datos mas precios de el lugar donde se encuentra uno, ya que con los satelitales suele mostrar solo los datos regionales y no de el punto donde se encuentra uno. Esto tambien puede servir para dependiendo de la humedad sacar cosas de alguna habitación o un uso similar. 

## Tabla de Software utilizado
|Id|Software|Version|Tipo|
|---|---|---|---|
|1|Node-RED|1.3.5|Plataforma de programación para conectar dispositivos de hardware|
|2|MQTT|5.0|Protocolo de mensajería para IoT|
|3|Arduino IDE|1.8.15|Entorno de desarrollo integrado para programar placas Arduino|


## Prototipo
![prototipo](https://github.com/luislr220/ProjectsPIot2024/assets/114530204/dc14c2c9-b9d9-4322-8250-cf4a5bd9b6dc)

## Diagarama
<img width="562" alt="image" src="https://github.com/luislr220/ProjectsPIot2024/assets/114530204/61fbea87-7180-4a7c-a211-3a05f75c383b">
<br>

El potenciometro es usao como un sensor falso ocupando el lugar del BMP180, ya que wokwi no tiene este tipo de sensor, al igual que el lcd puede varias, en este caso se hizo así debido a como se le explico en el transcurso de la semana que no contabamos con los materiales y el efectivo necesario para realizar el prototipo, ya que lo que teniamos el año pasado se perdio.

### Conexiones
| Componente    | Descripción                                     | Conexión                                           |
|---------------|-------------------------------------------------|----------------------------------------------------|
| DHT (DHT11)   | Sensor de temperatura y humedad                 | Conectar el pin de datos (DHTPIN) al pin 4        |
| Potenciómetro | Potenciómetro para simular temperatura         | Conectar un terminal a GND y el otro a 5V, y el terminal central al pin analógico 34 (POT_PIN) |
| LCD (1602)    | Pantalla LCD con interfaz I2C                   | Conectar SDA al pin SDA del ESP32 (pin 21), SCL al pin SCL del ESP32 (pin 22), VSS a GND, VDD a 5V, A a 5V, y K a GND. |
| LED RGB       | LED RGB para mostrar temperatura en colores    | Conectar el pin rojo a LED_RED (pin 5), el pin verde a LED_GREEN (pin 18), y el pin azul a LED_BLUE (pin 19) |



