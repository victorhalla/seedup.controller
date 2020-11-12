# seedup.controller
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
 ![System Schematic](/docs/images/schematic.PNG "SEEDUP Controller System Schematic")

The shield will be designed to support diferrent type of sensors and controllers, like MOSFET, Relays, etc. First draft view of board is the following:
 ![Shield](/docs/images/seedup-board-v1.PNG "SEEDUP Board")

 The eletronics can be added in the board in a Plug&Play mode, like Relay Board
  ![Relay Board](/docs/images/seedup-relay-v1.PNG "SEEDUP Relay Board")
