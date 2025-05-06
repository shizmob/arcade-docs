
# Proprietary
## PolyGameMaster (PGM) `#MAME:pgm.cpp`
**CPU**: Motorola 68HC000FN20 @ 20MHz (main); Zilog Z80 @ 8.468MHz (sound); IGS027A (customized ARM processor with internal ROM, coprocessor in some game cartridges)

**RAM**: Epson SRM2B256SLMX55 8K x8 SRAM (x4, SOP28); Unicorn Microelectronics UM6164DS-12 8K x8 SRAM (x2, SOJ28); Unicorn Microelectronics UM61256FS-15 32K x8 SRAM (x3, SOJ28)

**Graphics:** ASIC, IGS023/IGS026, 448x224, 15-bit color, 59.185606 Hz/15KHz

**Sound:** ICS WaveFront 2115 Wavetable midi synthesizer

**Storage:** ROM cartridges

## PolyGameMaster 2 (PGM2) `#MAME:pgm2.cpp`
**CPU**: IGS036, customized ARM9 @ 100MHz? (main); Renesas R5F21256SN microcontroller (IC card controller)

**RAM**: IS61LV25616AL, 256Kx16 SRAM

**Graphics**: ASIC, IGS037, 512x240, 59.8 Hz

**Sound:** Yamaha YMZ774-S DSP @ 16.384Mhz

**Storage**: ROM chips 

**Extra:** IC card readers
## PolyGameMaster 3 (PGM3)`#MAME:pgm3.cpp #WEB:https://www.arcadebelgium.net/t4958-knights-of-valour-3-hd-sangoku-senki-3-hd`

**CPU:** SOCLE SOC38, customized ARM1176 @ 800MHz?

**RAM:** 2GB

**Graphics:** ? 800x600 / 1280x720

**Storage:** ROM cartridges (game); IC cards (player savedata)

**Extra:** IC card readers

## MA1000
(There is little to no information about this board yet.)

**Games:**
* Drummer Kids
* Go Go Pony
* Dolphin Stars
* Marine Treasures Single

## GP1
(name tentative; using the logo on the top of the board as its name)

Mostly used for slot machines and redemption games.

For Ocean King series, development of hardware or software has probably been outsourced to another company called Yuehua Software (YHS) as its logo has been printed on the case, but the game is still released under the IGS brand and making use of ASICs from IGS.

There is little to no information about this board yet.

**Storage:** SD Card ? & USB-OTG ?

**Games:**
* Ocean King 2 series (slot machines)
* Ocean King 3 series (slot machines)
* Halloween Night (M203CN/V204CN/M880CN/M204CN) (redemption game, possible to be converted to slot machine)
* Trick or Treat (M800CN?) (redemption game, possible to be converted to slot machine)
* Harpoon Lagoon (ICE) (replacement PCB)
* 西遊爭霸/鬥戰勝佛 (MD401CN?)
* 西遊爭霸2：大聖歸來 (MD109MO)
* 天天向前GO (M108CN)
* 淘氣鯊 (S101CN)

## GP2
There is little to no information about this board yet.

**CPU:** Qualcomm Snapdragon 845 ?

**OS:** Android ?

# PC-Based

