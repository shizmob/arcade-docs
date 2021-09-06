# Interfaces

## V337 RC

Simple sound interface. Connects to internal sound header and exposes 1 red/white RCA pair.

* Product: 2626960201 / (2626970201) / RC01933
* Label: V337 RC PCB
* Copyright: 2007 NAMCO BANDAI Games Inc.
* Connectors:
  - (external) 1x RCA white, 1x RCA red
  - (internal) 1x 3pin audio connector (pinout up-down: GND LEFT RIGHT)

## V337 RS

Simple serial interface board.

* Product: 2626960101 / (2626970101) / RS01369
* Label: V337 RS PCB
* Copyright: 2007 NAMCO BANDAI Games Inc.
* Connectors:
  - (internal) 1x 8pin (2x serial, pinout up-down: J2-GND J2-TXD J2-RXD J3-RXD J3-TXD J3-GND J3-CTS J3-RTS)
  - (external) 1x 8pin (2x serial, pinout left-right: TXD1 RXD1 GND1 TXD2 RXD2 RTS CTS GND2)
* Ribbon cable product: (2626970301) / RX01187

## H039 ESIF

External serial interface. Connects to motherboard serial, and exposes JVS and serial. Likely turns on/resets the motherboard too.

* Product: 8694960101 / (8694970101) / 10L00373
* Label: H039 ESIF PCB
* Chips:
  - Hitachi HD64F3672 (QFP48, H8 MCU)
  - "E 14.7456C" "2PH K487H" (14.7456 MHz crystal)
  - Sipex SP485EC (SOIC8, RS-485 transceiver)
  - Maxlinear SP3222EUCY (SSOP16, RS-232 transceiver)
* Connectors:
  - (external) 1x 4pin
  - (internal) 1x 12pin (to motherboard front panel and motherboard serial header, pinout up-down: JF1-RST-L JF1-RST-R JF1-PWRON-L JF1-PWRON-R JF1-HDDLED-L JF1-HDDLED-R JF1-PWRLED-L JF1-PWRLED-R COM-RTS COM-CTS COM-RXD COM-TXD
  - (internal) 1x 4pin (to power supply 12V and 5V, pinout left-right: GND GND NC GND 12V 5V)
  - (internal) 1x 4pin (to JVS expansion card, pinout left-right: V+ D+ D- V-)
