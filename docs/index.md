# Seedup Controller
SEEDUP is a Open Source shield that uses ESP32-CAM, Arduino Nano v3 and MCP23016 to fully control an hidroponic system.

The develop started back in 2015 as a small board to control an hidroponic system using the well know Arduino Nano board and after some months migrated to the Particle Platform that allow control over Wifi.

Now using ESP32-CAM, Arduino Nano v3 and MCP23016 the idea is to create a modular shield that can support the following:

1. Sensors
    1. Air Temperature and Humidity
    2. Light
    3. CO2
    4. Water PH
    5. Water EC
    6. Water Temperature
    7. Water Flow
    8. Water Level
2. Controllers
    1. Light
    2. Air Heater
    3. Air Cooler
    4. Air Fan
    5. CO2
    6. Water Circulation
    7. Water Valve
    8. Nutrients Peristaltic Pump
    9. Water Heater 
    10. Water Fog

The picture below shows a simple system schematic:
 ![System Schematic](/seedup.controller/images/seedup_schematic.png "SEEDUP Controller System Schematic")

The shield will be designed to support diferrent type of sensors and controllers, like MOSFET, Relays, etc. First draft view of board is the following:
 ![Shield](/seedup.controller/images/seedup-board-v1.PNG "SEEDUP Board")

To be able to start small I defined that 3 versions of the shield will be available: SeedUP, SeedUP Micro and SeedUP Nano with the following characteristcs:

**Shield** | **SeedUP** | **SeedUP Micro** | **SeedUP Nano**
:-- | :-: | :-: | :-:
**Wifi** | 802.11b/g/n | 802.11b/g/n | 802.11b/g/n
**Bluetooth** | 4.2 BT/BLE | 4.2 BT/BLE | 4.2 BT/BLE
**Camera** | Yes | - | -
**Controllers** | 20 | 4 | 1
-Relays | 11 (up to 20) | 4 | 1
-Triac | 4 | - | -
-Mosfet | 5 | - | -
**Sensors** | 10 | 1 | 1
-Air Temperature | Yes | - | -
-Air Humidity | Yes | - | -
-CO2 | Yes | - | -
-Light | Yes | - | -
-Water Flow | Yes | - | -
-Water Temperature | Yes | - | -
-Water EC | Yes | - | -
-Water PH | Yes | - | -
-Water Level | Yes | - | -
-Bluetooth* | Yes | Yes | Yes

*Bluetooth: use bluethooth sensors like Xiami Flora Sensor [https://xiaomi-mi.com/sockets-and-sensors/xiaomi-huahuacaocao-flower-care-smart-monitor/](https://xiaomi-mi.com/sockets-and-sensors/xiaomi-huahuacaocao-flower-care-smart-monitor/)

The idea behind 3 shields is to facilitate from home use to professional use allowing more people to benefit from it.

## SeedUP Nano
SeedUP Nano will basic work for self watering planter allowing to eliminate basic problems on a domestic indoor environment.

Many people want to plant indoors by placing pots next to the windows, but most of the time they are not successful. The two main problems are the lack of lighting and water. To solve the lighting problem it is necessary to add lamps that can overcome this deficiency and to automate the water process we can use the self watering system.

Shield will also be cabable to use bluetooth sensors to obtain data like soil moisture, temperature, sunlight and nutrient.

 ![SeedUp Nano](/seedup.controller/images/seedup_nano_schematic.png "SeedUP Nano")

### Self Watering System
Self-watering containers work on a reservoir system. There is a water storage tank at the bottom of the container. The soil soaks up the water from the bottom through a wick, so as long as you keep the reservoir filled, your plants get a consistent level of moisture, delivered directly to their roots.

## SeedUP Micro
SeedUP Micro will only differ from Nano version due the capacity to support up 4 relays. This will allow to run more complicated setup that use more lamps, water automatic irrigation and temperature control.

 ![SeedUp Micro](/seedup.controller/images/seedup_micro_schematic.png "SeedUP Micro")
