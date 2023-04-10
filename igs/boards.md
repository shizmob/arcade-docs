
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

**OS:** Linux, likely LFS

**Games:**
* Percussion Master
* Percussion Master Plus
* Percussion Master 2
* Rock Fever 5

### E2000
**Motherboard:** I-JOIN E2000

There are two variants:
* E2000-C6-V256: Has Celeron M 600MHz onboard
* E2000-V256: Has a PGA479 socket with Celeron M 370 attached.
Has two sub-variants, differences unknown but similar:
** IGS MB NX E2000C [SD2]
** IGS MB NX E2000D [WeDo]

**CPU:**
* Intel Celeron M (600MHz, SL8FN) (onboard) [E2000-C6-V256]
* Intel Celeron M 370 (1.5GHz, SL8MM) (socketed) [E2000-V256]

**GPU:** Nvidia GeForce 6200 (256 MB GDDR2) [GF-6200-AGP N-A1]

**RAM:** 2 x DDR1 slot. Memory sizes differ depending on games
* DSL 1 GB DDR-333 [WeDo]

**Chipset:** Intel 852GME

**Storage:**
* CompactFlash card
* IDE-based hard drives are also possible thru IDE connector

**SND:** Realtek ALC655 (AC'97)

**OS:** LFS Linux (kernel 2.4.31)

**BIOS:** customized Phoenix AwardBIOS. Other BIOS revisions may exist
* 07/03/2007-i852-W83627HF-6A69YILTC-00 [E2000C] [E2000D]

**Games:**
```
    E2000-C6-V256   - Panda Family
    E2000-C6-V256   - Rock Fever 5 (replacement/newer PCB)
    E2000-C6-V256   - Percussion Master Plus (replacement/newer PCB)
    E2000-C6-V256   - Percussion Master 2008 (replacement/newer PCB)
    E2000-C6-V256   - Gold Captain (航海小勇士)
    E2000-V256      - Pirate Revenge
    E2000-V256      - We Dancing Online
    E2000-V256      - We Dancing Online 2 (Plus)
    E2000-V256      - Speed Rider
    E2000-V256      - Speed Driver 2: Overtake
                    - Vibraphone (铁琴: 第一乐章)
                    - Submarine Crisis
```

**Notes:**
* BIOS can be accessed via Ctrl+D at boot-up

### E2100
**Motherboard:** Advantech DES-BT01

**BIOS:** Customized Phoenix-AwardBIOS v6.00PG, version as DES-BT01 BIOS V1.10
* 09/01/2010-945GS-8A79YAK8C-00 [**** DES-BT01 BIOS V1.10 (09/06/2010) ****]

**CPU:** Intel Atom N270

**GPU:** NVIDIA ION (GT218) series

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
* Percussion Master 3

### E3000
**Motherboard:** Pegatron E3000V (08M1-04E3000)

**BIOS:** AMI BIOS 8, more similar to regular ones. Other BIOS revisions may exist
* 64-0100-000001-00101111-022311-ATHLON64-E3K_X001-Y2KC [BIOS Date: 02/23/11 16:45:13 Ver: V11.0.0] [SR2] [SD4] [PT] [MuziBox]

**CPU:** AMD Athlon II X2 250

**GPU:** MSI GeForce 9800 GT (1 GB) (N9800GT-MD1G/PWM)

**RAM:** 2 x InnoDisk 1 GB DDR2-800 Low Profile DIMM

**Sound**: Realtek ALC888S (HD Audio)

**Storage:** SanDisk U100 SSD (16 GB)

**OS:** LFS Linux (kernel 2.6.32.8) / either Windows XPe or Embedded Standard 2009 [Music Gun Gun]

**Games:**
* Speed Driver 3
* Speed Driver 4
* Speed Rider (replacement PCB)
* Speed Rider 2
* Power Truck
* Power Truck Special
* Music Gun Gun (Taito, China version)
* MuziBox (音炫疯)

### E3100
**Motherboard:** Advantech EBC-TA17, marked as iTS I-JOIN E3100  
Has two variants:
* LF-00 (Overtake?)
* LF-01 (Danz Base / Monster Eye)

**BIOS:** Customized PhoenixBIOS, each game has its own variation of BIOS.  
Currently found BIOS versions are: 
* E3100_BIOS_DB_V01.1.14-139 Date: Apr 8 2014 (Danz Base)
* E3100_MESEAT_V01.1.15-139.1 Date:Jun 4 2014 (Monster Eye)
* E3100_BIOS_OT_V01.1.14-139.1 Date: Apr 8 2014 (Overtake / Overtake DX / UltraRace)

**CPU:** Intel Core i3-3220

**GPU:** NVIDIA GeForce GTX 750 (1 GB)

**RAM:** 4 GB DDR3

**Sound:** C-Media CM6206, embedded on I-JOIN M3000 expansion board

**Storage:** ADLINK 32 GB Industrial SSD (IGS OEM, SSB032GTTC7-SBA-2), 2.5' SATA, mounted on I-JOIN M2000 expansion board then connects to the motherboard via proprietary 125 PIN connector

**Networking:** ASIX AX88772BLF Ethernet controller embedded on I-JOIN M3000 expansion board

**OS:** Windows Embedded Standard 2009 (32-bit)

**Extra:**
 I-JOIN M3000 (LI-05) expansion board: A strange board that takes 2 PCIe slots (one 16x, one 4x) at once, which handles sound and networking. Also with a IDE-alike socket on it, the functionality is yet to be determined.
 
 I-JOIN M2000 expansion board: Probably some kind of security module, contains FPGA for decrypting the hard disk. SSD is mounted on this and then connects to the motherboard via proprietary 125-pin connector.

**Games:**
* Danz Base
* Monster Eye
* Monster Eye 2 (?)
* Overtake
* Overtake DX
* Ultra Race (?)

## S/V-series
### S3000
**Motherboard:** GIGABYTE H110M-S2PV

**GPU:** Nvidia GeForce GTX 1050 (2 GB) [Transform: Hero of Robots], other variations may exist

**OS:** Windows 10 IoT Embedded LTSB 2016 / LFS Linux (only found in Speed Driver 4 replacement PCBs)

**Games:**
* Speed Driver 4 (replacement PCB)
* Transform Hero of Robots
* Speed Rider 3

### V3000
**Motherboard:** GIGABYTE H110M-S2PV

**CPU:** Core i3-7100 [Asphalt 9 Legends Arcade]

**GPU:** 
* Nvidia GeForce RTX 2060 Super (as replacement GPU) [Ultra Moto VR]
* GIGABYTE GeForce GTX 1650 OC 4G [Asphalt 9 Legends Arcade]
Other variations may exist

**RAM:** 2 x 8 GB DDR4-2400 (16 GB) [Asphalt 9 Legends Arcade]

**Sound:** Realtek ALC887 (HD Audio)

**OS:** Windows 10 IoT Embedded LTSB 2016 (?)

**Games:**
* Speed Driver 5
* Overtake VR (?)
* Ultra Moto VR
* Asphalt 9 Arcade DX

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

**BIOS:** modified National Semiconductors XpressROM BIOS [Percussion Kids, newer revision PCB]

**Games:**
* Percussion Kids (2005)
* Tempo Kiddo (2005)
* IQ乐园PART4 (2007)
* 手指指2007 (2007)

**Notes:**
* Based on same board for earlier EZTouch games (IGS-Osprey) but with CPU module now onboard and IDE connector.
* The key to enter BIOS is still unknown.
* The IGS027A ASIC is connected thru Texas Instruments PCI1510 bus chip.
* The MBR of the game's CompactFlash is encrypted by the BIOS, but the contents are still accessible using imaging tools.
* The encrypted MBR has the header of "IGS-I-JOIN-C1000". It's not possible to boot from other boot drives like USB without the header present; it will fail with "Boot False(B)."
* C-Media CMI8738 is used instead of the AC'97 chip for Percussion Kids and Tempo Kiddo, although the Realtek AC'97 chip is still present onboard.

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

**BIOS:** customized Phoenix AwardBIOS

**Games:**
```
    Rev2.0      - Jungle Drummer (丛林鼓王)
    Rev2.1      - IQ Park Online (IQ乐园网络版)
    Rev2.1      - IQ Park 2008 (IQ乐园2008)
    Rev2.1      - IQ Park 2011 (IQ乐园2011)
    Rev2.1      - IQ Park 2011 (IQ乐园2012)
                - Global Touch 2007 Sigma
                - Diamond Progressive (control box)

```

**Notes:**
* BIOS can be accessed via Ctrl+D while at the IGS BIOS splash screen at boot-up
* Onboard video memory size can be adjusted up to 256 MB

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