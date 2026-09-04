
# Outatime Pro
A PCB for Casio CA-53W or 3208 module based on the [Sensor Watch Pro](https://github.com/joeycastillo/Sensor-Watch). It has the same features!

![PCB view](img/pcb-preview.png)

# Firmware
Firmware is being worked on [here](https://github.com/evyd13/second-movement/tree/outatime-pro).

# WARNING
THIS IS NOT TESTED IN ANY WAY. DO NOT ORDER THIS THINKING IT WILL WORK. FIRMWARE DOESN'T EXIST FOR IT YET. IT IS A WORK IN PROGRESS.
However, the PCB design is done.

## Version number
Version number is date formate yyMMDD, August 25th 2026 would be v260825.

# To-Do
The following still needs work:

- Firmware needs to be finished (work has started!)
- figure out if the selection signals for PAM need to be connected to GPIO or always HIGH.
- PCB needs to be ordered and tested (I intend to do this in a few months time, need to gather funds for a prototype)
- It needs to be worn and loved!!

# Bootloader
I contacted devolov, they said to me that the firmware needs to be flashed with utils/flash_watch_pyruler using Adafruit PyRuler or Trinket. (I intend to use Seeed XIAO or maybe Pi Pico.)

Bootloader.h is generated from https://github.com/joeycastillo/uf2-samdx1.
(Thanks @devolov!)

# LCD
The LCD is fairly simple. It has 35 pins, of which the leftmost is not connected. The first 3 connected pins are common, the rest are segments. Mapping can be found within the emulator svg file or watch_common_display.h.

# Thanks to and relevant projects
- Joey Castillo for Sensor Watch, which this project is mostly based on. https://github.com/joeycastillo/Sensor-Watch/tree/main
- Travis Goodspeed, for incredible documentation about the Casio CA-53W. https://github.com/travisgoodspeed/goodwatch
- Vasily Zhuravsky, for a nice USB edge connector library https://github.com/vasya-zh/PCB-Edge-USB-connector-KiCad-library
- Dmitry Teplitsky, for making me think I can do it https://github.com/icelord75/icesio
- Greg Davill, for pointing the way to a microcontroller to use. https://github.com/gregdavill/advent-calendar-of-circuits-2020/tree/main/arm-watch
