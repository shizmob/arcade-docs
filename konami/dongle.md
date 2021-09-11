# Dongles

Document about Konami's software and hardware license management using different kinds of dongles.

## Casette

* Connection: custom edge connector
* Housing: custom plastic case in blue
* Variants:
  - Small (used in games without digital I/O)
  - Wide (used in games with digital I/O): has extra connectors on the cartride for amp control and linking
* Used in: [System 573](boards.md#system-573)

## Card

* Connection: custom card connector
* Housing: custom small housing in black
* Components:
  - Early:
    - Xicor X76F041 (SOIC8, 4k-bit EEPROM, I2C)
  - Late:
    - ST 24W02 (TSSOP8/SOIC8?, 2k-bit EEPROM, I2C)
* Used in: [Twinkle](boards.md#twinkle)

## Roundplug

* Connection: mini-DIN
* Housing: custom plastic case in black (license) or white (account)
* Components:
  - Dallas DS2430A (256-bit EEPROM, 1-wire)
* Used in: [Python](boards.md#python), [Python 2](boards.md#python-2), most Konami PC hardware pre-iKey/eToken

## Serial plug

* Connection: RS232 DE-9
* Housing: black plastic case, "www.iButton.com" engraving, white label
* Variants:
  - Old
    * White label with Konami logo and hand-written serial number
    * Dallas DS1991L-F5 (iButton, 1-wire)
    * Dallas DS2502 (1Kbit memory, 1-wire)
    * Dallas DS2480B (1-wire to RS232 driver)
    * Dallas DS9502P (ESD protection diode)
  - New
    * White label with Konami logo, game name and product code, and serial number
    * Dallas ??? (iButton, 1-wire)
    * Dallas DS2401 (serial number, 1-wire)
    * Dallas DS2480 (1-wire to RS232 driver)
* Used in: [Firebeat](boards.md#firebeat)

## iKey

* Connection: USB
* Housing: custom plastic housing in black (license) or white (account)
* Components:
  - Rainbow Technologies iKey 2032
* Used in: Konami PC hardware post-roundplug and pre-eToken

## eToken

* Connection: USB
* Housing: stock
* Components:
  - Safenet eToken 5110 or 5100
  - Identifier tag attached in blue/white (license), black/white (license, PASELI charger), white/red (account), white/black (account, PASELI charger)
* Used in: Konami PC hardware post-iKey
* Later eTokens have a Gemalto engraving
