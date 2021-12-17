# ESP8266 clock module

Using ESP-12F module with ESP8266 as the core as the main control

Onboard a 0.96 inch OLED, clock chip, five-way button, single-cell 18650 lithium battery charging chip; the battery can be charged through the microUSB interface Charging and programming ESP8266. Users can develop a different wifi clock based on their own ideas.

## Features

The 0.96 inch OLED can display the time intuitively.

The clock can be calibrated via wifi. Access to 18650 lithium battery can be used anytime, anywhere. It can charge the 18650 lithium battery, and there is a charging indicator to indicate the charging

The lead pins can be connected to other device modules for development. MicroUSB automatic programming function. Five-way buttons connected to five pins are equivalent to five buttons.

![esp8266](esp8266.jpg?raw=true "esp8266")


esptool --port /dev/ttyUSB0 --baud 921600 read_flash 0x00000 0x400000 backup.img

esptool --port /dev/ttyUSB0 --baud 921600 erase_flash

esptool --port /dev/ttyUSB0 run
