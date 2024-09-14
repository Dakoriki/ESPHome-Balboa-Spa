Good recourses which this is made with/from:

https://github.com/ccutrer/balboa_worldwide_app/wiki ; https://github.com/ccutrer/balboa_worldwide_app/blob/main/doc/protocol.md ; https://github.com/cribskip/esp8266_spa ; https://github.com/jrowny/ESPHomeSpa ; https://github.com/vBrolin/ESPHomeSpa

# ESPHome Balboa Spa

Get local control of a Balboa spa using an ESPhome supported micro controller (ESP32, ESP8266)

# Funtionality

With this project you can:

- View and Control:
  - Temperature
  - Jets
  - Lights
  - Time on the spa clock
  - Onboard filtration cycles
- View the state of the spa heater and circulation pump
- Set temperature range (High/Low) and rest mode (Heat/Rest)

Upstream sources have been tested with Balboa BP2100G0 and BP601 series controllers
This fork has been tested with a BP2100G1 controller with an ESP8266

# Hardware and Connections

From upstream sources:

- [Parts](https://github.com/cribskip/esp8266_spa#parts)
- [Connections](https://github.com/cribskip/esp8266_spa#hardware-connections)

Some parts I used:

- Wemos D1 Mini Pro with an [external antenna*](pictures/external_antenna.md)
- [LM2596 Step-down voltage regulator (Aliexpress)](https://www.aliexpress.com/item/32653212622.html)
- TTL to RS458 module
- [Case**](https://www.aliexpress.com/item/1005005341333614.html) and [PCB](https://www.aliexpress.com/item/1005003384353640.html) (Use 4X6 if you use the case as well), both Alixpress
- [Screw terminal blocks (Aliexpress)](https://www.aliexpress.com/item/32868515933.html)

**The case I used is kinda small, you can use a different bigger case

The hardware layout I used:

![1](pictures/with_esp.jpg) ![2](pictures/under_esp.jpg)

# Project defaults

This project is set up for a spa that has:

- 3 Jets, 1 Light, Temperature in Celcius, a Heater, a Circulation pump, 2 Filter timeable cycles, Heat/Rest mode, High/low temperature range and a clock for time

If your spa has more or less or different things you will most likely changed things in the code

