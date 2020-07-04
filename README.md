# Marlin1.1.9-for-Creality

Marlin 1.1.9 firmware for Creality 3D printers and different upgrades

Based on [Marlin](https://github.com/MarlinFirmware/Marlin) firmware, with different configurations for Creality 3D printers (mainly Ender series), e.g. silent board or BLTouch upgrade.

## Directories

* _/Marlin_ - source code folder, you can open _Marlin.ino_ in Arduino IDE and compile the firmware yourself. By default, it contains 'vanilla' Ender 3 configuration files from [Marlin](https://github.com/MarlinFirmware/Marlin) repository
* _/bin_ - compiled firmware which can be uploaded via programmer provided by Creality in BLTouch upgrade kit
* _/conf_ - configuration files for different versions, copy the version you need to _Marlin_ directory
* _/sanguino_ - board definition you'll need for Arduino IDE compilation process
