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
Despite using Intel processors, PGM3 is not a PC/AT compatible system.

**CPU:** Intel Atom D525 @ 1.80GHz ? / SOCLE SOC38, customized ARM1176 @ 800MHz?

**RAM:** 2GB

**Graphics:** ? 800x600 / 1280x720

**Storage:** ROM cartridges (game); IC cards (player savedata)

**Extra:** IC card readers
## MA1000
(There is little to no information about this board yet.)

# PC-Based
## E2000
**Motherboard:** I-JOIN E2000-C6-V256

**Storage:** CompactFlash cards

**OS:** Linux, likely LFS

## E2100
**Motherboard:** Advantech DES-BT01

**BIOS:** Customized Phoenix-AwardBIOS v6.00PG, version as DES-BT01 BIOS V1.10

**CPU:** Intel Atom N270

**Storage:** CompactFlash cards

**OS:** Linux, likely LFS

## E2200
**Motherboard:** Advantech DAC-BT07

**BIOS:** Customized AMI BIOS 8, version as E2200 BIOS V1.0.0 (20111207)

**CPU:** Intel Atom D525 @ 1.83GHz

**Storage:** CompactFlash cards

**OS:** Linux, likely LFS

## E3000
**Motherboard:** Model number IGS LX MB E3000V, unknown manufacture

**BIOS:** AMI BIOS 8, more similar to regular ones

**CPU:** AMD Athlon II X2 250

**GPU:** MSI GeForce 9800 GT (1 GB)

**RAM:** 2 x InnoDisk 1 GB DDR2-800 Low Profile DIMM

**Sound**: Realtek ALC888S (HD Audio)

**Storage:** SSD ?

**OS:** Linux, likely LFS


## E3100
**Motherboard:** Advantech EBC-TA17, marked as iTS I-JOIN E3100

**BIOS:** Customized PhoenixBIOS, each game has its own variation of BIOS.
Currently found BIOS versions are: 
* E3100_BIOS_DB_V01.1.14-139 (Danz Base)
* E3100_MESEAT_V01.1.15-139.1 (Monser Eye)
* E3100_BIOS_OT_V01.1.14-139.1 (Overtake/Overtake DX/UltraRace)

**GPU:** NVIDIA GeForce GTX 750 (1 GB)

**RAM:** 4 GB DDR3

**Sound:** C-Media CM6206, embedded on I-JOIN M3000 expansion board

**Storage:** ADLINK 32 GB Industrial SSD, 2.5' SATA, mounted on I-JOIN M2000 expansion board then connects to the motherboard via proprietary 125 PIN connector

**Networking:** ASIX AX88772BLF Ethernet controller embedded on I-JOIN M3000 expansion board

**OS:** Windows Embedded Standard 2009 (32-bit)

**Extra:**
 I-JOIN M3000 expansion board: A strange board that takes 2 PCIe slots (one 16x, on 4x) at once, which handles sound and networking. Also with a IDE-alike socket on it, the functionality is yet to be determined.
 
 I-JOIN M2000 expansion board: Probably some kind of security module, contains FPGA for decrypting the hard disk. Hard disk is mounted on this and then connects to the motherboard via proprietary 125 PIN connector.

## S3000
**Motherboard:** GIGABYTE H110M-S2PV ?

**GPU:** Nvidia GeForce GTX 1050 (2 GB), other variations may exist

**OS:** Windows 10 IoT Embedded LTSB 2016 / LFS Linux (only found in SpeedDriver 4 replacement PCBs)

## V3000

