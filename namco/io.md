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
  - Sipex SP3222EUCY (SSOP16, RS-232 transceiver)
* Connectors:
  - (external) 1x 4pin
  - (internal) 1x 12pin (to motherboard front panel and motherboard serial header, pinout up-down: JF1-RST-L JF1-RST-R JF1-PWRON-L JF1-PWRON-R JF1-HDDLED-L JF1-HDDLED-R JF1-PWRLED-L JF1-PWRLED-R COM-RTS COM-CTS COM-RXD COM-TXD
  - (internal) 1x 7pin (to power supply 12V and 5V, pinout left-right: GND GND NC GND 12V 5V)
  - (internal) 1x 4pin (to JVS expansion card, pinout left-right: V+ D+ D- V-)

## H055 CARD-IF

Banapass card reader. Connects to host via a custom serial port connector, usually labeled "SERIAL 3 (CARD IF)".

* Product: 8918960101 / (8918970101)
* Label: H055 CARD-IF PCB
* Copyright: 2010 NAMCO BANDAI Games Inc.
* Chips:
  - Hitachi HD64F3062BF25V (QFP100, H8 MCU)
  - Toshiba TD62083AFG (SOIC16, 8ch Darlington Sink Driver for the LEDs)
  - Sony RC-S620/S (NFC Reader Module via UART)
  - Sipex SP3222EUCY (SSOP16, RS-232 transceiver)
  - Murata Piezo Buzzer
* Connectors:
  - (external) 1x 3pin (CN2)
  - (external) 1x 9pin (CN1, SERIAL + POWER, pinout left-right: 12V GND COM-RXD COM-TXD COM-RTS COM-CTS COM-GND NC NC)

## H058 TSIF

External interface. Connects to motherboard and exposes a bunch of custom connectors.

* Product: 8920960102 / (8920970102) / 12010769
* Label: H058 TSIF PCB
* Chips:
  - FTDI FT232RL (SSOP28, RS-232 to USB transceiver)
  - Sipex SP3222EUCY (SSOP16, RS-232 transceiver)
* Connectors:
  - (external) 1x 3pin  (CN3, SERIAL1, to SP3222EUCY, pinout left-right: GND T1OUT R1IN)
  - (external) 1x 8pin  (CN6, SERIAL2, to CN4, pinout left-right: 12V GND RXD1 TXD1 RTS1 CTS1 GND1)
  - (external) 1x 3pin  (CN5, SERIAL3, to CN4, pinout left-right: TXD2 RXD2 GND2)
  - (external) 1x 3.5mm (CN2, AUDIO2, to CN1)
  - (internal) 1x 4pin  (CN1, audio, pinout left-right: LINE2_L FAUDIO_JD LINE2_R GND)
  - (internal) 1x 16pin (CN4, serial & front panel, pinout left-right: RXD1 TXD1 RTS1 CTS1 GND1 TXD2 RXD2 GND2 HDDLED+ HDDLED- PWRLED+ PWRLED- PWRON+ PWRON- RESET- RESET+)
  - (internal) 1x 2pin  (CN9, power, pinout left-right: 12V GND)
  - (internal) 1x 5pin  (CN8, USB, pinout left-right: 5V D- D+ D- NC)

## H058 TSIFPLUS

External interface. Connects to motherboard and exposes a custom connector, JVS USB, two LEDs, an on-board jumper (JP2, unpopulated) and a switch (SW1, unpopulated).

* Product: 8920960201 / (8920970201) / 140125415
* Label: H058 TSIFPLUS PCB
* Chips:
  - Hitachi HD64F3672 (QFP48, H8 MCU)
  - "14745 KSS 3LF" (14.745 MHz crystal)
  - Sipex SP485EC (SOIC8, RS-485 transceiver)
  - Sipex SP3222EUCY (SSOP16, RS-232 transceiver)
* Connectors:
  - (external) 1x 7pin  (CN3, SERIAL 3 (CARD IF), pinout left-right: 12V GND RXD1 TXD1 RTS1 CTS1 GND1)
  - (external) 1x USB   (CN4, JV IO (JAMMA))
  - (internal) 1x 20pin (CN2, serial & front panel, pinout up-down left-right: RXD1 TXD1 RTS1 CTS1 GND1 TXD2 RXD2 RTS2 CTS2 NC HDDLED+ HDDLED- PWRLED+ PWRLED- JP2+ JP2- SW2+ SW2- NC NC)
  - (internal) 1x 4pin  (CN1, power, pinout left-right: 5V GND 12V GND)

## ESIF2

External serial interface, revision 2. Looks identical to the [H039 ESIF](#h039-esif). Connects to motherboard serial, and exposes JVS and serial. Likely turns on/resets the motherboard too.

* Product: 8921960100 / (8921970100)
* Label: ESIF2 PCB
* Chips:
  - Hitachi HD64F3672 (QFP48, H8 MCU)
  - "E 14.7456C" "2PK D494I" (14.7456 MHz crystal)
  - Sipex SP485EC (SOIC8, RS-485 transceiver)
  - Sipex SP3222EUCY (SSOP16, RS-232 transceiver)
* Connectors:
  - (external) 1x 4pin
  - (internal) 1x 12pin (to motherboard front panel and motherboard serial header)
  - (internal) 1x 7pin (to power supply 12V and 5V, pinout left-right: GND GND NC GND 12V 5V)
  - (internal) 1x 4pin (to JVS expansion card, pinout left-right: V+ D+ D- V-)

# Boards

## IO

* Product: 2479961102 / (2479971102); 2591982102
* Label: V185 I/O PCB; V291 I/O PCB
* Copyright: NAMCO

## STD CONNECT

* Product: 8523960201 / (8523970201) / A05585
* Label: 汎用 STD CONNECT PCB
* Copyright: 2007 NAMCO BANDAI Games Inc.

## FCA

* Product: 8662969102 / (8662979102)
* Label: FCA PCB
* Copyright: NAMCO

## FCA2

* Product: 8662969200 / (8662979100)
* Label: FCA2(B) PCB

## FCB

* Product: 2582960101 (2582970101)
* Label: V290 FCB PCB

## MIU

* Product: 2512960101 / (2512970101); 8662969301; 2591961001
* Label: V221 MIU PCB; (JV) TMIU PCB; V291 XMIU PCB

## STR

* Product: 2487960103 / (2487970103); 2553960100; 2600960100
* Label: V194 STR PCB; V257 STR PCB; V315 STR PCB

## STR2

* Product: 2609965100 / (2609970100)
* Label: V320 STR2(B) PCB
* Copyright: 2006 NAMCO BANDAI Games Inc.

## STR3

* Product: 8670961500 / (8670971500)
* Label: 汎用（ドライブ））STR3 PCB

## STR4

## NA-JV

* Product: 8682960602 / (8682970602); 26169605
* Label: 汎用 NA-JV PCB; V329 NA-JV PCB
* Copyright: NAMCO

## NA-JV2

* Product: 8682960602 / (8682970602); 8523961000 [sticker]
* Label: 汎用 NAJV2 PCB; 汎用 NAJV2 PCB [sticker]
* Copyright: NAMCO

# NA-JV(S)

* Product: ... / (8682970602); 8682961002 [sticker]
* Label: ...; 汎用(PCB) NA-JV(S) PCB [sticker]
* Copyright: NAMCO

## USIO

* Product: 8682960801 / (8682970801); 2655961101
* Label: 汎用 (PCB) USIO PCB; V371 USIO PCB
* Copyright: 2008 NAMCO BANDAI GAMES Inc.

## USIO(T)

* Product:  8682960902 / (8682970902); 2686962102 [sticker]
* Label: ...; V406 USIO(T) PCB [sticker]
* Copyright: 2010 NAMCO BANDAI Games Inc.

## WIDE USIO

* Product: 1892960100 / (1892970100)
* Label: WIDE USIO PCB
* Copyright: 2014 NAMCO BANDAI Games Inc.
