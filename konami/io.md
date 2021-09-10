# Interfaces

## APC

* Product: TOPS APC CARD

## P2IO

* Product: PWB0000359443 / PWB110526140000
* Connector: USB (host), JAMMA (cab)

## P3IO

* Product: PWB112263690000
* Connectors: JAMMA (cab), custom (COM1, cab), TTL (COM2, cab), 2x TTL (COM3-4, cab),  RGB (cab), 2x RCA (cab), secplug (cab)

## P4IO

* Product: 115710800000 (blue board) / PWB112840930000 (green board)
* Codename: "Cerel"
* Connectors: USB (host), serial (host), serial (cab), custom x4 (cab)
* Firmware families:
  - ACIO name: "BMPU" (ID: 0x0B000000) \[O26\]
    * Generic test and service switches, and general input
    * Known versions: 1.1.2 / Jun 12 2013 19:24:19 / O26

## C02 IO

* GEC02-PWB(A)A
* PCB product: PN0000228708
* case/metal housing: PN0000246977
* case/box cover: PN0000246978
* Interface to main PCB: USB 1.1
* Compatible games: [C02](software/C02.md), [D01](software/D01.md), [E11](software/E11.md),
[ECO](software/ECO.md), [FDD](software/FDD.md), [GLD](software/GLD.md), [HDD](software/HDD.md),
[I00](software/I00.md), [JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md),
[LDJ (only up to 24 included)](software/LDJ.md)

## D01 IO

* Interface to main PCB: USB 1.1
* Compatible games: [D01](software/D01.md), [E11](software/E11.md), [ECO](software/ECO.md),
[FDD](software/FDD.md), [GLD](software/GLD.md), [HDD](software/HDD.md), [I00](software/I00.md),
[JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md), 
[LDJ (only up to 24 included)](software/LDJ.md)

## D55 IO

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/v1004013462`

* GSD55 PWB(K1?) HPST
* Product: PWB11??????????
* Compatible games: D55, F56, K56

## K39 IO

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/u452002755`

* `GUK39-JA`: used in pop'n card dispenser?
* Product: PWB11106490000
* Codename: "Alard"

## USBIO2

* KDE-J
* PCB product: PWB1113692080000, PWB111362080000
  * Case/metal housing: PN00001_1263
* Interface to main PCB: USB 2.0
* Compatible games: [GLD](software/GLD.md), [HDD](software/HDD.md), [I00](software/I00.md),
[JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md), [LDJ (only up to 24 included)](software/LDJ.md)

## KFCA

* Product: PWB114435950000
* Codename: "Nadeshiko"
* Firmware families:
  - ACIO name: "KFCA" (ID: 0x09060000) \[KFC/PAN\]
    * Known versions: 1.0.5 / Aug 30 2011 13:23:47 / PAN
  - ACIO name: "RVOL" (ID: 0x09060001) \[PIX\]

## BIO2

* Product: PWB116784030000
* Codename: "xenolithus"
* Firmware families:
  - BI2A (ID: 0x0D060000)
  - BI2X
* Connectors: USB
* Compatible games: [LDJ (starting 25)](software/LDJ.md)

### BIO2 LDJ sub IO

* Product: PWB116784480000

# Devices

## C02 magnetic card readers

* PN 0000254292
* Compatible games: [C02](software/C02.md), [D01](software/D01.md), [E11](software/E11.md),
[ECO](software/ECO.md)

## DDRS

DDR led spike. Also used in Reflec Beat.

* ACIO name: "DDRS" (ID: 0x05010000)

## H44B

jubeat (H44) lights.

## HBHI

## HDXS

DDR front panel and speaker lights.

* ACIO name: "HDXS" / "HDXB" (ID: 0x04020000)

## HGTH

## ICC

e-AMUSEMENT pass (IC card) reader. Is really two types of devices: the old slot card reader, and the new NFC card reader.

* Product:
  - FRWF-K01A / FRWF-K02B [slot reader]
  - Secure-Tech NS-ARW13T-KNM2 (case) / ARW13T-RS01B-CSW01 (PCB) [NFC reader]
* Firmware families:
  - ACIO name: "ICCA" (ID: 0x03000000) [slot reader]
    * Known versions: 1.1.0 / Oct 26 2005 13:55:03 / FDH/GDJ
  - ACIO name: "ICCB" (ID: 0x03000000) [NFC reader]
    * Known versions: 1.5.1 / Apr 12 2010 09:29:00 / KFC/LDJ
  - ACIO name: "ICCC" [NFC reader]
    * Known versions: 1.7.3 / Oct 05 2012 20:26:53 / L44, 1.7.4 / Feb 27 2013 16:44:51 / PIX/PAN

## J32D

Guitarfreaks/Drummania XG (J32) device.

## KLPA

## MDXF

DDR A (MDX) device.

## NDDB

## PANB

Nostalgia (PAN) panel.

## PJEC

## PJEI
