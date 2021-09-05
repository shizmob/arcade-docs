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

## USBIO2

* Product: PWB1113692080000
* Connectors: USB

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

# Devices

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

## KLPA

## MDXF

## NDDB

## PANB

Nostalgia (PAN) panel.

## PJEC

## PJEI