## pre E-Series
### IGS Osprey `#MAME:igspc.cpp`
(name tentative; name is found on the motherboard's BIOS as a string)

**CPU:** Geode GX 533 (400 MHz)

**Games:** EZTouch 2006? (China), EZTouch 2005

**SND:** Realtek (AC'97)

**OS:** Red Hat Linux (32-bit, using Linux kernel 2.4.24)

**Note:** Osprey is the codename for the AMD Geode GX DB533 developmental board in which this board is mostly based off.

## E-series
### E1000
**Motherboard:** IGS NX MB E1000

**CPU:** AMD Geode NX 1500 (1 GHz)

**GPU:** Nvidia GeForce 4 MX IGP

**Chipset**: Nvidia nForce2 IGP

**Southbridge:** Nvidia MCP2-T

**Storage:** CompactFlash cards

**SND:** Realtek ALC655 (AC'97)

**OS:** LFS Linux 

**BIOS:** customized Phoenix-Award BIOS v6.00PG.
* 01/09/2007-nVidia-nForce-6A61BPA9C-00  
Other BIOS revisions may exist

**Games:**
* Percussion Master
* Percussion Master Plus
* Percussion Master 2
* Rock Fever 5

### E2000
**Motherboard:** I-JOIN E2000 (IBASE OEM)  
There are two variants:
* E2000-C6-V256: Has Celeron M 600MHz onboard
* E2000-V256: Has a PGA479 socket with Celeron M 370 (1.5 GHz) attached.  
Has two sub-variants, differences unknown but similar:
** IGS MB NX E2000C [SD2]
** IGS MB NX E2000D [WeDo]

**CPU:**
* Intel Celeron M (600MHz, SL8FN) (onboard) [E2000-C6-V256]
* Intel Celeron M 370 (1.5GHz, SL8MM) (socketed) [E2000-V256]

**GPU:** Nvidia GeForce 6200 (256 MB, GDDR2) [GF-6200-AGP N-A1]

**RAM:** 2 x DDR1 slot. Memory sizes may differ depending on games
* DSL 2 x 256 MB (512 MB) DDR-333 [Pirate Revenge]
* DSL 1 GB DDR-333 [WeDo]

**Chipset:** Intel 852GME

**Storage:**
* CompactFlash card
* IDE-based hard drives are also possible thru IDE connector

**SND:** Realtek ALC655 (AC'97)

**NETWORK:** Intel 82801DB PRO/100 VE (CNR) Ethernet

**OS:** LFS Linux (kernel 2.4.31)

**BIOS:** customized Phoenix-Award BIOS v6.00PG.  

There are two known BIOS revisions of this board, though both share the same BIOS date but have different VBIOS revisions.  

The A1 BIOS is one of the first BIOSes to ship with first batches of the board (coming with its first games like Go Go Ball, Pirate Revenge and Speed Driver 2), while the A11 BIOS is more common on newer batches of the boards.  

* 07/03/2007-i852-W83627HF-6A69YILTC-00 [A1] [A11]

**VBIOS:**
* A1: NV44A P382 VGA BIOS Version 5.44.A2.10.00 (07/03/07)
* A11: NV44A P382 VGA BIOS Version 5.44.A2.10.00 (02/22/08)

**Games:**
```
    E2000-C6-V256   - Panda Family (2009)
    E2000-C6-V256   - Rock Fever 5 (replacement/newer PCB) (2008)
    E2000-C6-V256   - Percussion Master Plus (replacement/newer PCB) (2007?)
    E2000-C6-V256   - Percussion Master 2008 (replacement/newer PCB) (2008)
    E2000-C6-V256   - Gold Captain (航海小勇士) (2009)
    E2000-C6-V256   - Submarine Crisis (2008)
    E2000-C6-V256(?)- Vibraphone (铁琴: 第一乐章) (2010)
    E2000-V256      - Pirate Revenge (怒海英豪) (2007)
    E2000-V256      - We Dancing Online (2009)
    E2000-V256      - We Dancing Online 2 (Plus) (2010)
    E2000-V256      - Speed Rider (2009)
    E2000-V256      - Speed Driver 2: Overtake (2007)
    E2000-V256      - 海遊漁 (China)
```

**Notes:**
* BIOS can be accessed via Ctrl+D at boot-up during the black BIOS splash screen.

### E2100
**Motherboard:** Advantech DES-BT01

**BIOS:** Customized Phoenix-AwardBIOS v6.00PG, version as DES-BT01 BIOS V1.10
* 09/01/2010-945GS-8A79YAK8C-00 [**** DES-BT01 BIOS V1.10 (09/06/2010) ****]

**CPU:** Intel Atom N270

**GPU:** NVIDIA ION (GT218) series

**RAM:** 1 GB DDR2 (onboard)

**Chipset:** Intel 945GS

**Storage:** CompactFlash cards

**OS:** LFS Linux (kernel 2.6.32.8)

**Games:**
* Hero of Robots
* Demon Hunter
* Fish Lagoon
* Harpoon Lagoon (ICE)
* Shooting Mania
* 無敵風火輪
* 海遊漁 (Japan)

### E2200
**Motherboard:** Advantech DAC-BT07
Has two variants:
* KN-00 (DAC-BT07 A101-4) (Percussion Master 3)
* KN-01 (DAC-BT07 A102-2)

**BIOS:** Customized AMI BIOS 8, version as E2200 BIOS V1.0.0 (20111207)
* 64-0100-009999-00101111-120711-Pineview-E22_V100-Y2KC [E2200 BIOS V1.0.0 (20111207)]

**CPU:** Intel Atom D525 @ 1.83GHz

**GPU:** Nvidia GeForce (GT218-based, similar to Nvidia ION)

**Storage:** CompactFlash cards

**OS:** LFS Linux (kernel 2.6.32.8)

**Games:**
* Percussion Master 3 (2012)

### E3000
**Motherboard:** Pegatron E3000V (08M1-04E3000)

**BIOS:** AMI BIOS 8, more similar to regular ones. Other BIOS revisions may exist
* 64-0100-000001-00101111-032310-ATHLON64-E3K_X001-Y2KC [BIOS Date: 03/23/10 10:42:20 Ver: X10] [Vibraphone] [SR1.5]
* 64-0100-000001-00101111-022311-ATHLON64-E3K_X001-Y2KC [BIOS Date: 02/23/11 16:45:13 Ver: V11.0.0] [SR2] [SD4] [PT] [MuziBox]

**CPU:** AMD Athlon II X2 250

**GPU:** MSI GeForce 9800 GT (1 GB) (N9800GT-MD1G/PWM)

**RAM:** 2 x InnoDisk 1 GB DDR2-800 Low Profile DIMM

**Sound**: Realtek ALC888S (HD Audio)

**Storage:**
* SanDisk U100 SSD (16 GB) [Power Truck]
* InnoDisk iCF CompactFlash (8 GB) [Animal Kingdom: Fantasy Adventure]

**OS:** LFS Linux (kernel 2.6.32.8) / either Windows XPe or Embedded Standard 2009 [Music Gun Gun]

**Games:**
* Speed Driver 3: Crash Hour (2010)
* Speed Driver 4: World Fever (2012)
* Speed Rider (replacement PCB, also known as version 1.5) (2010)
* Speed Rider 2 (2011)
* Power Truck (2011)
* Power Truck Special (2014)
* Animal Kingdom: Fantasy Adventure (2013)
* Music Gun Gun (Taito, China version) (2010)
* MuziBox (音炫疯) (2012)
* Vibraphone (铁琴: 第一乐章) (2010) (newer board)

**PSU:** External.

### E3100
**Motherboard:** Advantech EBC-TA17, marked as iTS I-JOIN E3100  
Has two variants:
* LF-00 (Overtake?)
* LF-01 (Danz Base / Monster Eye)

**BIOS:** Customized PhoenixBIOS, each game has its own variation of BIOS.  
Currently found BIOS versions are: 
* E3100_BIOS_DB_V01.1.14-139 Date: Apr 8 2014 (Danz Base)
* E3100_MESEAT_V01.1.15-139.1 Date:Jun 4 2014 (Monster Eye)
* E3100_BIOS_OT_V01.1.14-139.1 Date: Apr 8 2014 (Overtake / Overtake DX)
An earlier BIOS revision from Sep 3 2013 exists for Danz Base.

**CPU:** Intel Core i3-3220 [Monster Eye] [Danz Base]
  Other variations may exist

**GPU:**
* NVIDIA GeForce GTX 750 (1 GB) [Monster Eye]
* Aetina GeForce GTX 650 / 740 (OEM) (N650C-H7FX) (1 GB, GDDR5) [Danz Base]
  Other variations may exist

**RAM:** 4 GB (2 x 2 GB) DDR3-1333 (dual-channel) [Monster Eye] [Danz Base]

**Sound:** C-Media CM6206, embedded on I-JOIN M3000 expansion board and can do 8-channel audio with another expansion board attached to the M3000 board.

**Storage:** ADLINK 32 GB Industrial SSD (IGS OEM, SSB032GTTC7-SBA-2), 2.5' SATA, mounted on I-JOIN M2000 expansion board. Normally encrypted, it's decrypted on the fly using the M2000 expansion board.

**Networking:** ASIX AX88772BLF Ethernet controller embedded on I-JOIN M3000 expansion board

**OS:** Windows Embedded Standard 2009 (32-bit)

**Extra:**
* I-JOIN M3000 (LI-05) expansion board: A strange board that takes 2 PCIe slots (one 16x, one 4x) at once, which handles sound and networking. Has an IGS036 chip embedded on the board, the functionality is yet to be determined. Has a slot for the additional 8-channel audio expansion board in the back.

* 8-channel audio expansion board: Attached to the M3000 expansion board, this provides 8-channel audio channel expandibility for the C-Media audio chip. This provides Center/Subwoofer (blue port), Side Speaker (black port) and Rear Speaker (pink port) ports. Also with a IDE-alike socket on it, the functionality is yet to be determined. Only known to be used in Monster Eye.
 
* I-JOIN M2000 expansion board: Probably some kind of security module, contains FPGA for decrypting the hard disk. SSD is mounted on this and then connects to the motherboard via proprietary 125-pin connector.

**Games:**
* Danz Base (2013)
* Monster Eye (2014)
* Overtake (2013)
* Overtake DX (2016)

**PSU:** External. Usually uses a Seasonic S12-II PSU

## S/V-series
### S3000/V3000
The S3000 has a wide casing with the power supply on the left side of the casing.
The V3000 is the same as S3000, except with an external power supply similar to the E3000 and E3100 and is less wider.
The V3000 has the same BIOS splash as the S3000, so to know if it's a S3000/V3000 requires access to the cabinet or looking at the manual.

**Motherboard:** GIGABYTE H110M-S2PV

**CPU:**
* Pentium G4400 [Transform: Hero of Robots, Ultra Race, Speed Rider 2]
* Core i3-7100 [Asphalt 9 Legends Arcade, Speed Driver 5, Monster Eye 2]
* Core i7-6700 [Overtake VR, Asphalt 9 Arcade VR]  
Other variations may exist

**GPU:**
* Aetina GeForce GTX 650 / 740 (OEM) (N650C-H7FX) (1 GB, GDDR5) [Transform: Hero of Robots] [SD4 (newer PCB)] [SR2 (newer PCB)] [UltraRace]
* Nvidia GeForce GTX 1050 (2 GB) [Transform: Hero of Robots (later versions)] [機甲英雄HOR] [SD5] [ME2]
* GIGABYTE GeForce GTX 1650 OC 4G [Asphalt 9 Legends Arcade]
* MSI GeForce GTX 1080 GAMING X 8G [Overtake VR]
* Nvidia GeForce RTX 2060 Super (as replacement GPU) [UMVR]
* ASUS DUAL RTX 3060 V2 OC (DUAL-RTX3060-O12G-V2) (12 GB) [A9VR]
* Intel HD Graphics [FotoZone]  
Other variations may exist

**RAM:**
* 1 x 4 GB DDR4 [Ultra Race]
* 2 x 4 GB DDR4-2400 (8 GB) [Monster Eye 2]
* 2 x 8 GB DDR4-2400 (16 GB) [Asphalt 9 Legends Arcade, Overtake VR, Speed Driver 5, Ultra Moto VR]
* 1 x 16 GB DDR4 + 1 x 8 GB DDR4 (24 GB) [Asphalt 9 Arcade VR]

**SSD:**
* 64 GB [Monster Eye 2] [Asphalt 9 Arcade VR]
* Transcend SSD370 32 GB SSD (TS32GSSD370) [Ultra Race]

**Sound:** Realtek ALC887 (HD Audio)

**BIOS:** customized GIGABYTE AMI BIOS, with a custom S3000 splash screen regardless of the S3000/V3000 board used.  

There are revisions of this BIOS:
* F4d
* F21j ZG

**OS:**
* Windows 10 IoT Embedded LTSB 2016 [Transform: Hero of Robots] [機甲英雄HOR] [Overtake VR]
* Windows Embedded Standard 7 (SP1) (x64) [Ultra Race]
* Windows 10 IoT Embedded LTSC 2021 [Sailor's Quest VR]
* LFS Linux [SD4] [SR2] [FotoZone]

**PSU:** Seasonic S12II-520B (520 W) [S3000]

**Games:**
```
    S3000   - Transform Hero of Robots (2017)
    S3000   - 機甲英雄Hero of Robots
    V3000   - Asphalt 9 Arcade DX (2021)
    V3000   - Asphalt 9 Arcade VR (2021)
    V3000   - FotoZone - Back to Jurassic (branded as S3000) (2017)
    V3000   - Monster Eye 2 (2018)
    V3000   - Overtake VR (2018)
    V3000   - Sailor's Quest VR (2022)
    V3000   - Speed Driver 5 (2019)
    V3000   - Ultra Moto VR (2019)
    V3000   - Ultra Race (2016)
            - Hyper Cross (2023)
            - Speed Rider 3 (2017)
            - Speed Rider 3DX (2019)
            - Speed Driver 4: World Fever (newer PCB) (2017)
            - Speed Rider 2 (newer PCB) (2016)
            
```

### S5000
**Motherboard:** customized GIGABYTE H610M-HD3P (rev 2.0)

**CPU:** Intel Pentium G7400

**GPU:**
* GIGABYTE GTX 1650 OC 4 GB [Moto Blitz DX]
* ZOTAC GAMING GeForce RTX 3050 Eco Solo 8 GB [ME3]

**RAM:**
* 2 x InnoDisk 16 GB DDR5 (M5UV-AGS2JC0P-BA83) [Moto Blitz DX]
* 1 x 16 GB DDR5-4800 [ME3]

**SSD:** 128 GB

**Security:** SafeNet KeyPro and M23 sub-board used in tandem for security

**Games:**
* Asphalt Moto Blitz DX
* Monster Eye 3 / Kaiju Rampage

## C-series
### C1000
**Motherboard:** IGS NX MB C1000

**CPU:** AMD Geode GX 533 (400MHz)

**Chipset:** AMD Geode CS5535

**GPU:** Geode GX2 Video Controller (16 MB shared memory)

**RAM:** 128 MB DDR-200 (4 x Hynix HY5DU561622ETP-5)

**Sound:**
* Realtek ALC203 (AC'97)
* C-Media CMI8738 [Percussion Kids/Tempo Kiddo]

**LAN:** Realtek RTL8100C

**OS:** modified Red Hat Linux (32-bit, using Linux kernel 2.4.24)

**BIOS:** modified National Semiconductors XpressROM BIOS.
* 12/06/06 [Percussion Kids / Tempo Kiddo]
Other BIOS revisions may exist

**Games:**
* Percussion Kids (2005)
* Tempo Kiddo (2005)
* IQ乐园PART4 (2007)
* 手指指2007 (2007)

**Notes:**
* Based on same board for earlier EZTouch games (IGS-Osprey) but with CPU module now onboard and IDE connector.
* The key to enter BIOS is still unknown.
* The MBR of the game's CompactFlash is encrypted by the BIOS, but the contents are still accessible using imaging tools.
* C-Media CMI8738 is used instead of the AC'97 chip for Percussion Kids and Tempo Kiddo, although the Realtek AC'97 chip is still present onboard.

**The BIOS has several checks:**
* The IGS027A ASIC is connected thru Texas Instruments PCI1510 bus chip. Before booting from the CompactFlash, it checks to see if the PCI1510 chip is present or not. If it can find the chip, it will say "Find IGS Card.". Else, it will refuse to boot and output "Not Find IGS Card."
* The encrypted MBR has the header of "IGS-I-JOIN-C1000" and the BIOS has elements of GRUB strings to do check against. It's not possible to boot from other boot drives like USB without the header and GRUB strings present; it will fail with "Boot False(B)."

### C2000
**Motherboard:** I-JOIN C2000
Has two variants:
* Rev2.0: onboard DDR1 RAM with additional DIMM slot
* Rev2.1: same as Rev2.0, but without the onboard RAM and minor layout changes

**CPU:** AMD Geode series

**STH:** AMD Geode CS5536 (?)

**RAM:**
* onboard DDR1 RAM (size unknown) + 1 x DDR1 DIMM slot [Rev2.0]
* 1 x DDR1 DIMM slot [Rev2.1]

**Sound:** Realtek ALC650 (AC'97)

**LAN:** Realtek RTL8100CL

**BIOS:** customized Phoenix-AwardBIOS v6.00PG.
* 11/30/2007-AMD-GX3-6A43A00BC-00 [X11] [Rev2.0]
* 10/13/2009-AMD-GX3-6A43A00BC-00 [X13A] [Rev2.1]
Other BIOS revisions may exist, such as X13 (non-A)

**Games:**
```
    Rev2.0      - Jungle Drummer (丛林鼓王)
    Rev2.1      - IQ Park Online (IQ乐园网络版)
    Rev2.1      - IQ Park 2008 (IQ乐园2008)
    Rev2.1      - IQ Park 2011 (IQ乐园2011)
    Rev2.1      - IQ Park 2012 (IQ乐园2012)
                - Global Touch 2007 Sigma
                - Diamond Progressive (control box)

```

**Notes:**
* BIOS can be accessed via Ctrl+D while at the IGS BIOS splash screen at boot-up
* Onboard video memory size can be adjusted up to 256 MB
* Similar to its predecessor, it also has a check for the Texas Instruments Ti1510 chip embedded inside the board after the POST screen. It will fail with "Ti1510 is not Exist" error if it doesn't find one on the board.

## Misc
### Percussion Master (export)
**Motherboard:** ECS L4S5MG/651+ (V5.0A)

**Chipset:** SiS 651 (Northbridge) / SiS 692 (Southbridge)

**CPU:** Intel Celeron (?) (Socket 478)

**GPU:** Nvidia GeForce4 MX440 (64MB)

**RAM:** 512 MB DDR-333 

**OS:** Red Hat Linux (32-bit)

**Note:** Some cabs of Percussion Master 1 uses this PCB.

### Rock Fever 4 Remix
**Motherboard:** Foxconn 661FX7MI-S (?)

**CPU:** Intel Celeron D (?) (LGA 775)

**GPU:** Nvidia GeForce4 MX4000

**OS:** Linux, likely LFS

### Speed Driver Evolution / Top Driver Evolution
**Motherboard:** ECS 661GX-M7 (v1.1) / ECS 661FX-M7 (v1.1)

**CPU:** Intel Celeron D 335/336 (2.8GHz) (LGA 775)

**GPU:** GeForce 6200A (128 MB, AGP)

**RAM:** 512 MB DDR

**OS:** modified Fedora Linux (kernel 2.4.22)