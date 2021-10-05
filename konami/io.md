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

[C02 IO](io/c02-io.md)

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
[JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md), [LDJ (up to 24 SINOBUZ)](software/LDJ.md)

## KFCA

* Product: PWB114435950000
* Codename: "Nadeshiko"
* Firmware families:
  - ACIO name: "KFCA" (ID: 0x09060000) \[KFC/NBT/PAN\]
    * Known versions: 1.0.5 / Aug 30 2011 13:23:47 / PAN
  - ACIO name: "KFCA" (ID: 0x09060001) \[PIX\]
    * Referred to as "RVOL"  `#GAME:konami:PIX:modules/libacio_pix.dll`
    * Known versions: 1.6.1 / Oct 21 2015 16:39:52 / PIX

## BIO

* Product: GSO65 PWB(A1)116148170000
* Compatible games: O65, PTL, RTL

## BIO2

* Product: PWB116784030000
* Codename: "xenoliths"
* Firmware families:
  - ACIO name: "BI2A" (ID: 0x0D060000) \[KFC/LDJ/MDX/REC\]
    * Known versions: 1.2.1 / Nov 27 2017 14:48:52
  - BI2X \[S36/SA1/T44/TBS/TCS/TDJ/UFC\]
* Connectors: USB
* Compatible games: KFC (starting Vivid Wave), [LDJ (starting 25 CANNON BALLERS)](software/LDJ.md), MDX (GQMDX-JG 20th anniversary model), REC, S36, SA1, T44, TBS, TCS, TDJ, UFC

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

## EXTIO

Interface board for lighting and individual sensor data in P2IO and P3IO-based DDR cabinets.

* Product: PWB0000373993
* Copyright: 2004 KONAMI

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
  - Secure-Tech NS-ARW13T-KNM2 (case) / ARW13T-RS01B-CSW01 (PCB) / ARW13T-KNM-FM HM (radio) [slot reader]  `#WEB:https://fccid.io/VCTKJ111703250000/Internal-Photos/internal-photos-812722`
* Firmware families:
  - ACIO name: "ICCA" (ID: 0x03000000) [slot reader]
    * Known versions: 1.1.0 / Oct 26 2005 13:55:03 / FDH/GDJ
  - ACIO name: "ICCB" (ID: 0x03000000) [NFC reader]
    * Known versions: 1.5.1 / Apr 12 2010 09:29:00 / KFC/LDJ
  - ACIO name: "ICCC" (ID: 0x03000000) [NFC reader]
    * Known versions: 1.7.3 / Oct 05 2012 20:26:53 / L44, 1.7.4 / Feb 27 2013 16:44:51 / PIX/PAN/TDJ

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
