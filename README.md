# pico-dht

**Temperature and Humidity Sensor**

## Hardware wiring

Hardware required:

- Raspberry pi Pico
- DHT22 sensor
- Optional [case](https://www.printables.com/model/1116831-raspberry-pi-pico-w-dht22-temperature-sensor-enclo)

It's important that the wiring are according to the following:

- `Power`  3V from pico `3V3(OUT)` to first pin from left on DHT.
- Resistor (10 kOhm) between first and second pi on DHT.
- `GND` on pico to 4th pin on DHT (right most).

![Raspberry Pi Pico Pinout](https://www.raspberrypi.com/documentation/microcontrollers/images/picow-pinout.svg)

