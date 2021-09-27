# Dongles

Document about Konami's software and hardware license management using different kinds of dongles.

## Casette

* Connection: custom edge connector
* Housing: custom plastic case in blue
* Variants:
  * Small, used in games without digital I/O:
    - GX700-PWB(D)
      - Xicor X76F041 (SOIC8, 4k-bit EEPROM, I2C, label "0038323")
    - GX894-PWB(D)
      - Xicor X76F041 (SOIC8, 4k-bit EEPROM, I2C, label "0038323")
      - TI ADC0838-N (A/D converter, SPI)?
      - Dallas Semiconductor DS2401 (SOIC6, serial number, 1-wire)
  * Wide, used in games with digital I/O:
    - GX883-PWB(D): has possible extra connectors on the cartridge front for amp control and linking
      - Xicor X76F041 (SOIC8, 1k-bit EEPROM, I2C, label "0038323")
      - Dallas Semiconductor DS2401 (SOIC6, serial number, 1-wire)
      - Analog Devices ADM232LJR (SOIC32, 2x RS-232 transceiver)
      - Cosel ZUS 1R5 0505 (DC-DC converter, 4.5V-9V -> 5V)
    - GE949-PWB(D)
      - GE949-PWB(D)A: has possible extra connectors on the cartridge front for amp control and linking
        - Microchip PIC16CE625 (TSSOP20, MCU+EEPROM, "ZS01")
        - Dallas Semiconductor DS2401 (SOIC6, serial number, 1-wire)
        - Linear Technology LT1381CS / Analog Devices ADM232AARN (SOIC32, 2x RS-232 transceiver)
        - Cosel ZUS 1R5 0505 (DC-DC converter, 4.5-9V -> 5V)
      - GE949-PWB(D)B: mostly unpopulated (including extra connector headers), silkscreen label "TYPE-B"
        - Microchip PIC16CE625 (TSSOP20, MCU+EEPROM, "ZS01")
        - Dallas Semiconductor DS2401 (SOIC6, serial number, 1-wire)
  * Custom:
    - PWB0000068810 (wide, used in 908): has extra connectors on the cartridge front for light control
      - Xicor X76F100 (SOIC8, 1k-bit EEPROM, I2C, label "0038323")
      - 2x Mitsubishi M54585FP (SOIC20, transistor array)
      - 2x 74LS175 (SOIC16, 4x D-flipflop)
      - bunch of capacitors and resistors
    - PWB0000088954 (wide, used in A18): has extra connectors on the cartridge front for light control
      - Xicor X76F100 (SOIC8, 1k-bit EEPROM, I2C, label "0038323")
      - Dallas Semiconductor DS2401 (SOIC6, serial number, 1-wire)
      - 2x Mitsubishi M54585FP (SOIC20, transistor array)
      - 2x 74HC4094 (SOIC16, shift register)
      - bunch of capacitors and resistors
  * Likely others for at least 876, 930, A07
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
* Housing: Dallas DS1411 black plastic case, "www.iButton.com" engraving, custom white label
* Variants:
  - Old (DS1411-009)
    * Custom white label with Konami logo and hand-written serial number
    * Dallas DS1991L-F5 (iButton, 1-wire)
    * Dallas DS2502 (1Kbit memory, 1-wire)
    * Dallas DS2480B (1-wire to RS232 driver)
    * Dallas DS9502P (ESD protection diode)
  - New
    * Custom white label with Konami logo, game name and product code, and serial number
    * Dallas DS1991L-F5 (iButton, 1-wire)
    * Dallas DS2401 (serial number, 1-wire)
    * Dallas DS2480B (1-wire to RS232 driver)
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
  - Identifier tag attached in blue/white (license), black/white (license, alt?), white/red (account), white/black (account, PASELI charger)
* Used in: Konami PC hardware post-iKey
* Later eTokens have a Gemalto engraving
