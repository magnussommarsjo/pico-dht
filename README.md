# pico-dht

**Temperature and Humidity Sensor**

## Hardware wiring

Hardware required:

- Raspberry pi Pico (RP2040)
- DHT22 sensor
- Optional [case](https://www.printables.com/model/1116831-raspberry-pi-pico-w-dht22-temperature-sensor-enclo)

It's important that the wiring are according to the following:

- `Power`  3V from pico `3V3(OUT)` to first pin from left on DHT.
- `GND` on pico to 4th pin on DHT (right most).

![Raspberry Pi Pico Pinout](https://www.raspberrypi.com/documentation/microcontrollers/images/picow-pinout.svg)

## Software

Suggestion is to use `uv` as package manager or `pip` to install packages as a venv from the `pyproject.yaml` file.

To compile, a file called `secrets.yaml` must exist with your wifi credentials similar to

```yaml
wifi_ssid: "SSID"
wifi_password: "PASSWORD"
```

After this is set up you have to activate the virtual environment and run with your pico connected via usb.

```sh
esphome run sensor.yaml
```
