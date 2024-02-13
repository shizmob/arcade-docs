# Andamiro boards

## MK1

The oldest piece of hardware we have seen in the wild was a MK3 board so far. But there are several hints that
some piece of hardware pre-dating the MK3 existed at some point:

* The first three Pump It Up games, [1st](game/piu/1st.md), [2nd](game/piu/2nd.md) and [3rd/OBG](game/piu/3rd.md),\
  are storing their music as actual CD audio, not MP3 files in the data area of the discs
* MP3 hardware decoder chips were likely not cheap/easily available at that time. Furthermore, the total audio length
  of all songs still fit onto the disc as CD audio tracks
* The first three Pump It Up games did not use a lock-chip as a means for copy-protection. Possible,
  that this piece of hardware wasn't available from the beginning and therefore not used

### MK1 compatible games

* [Pump it Up: The 1st Dance Floor](game/piu/1st.md)
* [Pump it Up: The 2nd Dance Floor](game/piu/2nd.md)
* [Pump it Up The O.B.G: The 3rd Dance Floor](game/piu/3rd.md)

## MK3

* Custom PCB assembly with daughter boards stacked
* DOS OS stored on ROM chip
* Games stored and loaded from CD
* [PIUIO](io.md#mk3io) interface connected via ISA Bus
* Hardware audio decoder chip for MP3 audio
* CAT702 ZN security "Lock chip" for copy-protection
* EEPROM to store game settings

### System Configuration using DOS PC-Doctor

System configuration dump with DOS PC-Doctor. The HDD listed in the information below is part of the
system that was used to dump this information. The DVD drive is a replacement of a likely broken
CD drive.

```text
SYSTEM CONFIGURATION=====================================================

     Operating System - DOS 7.10 in HMA
             CPU Type - 333 MHz Intel Celeron 333
                CPUID - "GenuineIntel", Family 6, Model 6, Step 5
                      - MMX available
     Coprocessor Type - 686
   Expansion Bus Type - ISA, PCI
        ROM BIOS Date - 04/20/99 
   ROM BIOS Copyright - COPYRIGHT Award Software Inc.
       Additional ROM - C800[8kB] 
          Base Memory - 640 kB
      Expanded Memory - N/A
      Extended Memory - 64512 kB (CMOS Configuration)
           XMS Memory - 62400 kB (XMS 3.00, Driver 3.95) A20=ON 
         Serial Ports - None Installed
       Parallel Ports - None Installed
        Video Adapter - VGA: 3Dfx Interactive, Inc.
                      - Total Memory : 8192 kB
    Fixed Disk Drives - 42 MB  
   Floppy Disk Drives - 1 - 1=3.5"/1.44M  
                Mouse - No Mouse
            Joysticks - None
           Sound Card - N/A
   CAS Fax/Modem Card - N/A
     Disk Compression - N/A
CD-ROM Driver Version - MSCDEX V2.25, Drive: D:
           Disk Cache - Smartdrive 5.02, Hits 76%, Size 2048 kB
   Primary IDE Master - ATAPI: HL-DT-STDVD-ROM GDR8164B
    Primary IDE Slave - IDE: QUANTUM FIREBALL_TM1280A, S/N:692708422782
 Secondary IDE Master - No Drive
  Secondary IDE Slave - No Drive
                 SCSI - N/A
              Network - N/A
     Power Management - APM V1.2, Power On
             USB Port - Installed on IRQ 10
         Chipset Type - Intel 440BX
        L2 Cache Type - 128 kB
           DRAM Row 0 - 64 MB
           DRAM Row 1 - Empty
           DRAM Row 2 - Empty
           DRAM Row 3 - Empty
           DRAM Row 4 - Empty
           DRAM Row 5 - Empty
           DRAM Row 6 - Empty
           DRAM Row 7 - Empty


PC-DOCTOR DOS 3.0 Copyr 2004 PC-Doctor, Inc. 16:15 9/25/2000
```

### On-board chips

* Audio related
  * MAS 3507D MPEG 1/2 Layer 2/3 Audio Decoder
  * DAC 3550A Stereo Audio DAC
  * YMZ280B PCMD8 8-Channel PCM/ADPCM Decoder
  * YAC516 DAC16-L Delta Sigma Modulation D/A Converter with 8 times Over-sampling Filter
* Security
  * [CAT702 ZN security](https://github.com/svn2github/mameplus/blob/master/trunk/mamep/src/mame/machine/cat702.c)

### MK3 compatible games

* [Pump it Up: The 1st Dance Floor](game/piu/1st.md)
* [Pump it Up: The 2nd Dance Floor](game/piu/2nd.md)
* [Pump it Up The O.B.G: The 3rd Dance Floor](game/piu/3rd.md)
* [Pump it Up The O.B.G: The Season Evolution Dance Floor](game/piu/3se.md)
* [Pump it Up: The Collection](game/piu/tc.md)
* [Pump it Up: The Perfect Collection](game/piu/pc.md)
* [Pump it Up Extra](game/piu/extra.md)
* [Pump it Up The Premiere: The International Dance Floor](game/piu/prem1.md)
* [Pump it Up The PREX: The International Dance Floor](game/piu/prex1.md)
* [Pump it Up The Rebirth: The 8th Dance Floor](game/piu/reb.md)
* [Pump it Up The Premiere 2: The International 2nd Dance Floor](game/piu/prem2.md)
* [Pump it Up The PREX 2](game/piu/prex2.md)
* [Pump it Up The Premiere 3: The International 3rd Dance Floor](game/piu/prem3.md)
* [Pump it Up The PREX 3: The International 4th Dance Floor](game/piu/prex3.md)

## MK5

* OS
  * Windows XP Embedded: revisions of [The Premiere 3](game/piu/prem3.md) and [The PREX 3](game/piu/prex3.md)
  * Linux: starting [Exceed](game/piu/exc.md)
* [PIUIO](io.md#MK5IO) connected to the ISA bus
* CPU: Intel Celeron 1 GHZ
* RAM: 128 MB
* GPU: on-board Riva TNT 2, 32 MB
* Chipset: Nvidia NV11
* Disk media
  * CDROM based for [The Premiere 3](game/piu/prem3.md) and [The PREX 3](game/piu/prex3.md)
  * DVD based for [Exceed](game/piu/exc.md) beta
  * HDD based for [Exceed](game/piu/exc.md) release and newer
* EEPROM to store game settings and high scores. Size increased (doubled?) comapred to [MK3](#mk-3)

### MK5 compatible games

* [Pump it Up The Premiere 3: The International 3rd Dance Floor](game/piu/prem3.md)
* [Pump it Up The PREX 3: The International 4th Dance Floor](game/piu/prex3.md)
* [Pump it Up Exceed: The International 5th Dance Floor](game/piu/exc.md)
* [Pump it Up Exceed 2: The International 6th Dance Floor](game/piu/exc2.md)
* [Pump it Up NX: New Xenesis](game/piu/nx.md)

## MK6

### Base specs

* Introduces [USBPIUIO](io.md#usbpiuio) interface for cabinet and pad inputs/outputs
* GPU: NVIDIA GeForce 5200 FX, 128 MB, AGP
* RAM: 256 MB, e.g. PC3100 Samsung
* Storage media: 2.5" HDDs of several manufacturers

### MK6 Rev1

* Started shipping with [Exceed 2](game/piu/exc2.md)
* Motherboard
  * Gigabyte GA-8IPE1000MK (rev. 1.x), Socket 478
  * Gigabyte GA-8IG1000MK Rev 2.X, LGA775
* CPU
  * For socket 478: Intel Celeron D, 2.53 GHZ/256/533
* Sound chip still compatible with [Exceed 2](game/piu/exc2.md) and [Zero](game/piu/zero.md)

### MK6 Rev2

* Started shipping later during the lifecycle of [NX](game/piu/nx.md)
  * (Some/most?) [FX](cabinet.md#fx) cabs with [NX](game/piu/nx.md) still came with Revision 1
* Motherboard: GA-8I865GME-775-RH Rev 1.X, LGA775
* Sometimes referred to as "MK 7"
* Sound chip **NOT** compatible with [Exceed 2](game/piu/exc2.md) and [Zero](game/piu/zero.md)

### Compatible games

* [Pump it Up Exceed 2: The International 6th Dance Floor](game/piu/exc2.md) (only Revision 1)
* [Pump it Up NX: New Xenesis](game/piu/nx.md) (only Revision 1)
* [Pump it Up NX2: Next Xenesis](game/piu/nx2.md)
* [Pump It Up PRO](game/piu/pro.md)
* [Pump It Up NX Absolute: International 10th Dance Floor](game/piu/nxa.md)
* [Pump It Up PRO 2](game/piu/pro2.md) (no 3D arrow skin)
* [Pump It Up 2010 Fiesta](game/piu/fst.md) (requires RAM upgrade to at least 512 MB)
* [Pump It Up 2011 Fiesta EX](game/piu/fex.md) (requires RAM upgrade to at least 512 MB)
* [Pump It Up 2013 Fiesta 2](game/piu/f2.md) (requires RAM upgrade to at least 512 MB)
* [Pump It Up 2015 Prime](game/piu/prime.md) (requires RAM upgrade to at least 512 MB, SD mode only)
* [Pump It Up 2017 Prime 2](game/piu/prime2.md) (supposed to run somewhat with Revision 2 but not 1)

## Main PCBs for Pump it Up after MK6

These are usually referred to as "MK9" or "MK10/MKX" depending on when released. However, these were never referred to
as specific MK versions nor revisions by Andamiro. Compatbility with different software versions might vary.

### 945

* Motherboard: Gigabyte GA-945GCM-S2L
* CPU: Intel Celeron "L420" 1.6Ghz
* GPU: GeForce 7200GS Low Profile or Geforce 8400GS 256M Low Profile
* RAM: 1GB DDR2 800Mhz
* IO: [USBPIUIO](io.md#usbpioio)
* Bundled with [NX2](game/piu/nx2.md) 1.54 and higher
* Anything before [NX2](game/piu/nx2.md) 1.54 doesn't work with this revision
* Shipped with upgrades and when buying a [FX cabinet](cabinet.md#fx) at that time

### G31

* Motherboard: Gigabyte G31M
* CPU: Intel Celeron "L430" 1.8Ghz
* GPU: Nvidia GeForce 8400GS 256MB Low Profile
* RAM: 512MB DDR2 800Mhz
* IO: [USBPIUIO](io.md#usbpioio)
* Bundled with Fiesta when buying a [TX cabinet](cabinet.md#tx) at that time
* GPU last compatible card with [Fiesta](game/piu/fst.md)/[FiestaEX](game/piu/fstex.md)

### G41

#### Asrock G41

* Motherboard: Asrock G41M-S3
* GPU: Nvidia GeForce GT210 or Geforce 9300GS
* CPU: Intel Celeron "L430" 1.8Ghz
* RAM: 1 GB
* IO: [USBPIUIO](io.md#usbpioio)
* Hardware shipped with [Pump it Up Jump cabinets](cabinet.md#jump)

#### Gigabyte G41

* Motherboard: Gigabyte G41M
* CPU: Intel Celeron "L430" 1.8Ghz
* RAM: 1 GB
* GPU: Nvidia GeForce GT210 or Geforce 9300GS
* IO: [USBPIUIO](io.md#usbpioio)
* Bundled with [Fiesta 2](game/piu/f2.md) when buying a [CX cabinet](cabinet.md#cx) at that time
* GPU last compatible card with Fiesta 2 OS

### H81

* Official name: `MCU: MK-8171`
* Motherboard: Asrock H81M-DGS REV2.01
* CPU: Intel Celeron G1840/2.8GHz
* GPU: Nvidia GeForce GT710 1GB 64bit GDDR3
* IO: [LXIO](io.md#lxio) and [USBPIUIO](io.md#usbpiuio) with breakout cables for LXIO "hanging out"
* RAM: 2 GB
* Bundled with Pump It Up [XX](game/piu/xx.md) upgrade kit

### H310

### H610

* Official name: `MCU: MK-6171`
* Motherboard: GIGABYTE H610M-K DDR4
* CPU: Intel Celeron G6900
* GPU: Nvidia GeForce GT710 1GB 64bit GDDR3
* IO: [LXIO](io.md#lxio) and [USBPIUIO](io.md#usbpiuio) with breakout cables for LXIO "hanging out"
* RAM: 8 GB DDR4-3200
* Bundled with Pump It Up [Phoenix](game/piu/phoenix.md) upgrade kit