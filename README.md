# RF1000 Firmware
Based on Repetier-Firmware - the fast and user friendly firmware.

## Installation

The firmware is compiled and downloaded with Arduino V 1.0.5 or later.

## Version 0.91.49dual (2014-12-22)

* This is the development branch on base of the V 0.91.48 stable release.
* It may contain more features than the master branch but it also can be less stable.

## Printing and milling

This version of the firmware can be used as pure printer firmware (= the current default) or as firmware that can be switched between the operating modes "print" and "mill".
In order to allow the "mill" mode, FEATURE_CNC_MODE must be set to "2". Afterwards, the menu receives an additional entry which allows to switch the current operating mode between "print" and "mill".
The default operating mode can be configured via DEFAULT_OPERATING_MODE.

## Documentation

For documentation please visit [http://www.repetier.com/documentation/repetier-firmware/](http://www.repetier.com/documentation/repetier-firmware/)

## Introduction

This variant of the Repetier-firmware has been optimized for the use with the
Renkforce RF1000 3D Printer of Conrad Electronic SE.
The firmware adds functionality which is not available within the standard
Repetier-firmware and uses the settings which match the available hardware.

The main differences to the standard Repetier-firmware are:

* Support for the RF1000 motherboard.
* Support for the RF1000 feature controller (= 6 additional hardware buttons).
* Support for motor current control via the TI DRV8711.
* Support for an external watchdog via the TI TPS382x.
* Printing can be paused/continued via a hardware button.
* Heat bed scan and Z-compensation via the built-in strain gauge of the extruder.
* Automatic emergency pause in case the strain gauge delivers too high measurements.
* Additional M-codes have been defined in order to control the RF1000-specific functionality.
* There is no support for the ArduinoDUE.

## Changelog

See changelog.txt
