esphome-aldes
=============

Esphome configuration YAML files to control Aldès Insipirair ventilation unit with Modbus.

This has been developed for my home automation. 
I have two Inspirair Top 300 units  and one Inspirair Side 240. 
They are all conencted to Home Assitant thanks to Esphome running on ESP32 board attached to UART to RS485 converter.
This allows me to control the air flow according to humidity and CO2 concentration.

Project Structure
-----------------

Main files are `insipirair.yaml` and `insipirair-side.yaml`.

Other files are my own configurations given as examples.
Don't forget to change WIFI network settings.

There are also a `inspirair-host.yaml` and `insipirair-side-host.yaml` that allows you to test Home Assistant integration without a ESP board nor a unit under the hand.

Wiring
------

| Esp board | UART to RS485 |
|-----------|---------------|
| TX        | RX            |
| RX        | TX            |
| GND       | GND           |
| +5V       | +5V           |

RX and TX might be swapped depending on the labelling logic.

TODO
----

  - add bypass servo control for Inspirair Side


