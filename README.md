# Marlin1.1.9-for-Creality

_Marlin 1.1.9 firmware for Creality 3D printers and different upgrades_

Based on [Marlin](https://github.com/MarlinFirmware/Marlin) firmware, with different configurations for Creality 3D printers (mainly Ender 3 series), e.g. silent board or BLTouch upgrade. This version is derived from _1.1.x-bugfix_ branch. This **is not official Creality firmware** and it lacks some features (e.g. power loss resume), but **it does have thermal runaway protection enabled** on the other hand.

## Directories

* _/Marlin_ - source code folder, you can open _Marlin.ino_ in [Arduino IDE](https://www.arduino.cc/en/main/software) and compile the firmware yourself. By default, it contains 'vanilla' Ender 3 configuration files from [Marlin](https://github.com/MarlinFirmware/Marlin) repository
* _/bin_ - compiled firmware which can be uploaded via programmer provided by Creality in **BLTouch upgrade kit**
* _/conf_ - configuration files for different versions, copy the version you need to _Marlin_ directory
* _/sanguino_ - board definition you'll need for Arduino IDE compilation process

---

## Croatian:

_Marlin 1.1.9 firmware za Creality 3D printere s raznim dodacima i konfiguracijama_

Ova verzija bazirana je na [Marlin](https://github.com/MarlinFirmware/Marlin) firmwareu (_1.1.x-bugfix_ branch) s raznim konfiguracijama za Creality 3D printere (uglavnom Ender 3) i za različite dodatke kao što su BLTouch ili silent motherboard. Ovo **nije službeni Creality firmware**, ali zato s druge strane **ima omogućen thermal runaway protection**.

## Direktoriji

* _/Marlin_ - izvorni kod Marlin firmwarea, možete otvoriti _Marlin.ino_ datoteku u [Arduino IDE-u](https://www.arduino.cc/en/main/software) i sami kompajlirati firmware s konfiguracijom po vlastitiom izboru. Konfiguracijske datoteke u ovom direktoriju odgovaraju tvorničkim Ender 3 postavkama (bez dodataka) i preuzete iz [Marlin](https://github.com/MarlinFirmware/Marlin) repozitorija
* _/bin_ - kompajlirane verzije firmwarea koje je moguće uploadati korištenjem programatora iz Creality **BLTouch upgrade kita**
* _/conf_ - konfiguracijske datoteke za različite verzije i dodatke, kopirajte onu koja vam odgovara u  _Marlin_ direktorij
* _/sanguino_ - definicija matične ploče potrebna za kompajliranje firmwarea u Arduino IDE-u

---

## Original Marlin README:

# Marlin 3D Printer Firmware

[![Build Status](https://travis-ci.org/MarlinFirmware/Marlin.svg?branch=RCBugFix)](https://travis-ci.org/MarlinFirmware/Marlin)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/2224/badge.svg)](https://scan.coverity.com/projects/2224)

<img align="top" width=175 src="marlin-250.png" />

Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).
Please test this firmware and let us know if it misbehaves in any way. Volunteers are standing by!

## Bugfix Branch

__Not for production use. Use with caution!__

This branch is used to accumulate patches to the latest 1.1.x release version. Periodically this branch will form the basis for the next minor 1.1.x release.

Download earlier versions of Marlin on the [Releases page](https://github.com/MarlinFirmware/Marlin/releases). (The latest tagged release of Marlin is version 1.1.9.)

## Recent Changes
- Internally always use native machine space
- Initial UBL LCD Menu
- New optimized G-code parser singleton
- Initial `M3`/`M4`/`M5` Spindle and Laser support
- Added `M421 Q` to offset a mesh point
- Refinements to `G26` and `G33`
- Added `M80 S` to query the power state
- "Cancel Print" now shuts off heaters
- Added `EXTRAPOLATE_BEYOND_GRID` option for mesh-based leveling

## Submitting Patches

Proposed patches should be submitted as a Pull Request against this branch ([bugfix-1.1.x](https://github.com/MarlinFirmware/Marlin/tree/bugfix-1.1.x)).

- This branch is for fixing bugs and integrating any new features for the duration of the Marlin 1.1.x life-cycle. We've opted for a simplified branch structure while we work on the maintainability and encapsulation of code modules. Version 2.0 and beyond should improve on separation of bug fixes and cutting-edge development.
- Follow the proper coding style to gain points with the maintainers. See our [Coding Standards](http://marlinfw.org/docs/development/coding_standards.html) page for more information.
- Please submit your questions and concerns to the [Issue Queue](https://github.com/MarlinFirmware/Marlin/issues). The "naive" question is often the one we forget to ask.

### [RepRap.org Wiki Page](http://reprap.org/wiki/Marlin)

## Credits

The current Marlin dev team consists of:
 - Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)]
 - Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)]
 - Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)]

Notable contributors include:
 - Alberto Cotronei [[@MagoKimbra](https://github.com/MagoKimbra)]
 - Andreas Hardtung [[@AnHardt](https://github.com/AnHardt)]
 - Bernhard Kubicek [[@bkubicek](https://github.com/bkubicek)]
 - Bob Cousins [[@bobc](https://github.com/bobc)]
 - Chris Palmer [[@nophead](https://github.com/nophead)]
 - David Braam [[@daid](https://github.com/daid)]
 - Edward Patel [[@epatel](https://github.com/epatel)]
 - Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)]
 - Ernesto Martinez [[@emartinez167](https://github.com/emartinez167)]
 - F. Malpartida [[@fmalpartida](https://github.com/fmalpartida)]
 - Jochen Groppe [[@CONSULitAS](https://github.com/CONSULitAS)]
 - João Brazio [[@jbrazio](https://github.com/jbrazio)]
 - Kai [[@Kaibob2](https://github.com/Kaibob2)]
 - Luc Van Daele[[@LVD-AC](https://github.com/LVD-AC)]
 - Nico Tonnhofer [[@Wurstnase](https://github.com/Wurstnase)]
 - Petr Zahradnik [[@clexpert](https://github.com/clexpert)]
 - Thomas Moore [[@tcm0116](https://github.com/tcm0116)]
 - [[@alexxy](https://github.com/alexxy)]
 - [[@android444](https://github.com/android444)]
 - [[@benlye](https://github.com/benlye)]
 - [[@bgort](https://github.com/bgort)]
 - [[@Grogyan](https://github.com/Grogyan)]
 - [[@marcio-ao](https://github.com/marcio-ao)]
 - [[@maverikou](https://github.com/maverikou)]
 - [[@oysteinkrog](https://github.com/oysteinkrog)]
 - [[@p3p](https://github.com/p3p)]
 - [[@paclema](https://github.com/paclema)]
 - [[@paulusjacobus](https://github.com/paulusjacobus)]
 - [[@psavva](https://github.com/psavva)]
 - [[@Tannoo](https://github.com/Tannoo)]
 - [[@teemuatlut](https://github.com/teemuatlut)]
 - ...and many others

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
