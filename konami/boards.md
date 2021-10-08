## System GX

`#MAME:konamigx`

## Bubble System

## DJ-MAIN

`#MAME:djmain`

Based on the [System GX](#system-gx).

## M2

`#MAME:konamim2`

Based on the 3DO.

## GV System

`#MAME:konamigv`

Sony Playstation 1-based board. Consists of either of the following boards:
* `ZV610 PWB301331`
* `GV999 PWB301949A`: has expansion connector and some newer IC revisions

According to BIOS ROM, runs "Konami OS by T.H.".

**MBD:** Sony Playstation 1 (custom)  

## NWK-TR

`#MAME:nwk-tr`

## System 573

`#MAME:ksys573`

Sony Playstation 1-based board. Consist of at least MAIN and either the ANALOG or DIGITAL board:
* GX700-PWB(A)B: main
* GX700-PWB(D):  security cartridge board

And possibly any of the following boards:
* GX700-PWB(F):  analog I/O
* GX700-PWB(J):
* GX700-PWB(K)A: analog I/O used in F24, similar to GX700-PWB(F)
* GX894-PWB(B)A: digital I/O
* GE765-PWB(B)A: analog I/O used in 765/865/889

Optional external boards:
* GE877-PWB(C):  gachagachamp aux input
* GN845-PWB(B):  DDR stage board
* G????:         network unit expansion

Note that even with the same I/O board, it can still be wired up differently to the external connector panel on a per-game basis.

Has twice as much RAM (4MB) as a retail PS1. According to BIOS ROM, runs "Konami OS by T.H.".

**MBD:** Sony Playstation 1 (custom)  
**IO:** [MAIN] IDE, 10pin (analog), 12pin (ext-out), 10pin (ext-in), VGA, 4pin (stereo out), 80pin (aux), 4pin (CD-DA input), parallel 44-pin (security), 4pin (CD power), 2pin (fan), 6pin (power), 30pin, USB (IO), RCA  

## Hornet

Seemingly based on the [NWK-TR](#nwk-tr).

## Twinkle

References:
* http://callusnext.com/twinkle.txt
* https://github.com/mamedev/mame/blob/master/src/mame/drivers/twinkle.cpp

Sony Playstation 1-based board. Consists of three boards:
* GQ751-PWB(A2): TWINKLE/MAIN
* GQ860-PWB(A1): TWINKLE/SUB2 (VIDEO)
* GQ863-PWB(A2): TWINKLE/SPU  (SOUND, HDD)

Has twice as much RAM (4MB) as a retail PS1. According to BIOS ROM, runs "Konami OS by T.H.".

**MBD:** Sony Playstation 1 (custom)  
**IO:**  [MAIN, front] RS232, security IC, parallel  
**IO:**  [MAIN, back]  RS232 (serial, DVD), miniDIN, ethernet (serial, I/O), parallel, power  
**IO:**  [SUB2, back]  composite, miniDIN, composite, VGA, power  
**IO:**  [SPU, front]  IDE  
**IO:**  [SPU, back]   RCA, RCA, power  
**CD:**  Panasonic CR-505-BCM (SCSI)  
**HDD:**  Maxtor 2B020H1 (541DX, 5400RPM, 20GB; may depend per game)  
**DVD:** Victor XV D701  

A DVD player is used to play back mpeg encoded Video CDs and DVDs. The decoded video is forwarded
via composite input to the main unit and blit into the UI by software.

## Firebeat

## Viper

## MET

`#MAME:konamigs`

Custom Hitachi SH3-based boards, used for DDR Kids and medal games.

## Python

Sony Playstation 2-based board. Based on a development system. Similar to Namco's System 246 and System 256.

## Python 2

Sony Playstation 2-based board. Unlike the first Python, based on a retail board using Sony's DNAS protection system.

## `KNM-*`

IBM embedded boards (日本アイ・ビー・エム株式会社)

### KNM-845G3-A02

Also known as: "BemaniPC Type 1" (unofficially).

Seemingly identical to the [KNM-845G3-A12](#knm-845g3-a12), unsure for which below specs are. Used in C02, D01, E11 hardware upgrade kits.  `#DOC:KONAMI:0000252536 #DOC:KONAMI:0000363152`

**CPU:** Intel Pentium 2.4 2.4 Ghz  
**RAM:** 1x ??? (DDR1, PC2100, 256MB)  
**MBD:** PM-845G3/GL/GV?  
**STH:** Intel 845G  
**GPU:** ASUS V9180MAGIC/T/64M (AGP, Nvidia GeForce MX4400, 64MB)
**SND:** Realtek AC'97  
**Games:** [C02](software/C02.md), [D01](software/D01.md), [E11](software/E11.md), [ECO](software/ECO.md), [FDD](software/FDD.md)  

### KNM-845G3-A11

**CPU:** Intel Celeron 2.0GHz (BX80532RC2000B)  
**RAM:** 2x Kingston KVR400X64C3A/512 (512MB)  
**MBD:** PM-845G3/GL/GV  
**STH:** Intel 845G  
**GPU:** Asus V9570/TD/P/256M/A (Nvidia GeForce FX5700, 256MB)  
**Games:** D00  
**Sticker:** 27  

### KNM-845G3-A12

Also known as: "BemaniPC Type 1" (unofficially).

Seemingly identical to the [KNM-845G3-A02](#knm-845g3-a02), unsure for which below specs are. Used in ECO, FDD hardware uprade kits.  `#DOC:KONAMI:110033580000`

**CPU:** Intel Pentium 2.4 2.4 Ghz  
**RAM:** 1x ??? (DDR1, PC2100, 256MB)  
**MBD:** PM-845G3/GL/GV?  
**STH:** Intel 845G  
**GPU:** ASUS V9180MAGIC/T/64M (AGP, Nvidia GeForce MX4400, 64MB)
**SND:** Realtek AC'97  
**Games:** [ECO](software/ECO.md), [FDD](software/FDD.md)  

## `FAB-*`

Sord embedded boards: https://www.sord.co.jp/company/corporate/history.html

### FAB-e865-KN003

**CPU:** Intel Celeron 2.5GHz  
**RAM:** 512MB  
**STH:** Intel 865G  
**GPU:** ATI Radeon 9600XT  

### FAB-e865-KN303

**MBD:** G4S306-C (Phoenix AWARDBIOS)  
**STH:** Intel 865G  
**CPU:** Intel Celeron 2.5Ghz  
**RAM:** 2x Micron MT4VDDT3264AY-335F1 (DDR2, PC2700, 256MB)  
**GPU:** ATI Radeon 9600XT 128M  
**HDD:** Seagate ST3402111A (40GB)  
**CD:**  reader  
**IO:**  [APC102-000](io.md#apc)  
**Sticker:** A3  
**Games:** F24  

### FAB-e945-KN201

**Sticker:** B1  
**Games:** K56 ステーション?  

### FAB-e945-KN202

**Sticker:** B2  
**Games:** K56 MAIN?  

### FAB-e945-KN203

**Sticker:** B3  
**Games:** K56 POP?  

### FAB-e945-KN204

?

**Sticker:** B4A
**Games:** GDK  

### FAB-e945-KN205

Also known as: "BemaniPC Type 2" (unofficially).

**CPU:** Pentium 4 2.5GHz  
**RAM:** 512MB PC2700  
**GPU:** ATI Radeon X1300  
**SND:** Realtek HD  
**Sticker:** B5  
**Games:** [GLD](software/GLD.md), [HDD](software/HDD.md), [I00](software/I00.md), [JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md)  

### FAB-e945-KN209

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/l701319133`

**Sticker:** B9  
**Games:** L65, M65  

### FAB-e945-KN210

**Sticker:** B10  
**Games:** GHL  

### FAB-e965-KN301

**MBD:** Toshiba TEM100-01B    
**Sticker:** C1  
**Games:** KPP, O70/Q70, G23  

### FAB-e965-KN303

**MBD:** Toshiba TEM100-01B  
**CPU:** Intel Core 2 Duo 2.13GHz  
**RAM:** 512MB/512MBx2/1GBx2  
**HDD:** 160GB  
**Sticker:** C3  
**Games:** HGT, LMA, JMA  `#WEB:https://page.auctions.yahoo.co.jp/jp/auction/p870019570`  

### FAB-e965-KN304

?

**Sticker:** C4  
**Games:** H24  

### FAB-e965-KN313

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/1004281047`

**MBD:** Toshiba TEM100-01B (TOPS BIOS Ver.1.08K1 02/22/10 16:57:28)  
**CPU:** Intel Core 2 Duo 2.13 GHz  
**RAM:** 2x Micron MT8HTF12864AY-667G1 (DDR2, PC2-5300, 1GB)  
**CD:**  -  
**IO:**  [APC103-000G](io.md#apc)  
**IO:**  eSATA + serial header bracket  
**Sticker:** C13  
**Games:** KGG  

### FAB-e67-TP601

**MBD:** Toshiba TEM130  
**Games:** KDM, KPU  

### FAB-e67-KN612

**Sticker:** E2  
**MBD:** Toshiba TEM130  
**Games:** NCK  

## `IT*`

AOpen embedded boards.

### 855

Also known as: "BemaniPC Type 3" (unofficially).

**MBD:** AOpen IT855GME-LX (AOpen i855G*-based?)  
**CPU:** Intel Celeron M 370  
**RAM:** 1x Buffalo DD4333-S512HCJ (DDR, 512MB, PC3200U)  
**GPU:** ATi Radeon 9600 XT (embedded)  
**IO:** \[M39\] [USB I/O 2](io.md#usbio2)  
**IO:** \[Others\] [P3IO](io.md#p3io)  
**Games:** ID2 / I44 / J44 / K44 / G22 / G33 / H32 / H33 / I32 / I33 / J32 / J33 / K32 / K33 / M39  
**Ref:** http://k4copious.blog.fc2.com/blog-entry-14.html / http://callusnext.com/pcbs/pc_pm.html  

### 945

Also known as: "JDX-945-02" / "KFC-945-01" / "BemaniPC Type 4" (unofficially).

**MBD:** AOpen IT945GME_M72 (AOpen i945G*-based?)  
**CPU:** AMD Athlon X2 4400+  
**RAM:** 2x Buffalo D2N667C-X512HEJ (SODIMM DDR2, 512MB, PC2-5300S)  
**GPU:** ATi E2400 MXM-II 256MB RH EDG  
**HDD:** \[MDX\] Seagate ST500DM002 (SATA 3.5", 500GB, 7200RPM)  
**IO:** \[JDX/KDX/MDX\] [P3IO](io.md#p3io)  
**IO:** \[KFC\] [KFCA](io.md#kfca)  
**Games:** JDX, KDX, MDX, KFC  

## `ADE-*`

Ennocom embedded boards: https://www.ennoconn.com/producttype_en-us_0_21_1.html
  
### HM65

Also known as: "ITHM65", "ITHM65_E4690".  `#DOC:KONAMI:116245360000`

**MBD:** ADE-704A  
**STH:** Intel HM65  
**CPU:** Intel Celeron B810  
**RAM:** 1 or 2x 2GB DD3 SODIMM  
**GPU:** AMD Radeon E4690  
**SSD:** Intel SSDSA2CT040G3 2.5" (SATA 2.5", 40GB)  
**IO:** \[KFC/NBT/PAN\] [KFCA](io.md#kfca)    
**IO:** \[LDJ\] [USB I/O 2](io.md#usbio2)  
**IO:** \[M39\] [USB I/O 2](io.md#usbio2)  
**IO:** \[M32/M33/MDX\] [P4IO](io.md#p4io)  
**Games:** KFC, L44, [LDJ](software/LDJ.md), M32, M33, M39, MBR, MDX, NBF, NBT, PAN  

### ADE-704B

(name tentative)

**MBD:** ADE-704B  
**CPU:** Intel Celeron 1020E  
**RAM:** 1x ??? (DDR3 SODIMM, 2GB)  
**GPU:** AMD Radeon E6760  
**HDD:** WDC WD3200LPCX (320GB)  
**IO:** \[KFC/PAN\] [KFCA](io.md#kfca)   
**Games:** KFC, NCG, PAN  
**Ref:** https://twitter.com/ham56p/status/1115528175142850561  
 
### ADE-6291

Also known as: "ADE".

**MBD:** ADE-6291  
**APU:** AMD RX-421BD  
**HDD:** [KFC/PAN?/L44?/M32?/M33?] WDC WD3200LPCX (320GB)  
**SSD:** [Others] innodisk 3ME2 mSATA (256GB)  
**IO:** \[L44/M32/M33\] [P4IO](io.md#p4io)  
**IO:** \[KFC/PAN\] [KFCA](io.md#kfca)   
**IO:** \[LDJ/MDX\] [BIO2(BI2A)](io.md#bio2)  
**IO:** \[REC\] 2x [BIO2(BI2A)](io.md#bio2)  
**Games:** KFC, L44, [LDJ](software/LDJ.md), M32, M33, MDX (Gold), PAN, REC  

## Misc

### R10

**MBD:** iEi KINO-KBN-i2-4201-R10-KNM VER 1.0  
**APU:** AMD GX-420CA (GE420CIAJ44HM)  
**RAM:** 1x Buffalo D3N1600-LS4GHAJ (SODIMM DDR3, 4GB, PC3L-12800S)  
**SSD:** innodisk 3ME2 mSATA (64GB) \[PIX\] / ??? "M064GPSN804TGJN0-PH" (64GB, mSATA, Phison PS3108 controller, S8FM07.9 firmware) \[O26\]  
**IO:** [P4IO](io.md#p4io)  
**Games:** O26, PIX  

### X10SLQ

(name tentative)

**MBD:** Supermicro X10SLQ  
**STH:** Intel Q87  
**CPU:** Intel Core i3-4330 3.5GHz  
**RAM:** 2x Innodisk DDR3L-1600 4GB  
**GPU:** GIGABYTE Nvidia GeForce GTX 1050 2GB  
**HDD:** WDC WD3200LPCX (320GB)  
**IO:** [BIO2(BI2A)](io.md#bio2)  
**Games:** KFC (VW)  

## ARESPEAR

Konami's own gaming PCs.

### C300

(name tentative)

**MBD:** Supermicro SuperO MBD-C7B360-CB-MW-O custom variant (microATX)  
**STH:** Intel B360  
**CPU:** Intel Core i5-9400F  
**RAM:** 1x Innodisk M4US-8GSSKCRG-S (8GB DDR4 2133 DIMM)  
**GPU:** GIGABYTE GV-N1650IXOC-4GD (Nvidia GeForce GTX 1650)  
**SSD:** Innodisk 3ME3 DES25-B56D08BC1QC (SATA 2.5", 256GB)  
**SND:** ASUS Xonar AE  
**IO:** [BIO2(BI2X)](io.md#bio2)  
**Games:** TDJ, UFC  
