# GEC02-PWB(A)A - bootleg

* A hardware bootleg of the [GEC02-PWB(A)A PCB](pwb-aa.md)
* Runs original base microcontroller and FPGA firmwares
* Key differences
  * Red dip-switches
  * Molex 4-pin power connector
* Important note regarding power connector
  * If power connector is mounted correctly (on the top PCB layer), +5V and +12V are swapped (!!!). You need adapter cable that swaps the two pins in order to power it correclty by any standard PC power supply
  * If the connector is mounted on the bottom of the PCB ("turned around"), the pins for +5V and +12V are correctly mapped to the molex connector
* Images
  * [PCB top](https://github.com/Shizmob/arcade-docs-media/blob/main/konami/GEC02/PWB(A)A%20bootleg/top.jpeg)
  * [PCB bottom](https://github.com/Shizmob/arcade-docs-media/blob/main/konami/GEC02/PWB(A)A%20bootleg/bottom.jpeg)