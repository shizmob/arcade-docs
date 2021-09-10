# SEGA boards

SEGA parts are referred to using a [proprietary format](identifiers.md#part-number).

## UFO catcher

```
  * 834-8051-01:    NEW UFO CATCHER(SONIC) EPR-14124 https://page.auctions.yahoo.co.jp/jp/auction/x782565940
  * 834-8421:       UFO Catcher Mini EPR-14355 https://page.auctions.yahoo.co.jp/jp/auction/r479052623
  * 834-12630:      GAME BD ??? (UFO Catcher 21) EPR-19063A/EPR-19064 https://page.auctions.yahoo.co.jp/jp/auction/p870216230
  * 834-13344:      GAME BD ??? (UFO Catcher 800) EPR-20413A
  * 834-14426:      GAME BD UCM (UFO Catcher 7 MAX) EPR-24139 https://page.auctions.yahoo.co.jp/jp/auction/p866025564
  * 834-14606:      GAME BD UCU (Sega UFO Catcher)
  * 837-10493-03/834-12710:   UFO Catcher 800            https://page.auctions.yahoo.co.jp/jp/auction/r441207101
  * 837-10493-04:   UFO Catcher 21             https://page.auctions.yahoo.co.jp/jp/auction/p870216230
```

## NAOMI

```
   Y = D: hardware kit
   840-xxxxD:     NAOMI + cartridge kit (see cartridges section)
   840-0051D:     NAOMI + 840-0001F + GD-rom drive kit  ("ASSY CASE NAO PCI DIMM BD")
   840-0071D-01:  NAOMI2 + 840-0001F + GD-rom drive kit ("ASSY CASE NAT PCI DIMM BD")
   840-0080D-01?: 840-0001F + GD-rom drive kit?         ("ASSY CASE PC1 DIMM BD")
   840-0089D:     NAOMI + 840-0004F + GD-rom drive kit  ("ASSY CASE NAO RTOS DIMM BD")
   840-0091D-1x:  "ASSY CASE NAT RT/232C &COM"
   840-0106D-01:  "ASSY CASE TRF 512 DIMM BD"

   Y = A: hardware
   840-0001A: NAOMI ("ASSY CASE NAOMI MAIN BD")
   840-0002A: (840-0150C)
            -1x: "ASSY CASE NAO CRX MAIN SER"
   840-0003A: (840-0003C) "SHIELD CASE ZBX NAO"
   840-0004A: NAOMI with serial ("ASSY CASE NAO MAIN SER R")
   840-0021A: (840-0021C) "SHIELD CASE NBA NAO"
   840-0046A: NAOMI2 ("ASSY CASE NAOMI 2 MAIN BD")
            -1x: "ASSY CASE NAT MAIN W/232C"

   Y = E: communication board?
   840-0001E: Cartridge underside board ("ASSY CASE NAO COMMUNICATION BD")

   Y = F: DIMM board
   840-0001F: DIMM 256MB, SCSI ("ASSY CASE NAO DIMM BD COM")
   840-0004F: DIMM 256MB, SERIAL, SCSI, ETHERNET ("DIMM BD NAO" / "ASSY CASE NAO DIMM BD COM RTOS")
   840-0005F: DIMM 256MB, ETHERNET
   840-0006F: DIMM 512MB, SERIAL, SCSI, ETHERNET ("DIMM BD NAT")
   840-0008F: DIMM 512MB, ETHERNET
```

## System SP

```
  * 834-14493 /          : GAME BD SP DKG      : Dinosaur King : US
  * 834-14661 /          : GAME BD SP 512 OSM  : Love and Berry : US
  * 834-14662 /          :                     :
  * 834-14713 /          : GAME BD SP MRW SATL : Mirage World [satl] : JP
  * 834-14788 /          :                     : Bingo Galaxy [main] : JP
  * 834-14789 /          :                     : Bingo Galaxy [satl] : JP
  * 834-14792 /          :                     : Dinosaur King 2 : EXP
  * 834-14865 /          :                     :
  * 834-14970 /          : GAME BD SP DKC      : Tetris Giant / Dekai Tetris : GL
  * 834-14750 /          :                     : Ami-no-San : JP : https://webcache.googleusercontent.com/search?q=cache:VCAbfytrwvYJ:https://aucfree.com/items/d359606190+&cd=14&hl=nl&ct=clnk&gl=nl
  * 834-15041 /          :                     : Ami-no-San : JP
  *           / 837-14434:                     : Dinosaur King - Operating: Dinosaur Rescue : US
  *           / 837-14481:                     : Bingo Galaxy [satl] : JP : EPR-24236 https://page.auctions.yahoo.co.jp/jp/auction/w464167213
  *           / 837-14699:                     :
  *           / 837-14700:                     :
  *           / 837-14790:                     : Ocha-Ken Hot Medal : JP
  *           / 837-14875:                     : Puyo Puyo : JP : EPR-24328 https://page.auctions.yahoo.co.jp/jp/auction/p844401477
  *           / 837-14881:                     : Brick People : GL
```

## Triforce

```
  C = D (board + game kit)
     * 842-0001D:    Triforce Type1 kit
     * 842-xxDDyyyr: Triforce Type3 DIMM kit ("ASSY TRF", xx = linear to GDT-xxxx game ID, yyy = ???)
     * 842-xxDNyyyr: Triforce Type3 NAND kit (xx = linear to GDT-xxxx game ID, yyy = ???)
         -01: silver housing
  C = A (board):
     * 842-0001A:    Triforce Type1 board
     * 842-00A0000r: Triforce Type3 board
  C = F (DIMM):
     * 842-00FD0000: Triforce Type3 DIMM board ("TRF DIMM MEDIA BD")
```

## Chihiro

```
  C = D (board + game kit):
     * 843-xxxxD, xxxx = linear to GDX-xxxx game ID: "ASSY CASE BOX" [known revisions: 0, 1, 2, 3]
         -0x: "ASSY CASE BOX"
         -1x: "ASSY CASE BOX COM NAO"
         -2x: "ASSY CASE BOX COM DIMM"
         -3x: "ASSY CASE BOX COM DIMM LAN"
  C = A (board):
     * 843-0001A: main board [known revisions: 0, 1]
         -0x: "ASSY CASE BOX MAIN BD"
         -1x: "ASSY CASE BOX MAIN BD X-B"
  C = B (game DIMM):
     * 843-xxxxB, xxxx = linear to GDX-xxxx game ID: "ASSY CASE BOX DIMM BD"
```

## Lindbergh

```
  * Lindbergh                       (AAGE, 844-00xxD, "ASSY CASE LBG L 1GB *", known revisions: 0, 1)
        Case: yellow, Lindbergh logo top left
        MBD:  ???
        CPU:  Pentium 4 3.0GHz HT
        RAM:  2x 512MB PC3200
        GPU:  Nvidia GeForce 6800GT [256MB, PCI: 10DE:0045] (revision 0)
              Nvidia Geforce 7800GS [256MB, PCI: 10DE:00F5/10DE:00F0] (revision 1, 844-0001D(-xx)-1x, "ASSY CASE LBG L 1GB 7800")
        CF:   MDA-C0004A
        IDE1: 40GB HDS728040PLAT20
        OS:   MontaVista Linux
        IO:   JVS card [PCI: 0CA3:18F7/1058:18C1], audio card

  * Lindbergh Star Horse [Yellow]   (AAGE, 844-10xxD, "ASSY CASE LBG SHT *", known revisions: 0, 1) [-00: server, -01: video, -02: sound, -03: satellite]
        Case: yellow, no logo
        MBD:  838-14526-91-02?
        CPU:  Pentium 4 3.0GHz HT
        RAM:  4x 512MB PC3200
        GPU:  Nvidia GeForce 6800GT? [256MB, PCI: 10DE:0045]] (revision 0)
              Nvidia Geforce 7800GS [256MB, PCI: 10DE:00F5/10DE:00F0] (revision 1, 844-10xxD-1x, "ASSY CASE LBG SHT * 7800")
        CF:   MDA-C0005A [601-11548-128A]
        IDE1: 839-14484R "CF-IDE TRANSLATION BD":    MDA-C0007A (satellite/live?)
              839-1370 "IDE 2.5-3.5 TRANSLATION BD": Transcend TS8GSS25-S [2.5" IDE SSD 8GB] (server)
        IDE2: 2x 512MB Hagiwara SYS-COM IDT-512MSH [3.5" IDE SSD 512MB, produced by Toshiba: THNID512MSAIH10AAB] (server)
        OS:   MontaVista Linux
        IO:   parallel card 837-14443-01 (server/video?/satellite)
        IO:   audio card (sound)

  * Lindbergh Blue                  (AAJE, 844-30xxD, "ASSY CASE LBG W *")
        Case: blue, Lindbergh B logo top left
        MBD:  ???
        CPU:  Pentium 4 3.0GHz HT
        RAM:  2x 512MB PC3200
        GPU:  ???
        CF:   MDA-C0031
        IDE1: ??? 40GB
        OS:   Windows XP Embedded
        IO:   JVS card, audio card

  * Lindbergh Terminal             (AAGE, 844-50xxD, "TOP ASSY LBG *") [-10: server, -20: satellite, -30: live, -40: terminal?]
        Case: silver, game & role top left, Lindbergh + SEGA + all.net P-RAS logo top center, "所有" top right, serial top far right)
        MBD:  Advantech POD-SG01? (838-14813 / 837-14849 / 979MSG01??E / POD-SG01-03A1E)
        CPU:  ???
        RAM:  ???
        GPU:  ???
        CF:   ???
        IDE1: ???
        OS:   MontaVista Linux
        IO:   JVS card [PCI: 0CA3:18F7/1058:18C1], audio card, P-ras card reader [PCI: 0DC3:0802]

  * Lindbergh Red                   (AAHE, 845-00xxD, "ASSY CASE LBJ L 512MB *", "ASSY CASE LBJ L 1GB *" [EX])
        Case: red, Lindbergh R logo top left
              red, Lindbergh R logo top left, EX sticker top center [EX]
        MBD:  838-14673?
        CPU:  Intel Celeron 2.8GHz
        RAM:  1x 512MB
              2x 512MB? [EX]
        GPU:  Nvidia GeForce 7600GS [PCI: 10DE:02E1]
        CF:   MDA-C0004A
        IDE1: ??? 40GB
        OS:   MontaVista Linux
        IO:   JVS card [PCI: 0CA3:18F7/1058:18C1], audio card(sometimes)

  * Lindbergh Red Terminal [Silver] (AAHE, 845-50xxD, "TOP ASSY LBJ *") [-10: server, -20: satellite, -30: live]
        Case: silver, game & role & red R sticker top left, Lindbergh & SEGA & all.net P-RAS logo top center, "所有" top right, serial top far right
        MBD:  ???
        CPU:  Intel Celeron 2.8GHz?
        RAM:  2x 256MB?
        GPU:  Nvidia GeForce 7600GS?
        CF:   MDA-C0004A?
        IDE1: ??? 40GB
        OS:   MontaVista Linux
        IO:   JVS card [PCI: 0CA3:18F7/1058:18C1], P-ras card reader [PCI: 0DC3:0802]
```

## Ring

```
  * RingEdge             (AAL, JP, 846-0001D, "ASSY CASE EDG W") [known revisions: 0, 1]
        MBD: MSI MS-9667 VER:1.0 (838-14852) [revision 0]
             Advantech DAC-BJ01 Rev.A1 (838-15014-01-91 / 19A8BJ0103 / 9696BJ0102E) [revision 1]
        CPU:
        RAM: 1x Transcend TS128MLQ64V8J? [1GB, DDR2-800, "1G DDR2 800 DIMM"]
        GPU: Nvidia GeForce 9600 GS (180-10545-0002-A01 / 600-10545-0021-106 A / 900-60545-2321-000 K, BIOS Version 62.94.4F.00.04, Samsung Memory 161-0070-600) [revision 1?]
        IO:  JVS/keychip card 837-14902 [custom connector]
        SSD: MDA-E0005

  * RingWide             (AAM, JP, 847-0001D, "ASSY CASE WDE W 1GB") [known revisions: 0, 1]
        MBD: Supermicro ??? [revision 0]
             Advantech POD-SG02        (838-14905-01 / 19A6SG0203 / 9696SG0201E) [revision 1]
        CPU: Intel Celeron 440
        RAM: 1x Transcend TS128MLQ64V6J [1GB, DDR2-667 CL5]
        GPU: ATI Mobility Radeon HD 2400
        SSD: MDA-E0004
        IO:  JVS/keychip card 837-14902 [custom connector]

  * RingEdge2            (AASE, JP, 846-5001D,    "ASSY CASE RGE2 W 2GB") [known revisions: 0, 1]
  * RingEdge2 MULTi      (AASE, JP, 846-5002D,    https://page.auctions.yahoo.co.jp/jp/auction/478150038)
  * RingEdge2 64GB SSD   (AASE, JP, 846-5003D,    "ASSY CASE RGE2 W M2G S64G")
  * RingEdge2 4GB MEMORY (AASE, JP, 846-5004D,    https://page.auctions.yahoo.co.jp/jp/auction/q375559711 / https://page.auctions.yahoo.co.jp/jp/auction/570113570)
        MBD: Advantech DAC-BJ02 Rev.A1 (838-15116-91 / 19A8BJ0203 / 9696BJ0203E)
        CPU: Intel Core i3-540
        RAM: 1x Transcend TS256MLK64V3N [2GB, DDR3-1333, "2G 1Rx8 DDR3 1333 U"]
        GPU: Nvidia GeForce GT545
        SSD: MDA-E0007A [846-5001D]
             MDA-E0011  [846-5003D]
        HDD: MDA-H0010C [846-5002D]
        IO:  JVS/keychip card 837-14902 [custom connector]
        PSU: Delta EDPS-250AB A [250W]
```

## ELEFUN

## Nu

```
  * Nu              (AAVE, JP, 848-0001D, "ASSY CASE NU W HDD")
  * Nu1.1           (AAVE, JP, 848-0002D, "ASSY CASE NU W HDD 750 TI")
        MBD: Advantech DAC-BJ05 (838-15284 / 19A2BJ0500-01) [AIMB-582 derivative]
        CPU: Intel i3-3220
        RAM: 2x Transcend TS256MLK64V6N [2GB, DDR3-1600, "2G 1Rx8 DDR3 1600 U"]
        GPU: Nvidia GeForce GTX 650Ti [Nu]
             Nvidia GeForce GTX 750Ti [Nu1.1]
        SSD: MDA-E0010 [Nu]
             MDA-E0012 [Nu1.1]
        HDD: HGST HTB-TT5SAE500(B) [500GB]
        IO:  JVS/RS232/CAN card 837-15280 [PCIe: 11DB:????]
        PSU: Delta EDPS-250AB A [250W]

  * Nu2             (AAVE, JP, 848-2001D, "ASSY CASE NU2")
        MBD: Gigabyte MDH11BM [837-15384]
        CPU: Intel Core i5-6500
        RAM: 2x SK Hynix HMA451U6AFR8N [4GB, DDR4-2133]
        GPU: Nvidia GeForce GTX 950 (BIOS 84.06.5A.00.05)
        SSD: TDK GBDisk GS1 120GB [MDA-E0013]
        PSU: Tiger Power TG-4080 [400W]

  * NuSX            (AAWE, JP, 848-1001D, "ASSY NUSX GAMEBOARD")
  * NuSX1.1         (AAWE, JP)
    MBD: ??? (838-15297 / IAI5I013X14A70042) [NuSX]
    TPM: Infineon SLB9635TT12
    APU: AMD R-268D [NuSX]
    RAM: 1x Transcend TS512MLK64W6H [NuSX, 4GB, DDR3-1600, "4G 1Rx8 DDR3L 1600 U"]
         1x ??? [NuSX1.1, 8GB]
    HDD: MDA-H0013 [NuSX]
    IO:  JVS/RS232/CAN card 837-15315 [PCIe: 11DB:6678]
```

## ALLS

```
  * ALLS UX                       (ACAE, JP, 849-0003, "ASSY CASE ALLS UX")
  * ALLS UX  (with sub-storage)   (ACAE, JP, 849-0004)
  * ALLS UX  (with sound board)   (ACAE, EX, 849-0005, "ASSY CASE ALLS UX W S/B")
        MBD: Gigabyte MDH11BM
        CPU: Intel Core i5-6500
        RAM: 2x SK Hynix HMA81GU6AFR8N-UH [8GB, DDR4-2400]
        GPU: ELSA GeForce GTX1070 8GB ST for SEGA
        SSD: TDK GBDisk GS1 120GB [MDA-E0017]
        HDD: HGST HTS725050A7E630 500GB [849-0004, 849-0005]
        PCI: "SoundBlaster" [849-0005]
        PSU: ???

  * ALLS HX                       (ACAX, JP, 849-0006, "ASSY CASE ALLS HX")
        MBD: Gigabyte MDH11BM
        CPU: Intel Core i5-6500
        RAM: 2x SK Hynix [4GB, DDR4-2133]
        GPU: Nvidia GeForce GTX 1050
        SSD: TDK GBDisk GS1 120GB [MDA-E0017]
        PSU: ???

  * ALLS UX2                      (ACAE, JP, 849-1001?)
  * ALLS UX2 (with sub-storage)   (ACAE, JP, 849-1002?)
        MBD: Gigabyte MCH31AM-S2
        CPU: ???
        RAM: 2x 8GB
        GPU: Gigabyte GeForce RTX 2070 WINDFORCE 8G?
        SSD: TDK GBDisk GS1 120GB [MDA-E0019]
        HDD: ???
        PSU: ???

  * ALLS HX2                      (ACAX, JP, 849-1003, "ASSY CASE ALLS HX2")
  * ALLS HX2 (with sub-storage)   (ACAX, JP, 849-1004, "ASSY CASE ALLS HX2 W HDD")
  * ALLS HX2 OP                   (ACAX, ??, 849-1???)
        MBD: Gigabyte MCH31AM-S2
        CPU: Intel Core i3-8100
        RAM: 2x 4GB
        GPU: Nvidia GeForce GTX 1050Ti
        SSD: TDK GBDisk GS1 120GB [MDA-E0019]
        HDD: Western Digital WD5000LUCT 500GB
        PSU: ???

  * ALLS MX2                      (ACA?, JP, 849-1005)
  * ALLS MX2 (with sub-storage)   (ACA?, JP, 849-1006)
  * ALLS MX2.1                    (ACA?, JP, 849-1009)
  * ALLS MX2.1 (with sub-storage) (ACA?, JP, 849-1010)
        MBD: ???
        CPU: ???
        RAM: 2x 8GB
        GPU: Nvidia GeForce GTX 1060 [MX2]
             Nvidia GeForce GTX 1660Ti [MX2.1]
        SSD: ???
        HDD: ??? [849-1006, 849-1010]
        PSU: ???

  * ALLS X2                       (ACA?, JP, 849-1007?)
  * ALLS X2 (with sub-storage)    (ACA?, JP, 849-1008?)
        MBD: ???
        CPU: ???
        RAM: 2x 4GB
        GPU: integrated
        SSD: ???
        HDD: ???
        PSU: ???
```
