## Precompiled versions of Marlin firmware for Ender3

Precompiled versions are based on configuration files found at _/conf/Ender3_ directory. There are two types of compiled files for each version - with or without bootloader. Creality mainboards are mainly shipped with no bootloader (except for Silent motherboard), which means you can't upload new firmware via USB port, but you have to use programmer (which can be some other Arduino board) connected to ICSP header on the mainboard. If you have bootloader already installed on your board, it doesn't matter whic file you upload - everything will work just fine and next time you want to upload the firmware you'll just have to plug in USB cable. On the other hand, if you're uploading firmware via programmer there is a difference - if you upload *_with_bootloader.hex* file, next time you upload firmware it can be done via USB cable. But if you upload firmware without bootloader, you'll need to use programmer for next upload too.

Firmware versions:
* *Ender3_Marlin_basic.hex* - default version for factory supplied motherboard with no upgrades
* *Ender3_Marlin_BLTouch.hex* - BLTouch (version 3.0 or higher) upgrade using factory motherboard
* *Ender3_Marlin_silent_motherboard.hex* - silent motherboard upgrade
* *Ender3_Marlin_silent_motherboard_BLTouch.hex* - BLTouch (3.0 or greater) upgrade using silent motherboard

For BLTouch upgrade, please see the notes in _conf/Ender3_ directory.

---

## Kompajlirane verzije Marlin firmwarea za Ender3

Kompajlirane verzije bazirane su na konfiguracijskim datotekama u _/conf/Ender3_ direktoriju. Za svaku verziju postoje dva tipa kompajlirane datoteke - sa ili bez bootloadera. Creality uglavnom isporučuje matične ploče bez bootloadera (osim Silent Motherboarda), što znači da je za upload firmwarea potrebno koristiti programator (ili neku Arduino pločicu) spojen na ICSP header na matičnoj ploči, upload putem USB-a nije moguć. Ukoliko vaša ploča već ima bootloader, nije bitno koji tip uploadate - sve će raditi normalno i, kod idućeg uploada, ponovno možete koristiti USB. S druge strane, ukoliko ploča nema bootloadera, a koristite *_with_bootloader.hex*, idući puta moći ćete uploadati firmware putem USB-a. U slučaju da uploadate firmware bez bootloadera, idući puta ćete ponovno morati koristiti programator za upload.

Verzije firmwarea:
* *Ender3_Marlin_basic.hex* - osnovna verzija za tvornički isporučenu matičnu ploču bez upgradea
* *Ender3_Marlin_BLTouch.hex* - BLTouch (verzija 3.0 ili viša) upgrade na tvorničkoj matičnoj ploči
* *Ender3_Marlin_silent_motherboard.hex* - silent motherboard upgrade
* *Ender3_Marlin_silent_motherboard_BLTouch.hex* - BLTouch verzija 3.0 ili viša) upgrade na silent motherboard ploči

Ukoliko koristite BLTouch upgrade, pogledajte napomene u _conf/Ender3_ direktoriju.
