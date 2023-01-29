## Bubble System

`#MAME:nemesis`

* Release: 1985
* Base: none

## System GX

`#MAME:konamigx`

* Release: 1994
* Base: none

## Tasman

`#MAME:tasman`

* Release: 199?
* Base: [System GX](#system-gx) (loosely)

## GQ System

`#MAME:konamigq`

* Release: 1995
* Base: Sony Playstation 1

## GV System

`#MAME:konamigv`

* Release: 1996
* Base: Sony Playstation 1

Consists of either of the following boards:
* `ZV610 PWB301331`
* `GV999 PWB301949A`: has expansion connector and some newer IC revisions

According to BIOS ROM, runs "Konami OS by T.H.".

## DJ-MAIN

`#MAME:djmain`

* Release: 1997
* Base: [System GX](#system-gx) (loosely)

## M2

`#MAME:konamim2`

* Release: 1997
* Base: 3DO

Based on the 3DO.

## NWK-TR

`#MAME:nwk-tr`

* Release: 1998
* Base: none

## Hornet

`#MAME:hornet`

* Release: 1998
* Base: [NWK-TR](#nwk-tr)

## System 573

`#MAME:ksys573`

* Release: 1998
* Base: Sony Playstation 1

Consist of at least MAIN and either the ANALOG or DIGITAL board:
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

## Twinkle

`#WEB:http://callusnext.com/twinkle.txt #MAME:twinkle`

* Release: 1999
* Base: Sony Playstation 1

Consists of three boards:
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

## Viper

`#MAME:viper`

* Release: 1999
* Base: none

## Firebeat

`#MAME:firebeat`

* Release: 2000
* Base: none

## MET

`#MAME:konamigs`

* Release: 2000
* Base: none

Custom Hitachi SH3-based boards, used for DDR Kids and medal games.

## Python

`#MAME:kpython #WEB:http://callusnext.com/pcbs/ps2_pm.html`

* Release: 2001
* Base: Sony Playstation 2
* HDD: CompactFlash [C18, C27]
* HDD: HDD [C00, C20, D11, E12, E13, F14, E33]
* Games: B08?, C00 / C20 / D11 / E12 / E13 / F14, C18 / C27, C30, E33

Similar to Namco's System 246 and System 256.

## Python 2

* Release: 2004?
* Base: Sony Playstation 2
* Games: D44, E00 / F00, E01, E02 / E03 / F02 / F03 / F32 / F33, FDH / GDJ

Unlike the first Python, based on a retail board using Sony's DNAS protection system.

## `KNM-*`

* Release: 2003 (?)
* Base: PC

IBM embedded boards (日本アイ・ビー・エム株式会社)

**MBD:** PM-845G3/GL/GV  
**STH:** Intel 845G  
**SND:** Realtek ALC202 (AC'97)  

### KNM-845G3-A02

Also known as: "BemaniPC Type 1" (unofficially).

Seemingly identical to the [KNM-845G3-A12](#knm-845g3-a12), for which below specs are; unconfirmed. Used in C02, D01, E11 hardware upgrade kits.  `#DOC:KONAMI:0000252536 #DOC:KONAMI:0000363152`

**CPU:** Intel Celeron 1.8GHz  
**RAM:** 1x ??? (DDR1, PC2100, 256MB)  
**GPU:** ASUS V9180MAGIC/T/64M (AGP, Nvidia GeForce4 MX440-8x, 64MB)  
**Games:** [C02](software/C02.md), [D01](software/D01.md), [E11](software/E11.md), [ECO](software/ECO.md), [FDD](software/FDD.md)  

### KNM-845G3-A11

**CPU:** Intel Celeron 2.0GHz (BX80532RC2000B)  
**RAM:** 2x Kingston KVR400X64C3A/512 (512MB)  
**MBD:** PM-845G3/GL/GV  
**STH:** Intel 845G  
**GPU:** Asus V9570/TD/P/256M/A (Nvidia GeForce FX5700, 256MB)  
**Games:** D00, CLX  
**Sticker:** 27  

### KNM-845G3-A12

Also known as: "BemaniPC Type 1" (unofficially).

Seemingly identical to the [KNM-845G3-A02](#knm-845g3-a02). Used in ECO, FDD hardware upgrade kits.  `#DOC:KONAMI:110033580000`

**PSU:** Delta DPS-180KB (180W, 115/230V AC input)  
**CPU:** Intel Celeron 2.0 GHz (Northwood-128)  
**RAM:** 1x ProMOS Technologies V826632K24SATG-C0 (DDR1, PC2700U, 256MB, "IBM FRU 31P9121")  
**GPU:** ASUS V9180MAGIC/T/N/64M/A (AGP, Nvidia GeForce4 MX440-8x, 64MB)  
**HDD:** (caddy: IMDKN0007123)  
**Games:** [E11](software/E11.md), [ECO](software/ECO.md), [FDD](software/FDD.md)  

### KNM-845G3-A??

Uses Intel Extreme integrated graphics instead of a GeForce GPU.

**CPU:** Intel Celeron 1.8GHz  
**GPU:** Intel Extreme Graphics  
**SND:** Realtek AC'97  
**Games:** C33, D33  

## `EPIA`

* Release: 2002/2003
* Base: PC ([VIA ITX boards])

### EPIA 5000

**MBD:** VIA EPIA-5000  
**CPU:** VIA Eden 533MHz  
**GPU:** Trident CyberBlade 3D  
**Games:** CCB, EGG  

### EPIA M10000

***MBD:** VIA EPIA-M10000  
***CPU:** VIA C3 (1 GHz)  
***GPU:** S3 CastleRock  
**Games:** E99  

## SORD FAB series

* Release: 2004 (FAB-e865), 2006 (FAB-e945), 2007 (FAB-e965), 2009 (FAB-e45), 2011 (FAB-e67)
* Base: PC ([Sord embedded boards](https://www.sord.co.jp/company/corporate/history.html))

### `FAB-e865-KN*`
**MBD:** DFI G4S306-C  
**STH:** Intel 865G  
**BIOS:** Phoenix-Award  

#### FAB-e865-KN001

**Games:** D22

#### FAB-e865-KN002

**CPU:** Intel Pentium 4 2.8GHz  
**GPU:** ATI Radeon 9600XT 128M  
**HDD:** Seagate ST3402111A (40GB)  
**DVD:**  TEAC DV-28E-N  
**Sticker:** A2  
**Games:** G27  

#### FAB-e865-KN003

**CPU:** Intel Celeron 2.5GHz  
**RAM:** 512MB  
**STH:** Intel 865G  
**GPU:** ATI Radeon 9600XT  

#### FAB-e865-KN303

**CPU:** Intel Celeron 2.5Ghz  
**RAM:** 2x Micron MT4VDDT3264AY-335F1 (DDR1, PC2700, 256MB)  
**GPU:** ATI Radeon 9600XT 128M  
**HDD:** Seagate ST3402111A (40GB)  
**CD:**  TEAC CD-224E  
**IO:**  [APC102-000](io.md#apc)  
**Sticker:** A3  
**Games:** F24, IG2, HCK, GGG, FA5, FLY  

#### FAB-e865-KN306

(Name tentative)

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/g1022126807 #WEB:https://page.auctions.yahoo.co.jp/jp/auction/g1028575835`

**DVD:** reader  
**Sticker:** A6  
**Games:** DPU(CAP)  

### `FAB-e945-KN*`
**MBD:** IEI MB-9454-P2VS  
**STH:** Intel 945G  
**SND:** Realtek ALC888  

#### FAB-e945-KN201

**Sticker:** B1  
**CPU:** Celeron D 341 (2.93GHz)  
**GPU:** ATI Radeon X1600 Pro (256 MB)  
**Games:** F56/J56/K56/M56 (STATION/ステーション)  

#### FAB-e945-KN202

**Sticker:** B2  
**Games:** K56 MAIN?  

#### FAB-e945-KN203

**Sticker:** B3  
**CPU:** Pentium 4 (3.40GHz)  
**GPU:** ATI Radeon X1600 Pro (PCIe, 256MB, VGA + S-Video + DVI) (109-A67631-12)  
**RAM:** 2 x 512 MB DDR2  
**Games:** K56 POP?, G65/H65/J65/K65/L65/M65/O65/P65(MAIN)  

#### FAB-e945-KN204A

**CPU:** Pentium 4 (3.40GHz)  
**RAM:** 2 x Micron MT8HTF6464AY053ED7 (512MB, PC4200U)  
**GPU:** ATI Radeon X1600 Pro (PCIe, 256MB, VGA + S-Video + DVI) (109-A67631-12)  
**HDD:** Seagate ST380815AS (80GB, 7200RPM)  
**CD:**  (absent)  
**IO:**  [945APC](io.md#apc)  
**IO:**  eSATA  
**PSU:** AcBel ATX-450C-A2SNN (450W, 100-240V)  
**Sticker:** B4A  
**Games:** GDK  

#### FAB-e945-KN205

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/r1029790798`

Also known as: "BemaniPC Type 2" (unofficially).

**CPU:** Celeron D 341 (2.93GHz)  
**RAM:** 1 x 512 MB 
**GPU:** ATI Radeon X1300  
**Sticker:** B5  
**Games:** [GLD](software/GLD.md), [HDD](software/HDD.md), [I00](software/I00.md), [JDJ](software/JDJ.md), [JDZ](software/JDZ.md), [KDZ](software/KDZ.md)  

#### FAB-e945-KN206

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/u1038929462`

**Sticker:** B6  
**CPU:** Celeron D 341 (2.93GHz)  
**GPU:** Intel GMA 950  
**Games:** F56/J56/K56 (MAIN), G51, G52, H53  

#### FAB-e945-KN209

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/l701319133`

**Sticker:** B9  
**CPU:** Celeron D 341 (2.93GHz)  
**GPU:** ATI Radeon X1600 Pro (PCIe, 256MB, VGA + S-Video + DVI) (109-A67631-12)  
**Games:** G65/H65/J65/K65/L65/M65/O65 (STATION/ステーション?)  

#### FAB-e945-KN210

**Sticker:** B10  
**CPU:** Celeron D 341 (2.93GHz)  
**GPU:** ATI Radeon X1300  
**RAM:** 2 x 512 MB (?)
**Games:** GHL  

### `FAB-e965-KN*`

**MBD:** Toshiba TEM100-01B  
**STH:** Intel Q965  
**SND:** ADI SoundMAX AD1988B (HD Audio)  

#### FAB-e965-KN301

**Sticker:** C1  
**CPU:** Intel Core 2 Duo E6400 (2.13GHz)  
**GPU:** ATI Radeon HD 2600 XT (109-B14831-00 HF) (S/N 180821 800735, P/N 102B1480500 777777) (256 MB, GDDR3)  
**RAM:** 1GBx2  
**Games:** IX8, MX8, KPP, K70/M70/O70/Q70/S70, G23, HPP

#### FAB-e965-KN302

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/1028851239 #WEB:https://twitter.com/KARG175/status/1339943401274294274  #WEB:https://page.auctions.yahoo.co.jp/jp/auction/u1054551394`

**Sticker:** C2  
**GPU:** ATI Radeon HD 2600 XT (109-B14831-00 HF) (256 MB, GDDR3)  
**RAM:** 1GBx2  
**Games:** IWA  

#### FAB-e965-KN303

**CPU:** Intel Core 2 Duo E6400 (2.13GHz)  
**GPU:** ATI Radeon HD 2600 XT (109-B14831-00 HF) (256 MB, GDDR3)  
**RAM:** 512MB/512MBx2/1GBx2  
**HDD:** 160GB  
**Sticker:** C3  
**Games:** JDZ(CHN), KDZ(CHN), I27, J27, K27, HGT, JMA, KMA, LMA, ICK, KCK, KLP  `#WEB:https://page.auctions.yahoo.co.jp/jp/auction/p870019570 #WEB:https://page.auctions.yahoo.co.jp/jp/auction/q1051296570 #CLAIM:erobot`  

#### FAB-e965-KN304

**CPU:** Intel Celeron 440 (2.00GHz) `#GAME:konami-WINDOWS\SYSTEM32\config\SYSTEM`  
**GPU:** ATI Radeon HD 2600 XT (109-B14831-00 HF) `#GAME:konami-WINDOWS\SYSTEM32\config\SYSTEM`  
**RAM:** 512MBx2  
**Sticker:** C4  
**Games:** H24  

#### FAB-e965-KN313

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/1004281047 #WEB:https://page.auctions.yahoo.co.jp/jp/auction/l1048062897 #WEB:https://page.auctions.yahoo.co.jp/jp/auction/p1039201164`

**MBD:** Toshiba TEM100-01B (TOPS BIOS Ver.1.08K1 02/22/10 16:57:28)  
**CPU:** Intel Core 2 Duo E6400 (2.13GHz)  
**GPU:** ATI Radeon HD 5770 (1 GB)
**RAM:** 2x Micron MT8HTF12864AY-667G1 (DDR2, PC2-5300, 1GB)  
**CD:**  -  
**IO:**  [APC103-000G](io.md#apc)  
**IO:**  eSATA + serial header bracket  
**Sticker:** C13  
**Games:** KGG  

### `FAB-e45-*`
#### FAB-e45-KN401

**MBD:** Toshiba TEM110  
**CPU:** Intel Core 2 Quad Q9400 (2.66GHz)  
**GPU:** ATI Radeon HD 5770 (1 GB) (102C0100200 000001)  
**RAM:** 2 x Micron MT8JTF12864AZ-1G1F1 (DDR3, PC3-8500, 1GB)  
**OS:** Windows XP Embedded (SP2)  
**SND:** Realtek ALC887 (HD Audio)  
**Sticker:** D1  
**Games:** I36  

### `FAB-e67-*`
**MBD:** Toshiba TEM130    
**STH:** Intel Q67  
**SND:** Realtek ALC662 `#GAME:konami-WINDOWS\SYSTEM32\config\SYSTEM`  

#### FAB-e67-TP601

**CPU:** Intel Core i7-2600  
**GPU:** AMD Radeon HD 6850 (1 GB)  
**RAM:** 4 GB DDR3  
**OS:** Windows XP Embedded (SP2) [KGG] / Windows Embedded Standard 7 (SP1) [KDM] [MMD] [NDD]  
**Sticker:** E1  
**Games:** KDM, KGG, KPU, NDD, MSH, MMD  
**BIOS:** AMIBIOS Aptio (BIOS Date: 12/20/2011 17:22:34 Ver: 3ABXC)  

#### FAB-e67-KN612

`#WEB:https://page.auctions.yahoo.co.jp/jp/auction/o1033199149 #WEB:https://page.auctions.yahoo.co.jp/jp/auction/x1051529573`

**MBD:** Toshiba TEM130-02A (3ACAF 2.00IV2)  
**CPU:** Intel Core i5-3550S `#GAME:konami-WINDOWS\SYSTEM32\config\SYSTEM`  
**GPU:** Sapphire Radeon HD 7770 GHz Edition (1 GB) `#GAME:konami-WINDOWS\SYSTEM32\config\SYSTEM`  
**RAM:** 2x2GB DDR3-12800  
**IO: ** [APC](io.md#apc)  
**OS:** Windows XP Embedded (SP2) `#GAME:konami-WINDOWS\SYSTEM32\config\SOFTWARE`  
**Sticker:** E2  
**Games:** NCK  

## `IT*`

* Release: 2007 (855) / 2008 (945)
* Base: PC (AOpen embedded boards)

### 855

`#WEB:http://callusnext.com/pcbs/pc_pm.html`

Also known as: "BemaniPC Type 3" (unofficially).

**MBD:** AOpen IT855GME-LX (AOpen i855G*-based?)  
**STD:** Intel 855GME  
**CPU:** Intel Celeron M 370 (1.50GHz)  
**RAM:** 1x Buffalo DD4333-S512HCJ (DDR, 512MB, PC3200U) (pop'n) / 1 GB DDR (Bishi Bashi, Jubeat, Yu-Gi-Oh)  
**GPU:** ATi Radeon 9600 XT (embedded)  
**SND:** Realtek ALC655 (AC'97)  
**IO:** \[M39\] [USB I/O 2](io.md#usbio2)  
**IO:** \[Others\] [P3IO](io.md#p3io)  
**OS:** Windows XP Embedded (SP2) (most games) / Windows XP Embedded (SP3) (I44, 2012 CHN)
**Games:** ID2 / I44 / J44 / K44 / G32 / G33 / H32 / H33 / I32 / I33 / J32 / J33 / K32 / K33 / M39 / H79 / G78 / IBB  
**Ref:** http://k4copious.blog.fc2.com/blog-entry-14.html / http://callusnext.com/pcbs/pc_pm.html  
**BIOS:** Phoenix-Award BIOS  

### 945

Also known as: "HDX-945-??" / "JDX-945-02" / "K32-945-01?" / "K33-945-01?" / "KBR-945-01" / "KFC-945-01" / "BemaniPC Type 4" (unofficially).

**MBD:** AOpen IT945GME_M72 (AOpen i945G*-based?)  
**STD:** Intel 945GME  
**CPU:** Intel Celeron M 440 (1.86GHz)  
**RAM:** 2x Buffalo D2N667C-X512HEJ (SODIMM DDR2, 512MB, PC2-5300S)  / 2x1GB  
**GPU:** ATI Radeon E2400 (256 MB, MXM-II) (RH EDG)  
**SND:** Realtek ALC883 (HD Audio)  
**HDD:** \[MDX\] Seagate ST500DM002 (SATA 3.5", 500GB, 7200RPM)  
**IO:** \[HDX/JDX/KDX/MDX\] [P3IO](io.md#p3io)  
**IO:** \[J32/J33/K32/K33/L32/L33/KBR/LBR\] [P4IO](io.md#p4io)  
**IO:** \[KFC\] [KFCA](io.md#kfca)  
**OS:** Windows XP Embedded (SP2) (most games) / Windows XP Embedded (SP3) (I44, 2012 CHN)
**Games:** HDX, J32, J33, JDX, K32, K33, KBR, KDX, L32, L33, LBR, MDX, KFC, I44(CHN), J44, K44, IMS, JMP, JC9, KPM  
**BIOS:** Phoenix-Award BIOS (07/16/08)  

## `ADE-*`

* Release: 2012 (HM65) / 2015? (76) / 2016 (ADE)
* Base: PC ([Ennocom embedded boards](https://www.ennoconn.com/producttype_en-us_0_21_1.html))

### HM65

Also known as: "ITHM65", "ITHM65_E4690".  `#DOC:KONAMI:116245360000`

**MBD:** Ennoconn ADE-704A  
**STH:** Intel HM65  
**CPU:** Intel Celeron B810  
**RAM:** 1 or 2x 2GB DD3 SODIMM  
**GPU:** AMD Radeon E4690  
**HDD:** WDC WD3200LPCX (320GB) [LDJ] [KFC] [M32] [M33] [M39] [MBR]
**SSD:** Intel SSDSA2CT040G3 2.5" (SATA 2.5", 40GB) [L44]
**SND:** Realtek ALC888 Series
**IO:** \[KFC/NBT/PAN\] [KFCA](io.md#kfca)    
**IO:** \[LDJ\] [USB I/O 2](io.md#usbio2)  
**IO:** \[M39\] [USB I/O 2](io.md#usbio2)  
**IO:** \[M32/M33/MDX\] [P4IO](io.md#p4io)  
**OS:** Windows XP Embedded (SP2) [LDJ] [MBR] [MDX], Windows XP Embedded (SP3) [L44] [LMM] [NBF], Windows Embedded 7 Standard (SP1) [PAN] [M32] [M33] [NBT]  
**Games:** KFC, L44, [LDJ](software/LDJ.md), M32, M33, M39, MBR, MDX, NBF, NBT, PAN, LPH, NSM, LMM  
**BIOS:** AMIBIOS

### 76

**MBD:** Ennoconn ADE-704B  
**STH:** Intel HM76  
**CPU:** Intel Celeron 1020E  
**RAM:** 1x ??? (DDR3 SODIMM, 2GB)  
**GPU:** AMD Radeon E6760  
**HDD:** WDC WD3200LPCX (320GB) [KFC]
**SSD:** ? [KFC] (SEA mini cab)  
**SND:** Realtek ALC888 Series  
**IO:** \[KFC/PAN\] [KFCA](io.md#kfca)   
**OS:** Windows XP Embedded (SP2) [KFC], Windows Embedded 7 Standard (SP1) [KFC] (SEA mini cab) [NCG] [OSP]
**Games:** KFC, NCG, PAN, OSP, PTL  
**BIOS:** AMIBIOS  
**Ref:** https://twitter.com/ham56p/status/1115528175142850561, https://page.auctions.yahoo.co.jp/jp/auction/o1010920842

### ADE-6291

Also known as: "ADE".

**MBD:** Ennoconn ADE-6291  
**APU:** AMD RX-421BD  
**HDD:** [KFC/PAN?/L44?/M32?/M33?/REC?/MDX?] WDC WD3200LPCX (320GB)  
**SSD:** [LDJ] innodisk 3ME2 mSATA (256GB)  
**SSD:** [L44/Others] innodisk 3MG2-P SATA  
**SND:** Realtek ALC888S
**IO:** \[L44/M32/M33\] [P4IO](io.md#p4io)  
**IO:** \[KFC/PAN\] [KFCA](io.md#kfca)   
**IO:** \[LDJ/MDX\] [BIO2(BI2A)](io.md#bio2)  
**IO:** \[REC\] 2x [BIO2(BI2A)](io.md#bio2)  
**Games:** KFC, L44, [LDJ](software/LDJ.md), M32, M33, MDX (New White/Gold), PAN, REC, G52, P65, S65  
**BIOS:** AMIBIOS  
**Note #1:** Two revisions exist for this board: ADE-6291 V1.0 [M32] [M33] [L44] / ADE-6291 V1.1 [LDJ] [MDX] [REC] [KFC]  
**Note #2:** ADE-6291 V1.1 has a 2-pin battery connector besides the PCIe slot.  
**Note #3:** Three BIOS revisions exist for this board: R100 (09/07/2016), R110 (02/14/2017), and R120 (06/08/2017)

## RICOH
(name tentative)

* Release: 2006/2007
* Base: PC

### MFC

**MBD:** RICOH IT2  
**CPU:** Intel Celeron M 410 (1.46GHz)  
**GPU:** Intel GMA 950  
**STH:** Intel 945GM  
**Games:** GK9, HK9, IK9, KK9, KBI  
**OS:** Windows XP Embedded (SP2)  
**BIOS:** AMIBIOS 8  

## Misc

### MB-875-M10
(name tentative)

* Release: 2004/2005
* Base: PC

**MBD:** JDS (Japan Data System) MB-875-M10  
**CPU:** Intel Celeron 2.0 GHz (Northwood-128)  
**GPU:** ATI Mobility Radeon 9600 (M10, 128 MB VRAM)  
**STH:** Intel 875P  
**SND:** VIA AC'97  
**Games:** J55, K55  

### Raw Thrills
* Release: 2008 (Optiplex 740) / 2010 (Optiplex 580)
* Base: PC

## Optiplex 740
**CPU:** AMD Athlon 64 X2 4400+  
**GPU:** ATI Radeon HD 2400 Pro  
**STH:** NVIDIA nForce 430  
**SND:** ADI SoundMAX (HD Audio)  
**OS:** Windows XP Embedded (SP2)  
**Games:** HDX (US/EU)  

## Optiplex 580
**CPU:** AMD Athlon II X2 240  
**GPU:** ATI Radeon HD 4200  
**STH:** AMD 785G  
**SND:** Realtek ALC269 (HD Audio)  
**OS:** Windows XP Embedded (SP2)  
**Games:** JDX (US/EU)  

### GXKC1-CA
(name tentative)
* Release: 2010/2011
* Base: PC

**MBD:** Pegatron IPXPV  
**CPU:** Intel Atom D510 (1.66GHz)  
**GPU:** NVIDIA ION  
**STH:** Intel NM10  
**SND:** Realtek ALC662 (HD Audio)  
**OS:** Windows XP Embedded (SP3)  
**Games:** KC1 (CHN)  

### R10

* Release: 2015 (?)
* Base: PC (iEi embedded boards)

**MBD:** iEi KINO-KBN-i2-4201-R10-KNM VER 1.0  
**APU:** AMD GX-420CA (GE420CIAJ44HM)  
**RAM:** 1x Buffalo D3N1600-LS4GHAJ (SODIMM DDR3, 4GB, PC3L-12800S)  
**SSD:** innodisk 3ME2 mSATA (64GB) \[PIX\] / ??? "M064GPSN804TGJN0-PH" (64GB, mSATA, Phison PS3108 controller, S8FM07.9 firmware) \[O26\]  
**SND:** Realtek ALC892  
**IO:** [P4IO](io.md#p4io)  
**Games:** O26, OTM, PIX, R66, KSF  
**BIOS:** AMIBIOS Aptio 4.6.5.4 (V2C9AD13.rom, 11/12/2014 15:43:39)  
**OS:** Windows Embedded Standard 7 (SP1) [O26] [PIX] [R66]  

### X10SLQ

(name tentative)

* Release: 2017/2018
* Base: PC (Supermicro server boards)

**MBD:** Supermicro X10SLQ  
**STH:** Intel Q87  
**CPU:** Intel Core i3-4330 (3.5GHz) [QBG] [KFC]  
**CPU:** Intel Core i5-4590S (3.0GHz) [RBC] [MDX] `#WEB:https://twitter.com/iMp95/status/1608406532705902597`  
**RAM:** 2 x Innodisk DDR3L-1600 4GB (M3UT-4GMSBLPC-P) [KFC] [MDX] `#WEB:https://twitter.com/iMp95/status/1608406532705902597`  
**RAM:** 2 x Innodisk DDR3-1600 4GB (M3UW-4GSSBC0C-E) [RBC]  
**GPU:** GIGABYTE GV-N1050D5-2GD (Nvidia GeForce GTX 1050) [QBG] [KFC] [RBC]  
**GPU:** GIGABYTE GV-N1650IXOC-4GD (Nvidia GeForce GTX 1650) [QBG] (Replacement)  
**GPU:** Intel HD Graphics 4600 (1.25GHz) [MDX] `#WEB:https://twitter.com/iMp95/status/1608406532705902597`  
**HDD:** WDC WD3200LPCX (320GB) [KFC]  
**HDD:** WDC WD10EFRX (1 TB) [MDX] `#WEB:https://twitter.com/iMp95/status/1608406532705902597`  
**SND:** Realtek ALC888S  
**IO:** [BIO2(BI2A)](io.md#bio2)  
**Games:** KFC (VW), QBG, RBC, MDX  
**PSU:** Supermicro PWS-404-PQ (400W) [MDX] `#WEB:https://twitter.com/iMp95/status/1608406532705902597`  
**BIOS:** AMIBIOS Aptio 2.15.1236 (Supermicro X10SLQ BIOS Date:01/20/2017 Rev:2.2a for KAM 09/13/2017)  
**OS:** Windows Embedded Standard 7 (SP1)  

## ARESPEAR

* Release: 2019
* Base: PC (Konami boards)

### C300 (Xonar AE)

(Name for its home variation. Name for actual arcade hardware is tentative)

**MBD:** Supermicro SuperO MBD-C7B360-CB-MW-O custom variant (microATX)  
**STH:** Intel B360  
**CPU:** Intel Core i5-9400F  
**RAM:** 1x Innodisk M4US-8GSSKCRG-S (8GB DDR4 2133 DIMM)  
**GPU:** GIGABYTE GV-N1650IXOC-4GD (Nvidia GeForce GTX 1650)  
**SSD:** Innodisk 3ME3 DES25-B56D08BC1QC (SATA 2.5", 256GB)  
**SND:** ASUS Xonar AE  
**IO:** [BIO2(BI2X)](io.md#bio2)  
**Games:** TDJ, UFC  
**OS:** Windows 10 IoT Enterprise LTSC 2019  
**Ref:** https://www.konami.com/amusement/arespear/desktops/c300/index.html


### C300

(Name for its home variation. Name for actual arcade hardware is tentative)

**MBD:** Supermicro SuperO MBD-C7B360-CB-MW-O custom variant (microATX)  
**STH:** Intel B360  
**CPU:** Intel Core i5-9400F  
**GPU:** GIGABYTE GV-N1650IXOC-4GD (Nvidia GeForce GTX 1650)  
**SSD:** WDC WD3200LUCT (320GB) [TBS] [UJK]  
**SND:** Realtek ALC892  
**Games:** TBS, UKS, UJK  
**OS:** Windows 10 IoT Enterprise LTSC 2019  
**Ref:** https://www.konami.com/amusement/arespear/desktops/c300/index.html  

### C700

(Name for its home variation. Name for actual arcade hardware is tentative)

**MBD:** Supermicro C7Z370-CG-L  
**STH:** Intel Z370  
**CPU:** Intel Core i7-9700F  
**GPU:** GIGABYTE GV-N3070EAGLE OC-8GD (Nvidia GeForce RTX 3070)  
**SND:** Realtek ALC1150  
**Games:** UDN  
**Note:** Despite Arespear C700 using an MSI RTX 2070 Super and Xonar AE, UDN's PCB uses a GIGABYTE RTX 3070 and uses onboard audio instead.  
**Ref:** https://www.konami.com/amusement/arespear/desktops/c700/index.html  
