# SEGA identifiers

This file describes the various identifiers and their formats that are used in products by SEGA.

## Part number

A generic identifier for a physical part. Seems to have been introduced by Gremlin Industries and continued by SEGA upon acquisition way back in 1978.

Format: `[0-9]{3}-[0-9A-Z]+`. The first part indicates the part category, the second part the identifier.

Examples:
* `842-0001A`: Triforce Type 1 board.

Known part categories (tree view):

```
0  - small auxiliary parts
 00: M SCREW
   P: PH
   T: TH
 08: TMP PRF SCREW
   T: TH
   B: BH
 10: S-TITE SCREW
   P: PH
   F: FH
 11: TAP SCREW #1
   P: PH
   T: TH
   F: FH
 12: TAP SCREW #2
   P: PH
 20: HEX SOCKET CAP SCR
   B: BH
   F: CSK
 28A: SET SCR HEX SOCKET CUP
 29: M(HEX) SOCKET
   B: BH
 30: HEX BOLT
 31: CRG BOLT
 32: WING BOLT
 45: PIN
   C: COT
   SU: SPRING
 50: NUT
   H: HEX
   F: FLG
   C: CAP
   U: U (NYLOC?)
 60: WASHER
   S: SPR
   F: FLT
 65: RING
   C: CIRCLIP
   S: STP
   E: E
 68: FLT WASHER
 73: O-RING
 79: "SCR NAIL THH STNLS"
 90: GREASE
 99: CORD (US?)
1  - medium-size auxiliary parts
 00: BEARING / CAM
 05: METAL BRACKET?     ("FAN BRKT LONG" / "HINGE" / "SHIELD CASE BRKT" / "SHIELD CASE" / "CHUTE PLATE" / "SHIPPING BRKT" / "TRAY")
 09: "KEY HOLDER"
 11: COUPLING MJT-40K-BL
 17: METAL PLATE?     (PLATE RETAINER / "EARTH TERMINAL PLATE" / "TERMINAL 3P" / "TNG RETAINER PLATE" / "PLATE LOCK" / "SHAFT WASHER" / "BASE PLATE" / PLATE 6-80 BLACK)
 23: SHAFT PIN
 25: "SPRING COMP MSR LEVER" / "SPRING TRIGGER"
 30: SPEAKER
 40: "COVER J-BOX" / "CABINET UNIV UPR"
 50: CAPACITOR (E) [electrolytic?]
 51: CAPACITOR (CERAMIC)
 52: CAPACITOR (FILM)
 53: CAPACITOR (TANT)
 70: BARE BD
 71: BARE BD
2  - medium-size auxiliary parts, displays, connectors, sockets, accessories
 00: DISPLAY
 09: CONN TERMINATOR? ("CONN CLOSED END")
 11: CONNECTOR        ("CONN OPT JOINT" / "CONN PIN TEST PT" / "CONN RING LUG")
 12: CONNECTOR        ("CONN JST" / "CONN M")
 13: SOCKET
 14: SOCKET           ("AC INLET PANEL TYPE" / "BULB SKT (ES-T250-E17)" / "SOCKET E11 W/CONN VL WH")
 20: METAL ACCESSORY?     (KEY / "CAM LOCK MASTER W/O KEY" / "VOL CONT B-5K OHM" / "MAG CNTR DC5V W/CONN" / "COIN ENTRY" / "VOL CONT" / "MAG CNTR DC5V")
   -5574: CAM LOCK W/KEYS
   -5575: CAM LOCK MASTER W/O KEY
   -5576: KEY MASTER FOR 220-5575
   -5793-1: MASTER LOCK  [A001]
   -5793-2: MASTER KEY   [A001]
   -5794:   COIN LOCK W/ KEYS
 30: XTAL
 40: "BLACK PUSHBUTTON CONTROL" / "JOYSTICK KNOB" / "BUTTON PLUNGER"
 50: METAL ACCESSORY?    ("REJECT BUTTON ASSEMBLY" / "THREADED ROD" / "UPPER SLEEVE" / "COPPER STRAP" / "MOLDING STRIP" / "CLAMP COMPONENT BD")
 53: PLASTIC ACCESSORY?  ("FL HOLDER" / "AIR VENT BLACK" / "WATER BOTTLE 500CC" / "CASH BOX" / KEYCHIPS)
   -5508-*: NAOMI/Triforce/Chihiro/System SP/Lindbergh keychip (SEGA)
   -5509-*: NAOMI/Triforce/Chihiro/System SP/Lindbergh keychip (licensed)
   -5640-*: Lindbergh Terminal keychip
   -5644-*: RINGEDGE/RINGWIDE keychip (SEGA, black)
   -5645-*: RINGEDGE/RINGWIDE keychip (licensed, black)
   -5646-*: RINGEDGE/RINGWIDE keychip (SEGA, red)
 60: FAN
 70: NOISE FILTER / "FERRITE CORE" / L.FILTER
 75: GLASS
 80: CLAMP/TIE/HINGE     (CORD CLAMP / "REAR HINGE" / "TERMINAL BINDING POST" / "HARNESS LUG" / "SCRIVET" / "SPACER HEX" / "SPACER FAI" / REPEAT TIE RF140 / BUSH / COLLAR)
 81: SCREW ("SCR PN HD Phil S/M Type A/AB 6-18 X 2.00 LG")
 82: BOLT
 83: NUT
 84: WASHER
 86: SCREW ("SCR PN HD Phil S/M Type A/AB 8-15 X .750 LG BLACK")
3  - tubes, ICs, motors, sensors, lamps
 10: "SUMITUBE F F 20MM" / PAPER INSL / VINYL TUBE / "INSL XSTR To-220"
 13: IC JELLYBEAN OP-AMP / VRM?    ("LM348"/"LM741")
 14: IC JELLYBEAN LOGIC? ("555"/"74LS374"/"74LS245"/"74LS138"/"74LS253"/"7406"/)
 15: IC ASIC?
 16: IC ROM?
 17: IC THIRD-PARTY?
 50: MOTOR / "TIMING BELT 300 S3M 06" / "CLUTCH TMC-10E-26"
 70: "MOTION SENSOR" / "PHOTO SENSOR"
 90: LAMP / EXT ELECTRODE / LED STRIP / LED
 00: "SW REGU" / INVERTER / PSU
4  - manuals, stickers, emblems, batteries, electronic parts
 01: BATTERY
 20: MANUAL / STICKER / DECAL
 21: STICKER / FILM
 22: PLAY INSTR
 23: EMBLEM
 40: STICKER
   W: WARNING
   D: D
   C: C
 41: STICKER PART NUMBER
 42: STICKER ("SHIELD CASE STICKER")
 43: SERIAL STICKER
 50: "MAGNET CONTACT S-NIOCX" / TIMER RELAY
 70: RESISTOR ("RESISTOR 1K, 1/4W, 5%")
 71: RESISTOR
 75: POTENTIOMETER
 77: "RES PACK"
 81: DIODE
 82: TRANSISTOR
5  - switches, fuses, wrenches, transformers
 09: SWITCH/BUTTON/TOUCH PANEL
 10: SWITCH/STICK
 12: CURRENT PROTECTOR / FUSE  ("C.P 15000MA CE UL" / "C.P 5A CE UL")
 14: FUSE / INLET?
 30: HEAT SINK
 40: WRENCH
 53: MANUAL? (US?)
 60: TRANSFORMER
6  - wires, media, misc
 00: WIRE/CABLE
 01: CARTON BOX / KIT / KNOB / L-LOCK BK / YURIA M4×12 BLACK K-UN / OUTLET AC F / CHAIN LATCH / CHAIN W FOOK / FAN GUARD / BUSH 1.2T 180MM
 05: CABLE (SCSI?)
 10: MEDIA (RETAIL)?
   -0624-xxxx:  NAOMI GD-ROM
   -0630-xxxx:  NAOMI GD-ROM
   -0650-xxxx:  Triforce GD-ROM
   -0652-xxxx:  Chihiro GD-ROM
   -0726-xxxx:  Lindbergh DVD
   -0727-xxxx:  Lindbergh DVD + keychip
   -0719:       Lindbergh DVD drive
   -0817-xxxx:  RingEdge/RingWide DVD ("DVD SOFT KIT *")
   -0837-xxxYY: ELEFUN keychip
   -0890-xxxYY: Nu keychip (SEGA, black)
   -0891-xxxYY: Nu keychip (licensed, black)
   -0892-xxxYY: Nu keychip (SEGA, red)
   -0893-xxxYY: Nu keychip (SEGA, blue)
   -0894-xxxx:  Nu DVD
   -0937-xxxYY: Nu2/ALLS keychip (SEGA, black)
   -0938-xxxYY: Nu2/ALLS keychip (licensed, black)
   -0939-xxxYY: Nu2/ALLS keychip (SEGA, red)
   -0941-xxxYY: Nu2/ALLS keychip (SEGA, blue)
   -0945-xxxx:  ALLS DVD
 11: MEDIA (DEV)?
7  - assembly
 00: ASSY
 31: WIRING DIAGRAM?
 32: WIRING DIAGRAM?
8  - assembly
 12: COIN MECH?
 31: HARNESS?
 33: GAME BD
 34: ROM BD / MAIN BD
 36: ??? https://page.auctions.yahoo.co.jp/jp/auction/f498150600
 37: COMM BD / EXTEND SOUND BOARD
 38: CONNECT BD  (SW BD NAOMICABINET / CONNECT BD W/FUSE & COVER / RS422/RS232C BD DOC / PWR AMP 2CH & MIXER / SERVO MOTOR DRIVE BD MIDI / SOUND AMP ANALOG IN / DC SEQUENCE BD / BASS AMP 50W X 1)
 39: AUX BD      (WINNER LED BD / CATCH SUGATSUNE / CONN BD / SSR BD / FLT BD NAOMI MULTI MASTER FRI / MOTOR DRIVE BD / TERMINAL BD)
 40: NAOMI/NAOMI2 assembly ("ASSY CASE NAO" / "ASSY CASE NAT")
 42: Triforce assembly ("ASSY CASE TRF")
 43: Chihiro assembly ("ASSY CASE BOX")
 44: Lindbergh assembly ("ASSY CASE LBG")
 45: Lindbergh Red ("Junior") assembly ("ASSY CASE LBJ")
 46: RingEdge assembly ("ASSY CASE RGE")
 47: RingWide assembly ("ASSY CASE WDE")
 48: Nu assembly ("ASSY CASE NU")
 49: ALLS assembly ("ASSY CASE ALLS")
9  - misc
 90: SCREW
 91: BRACKET/CLAMP (METAL?)
 92: BRACKET/CLAMP (PLASTIC?)
 98: SANWA MONITOR (31K MODE) (CONTROL PANEL?)
 99: US PARTS
```

Specific for board assemblies (84x):

```
8aa-bbbbC(-DE)(-FG)
8aa-bbCHiiiiJ [Triforce Type 3]

   aa: hardware line:
        40: NAOMI
        41: NAOMI (licensed)
        42: Triforce
        43: Chihiro
        44: Lindbergh, Lindbergh Blue
        45: Lindbergh Red
        46: RingEdge, RingEdge2
        47: RingWide
        48: Nu
        49: ALLS
 bbbb: part identifier
    C: part type:
        A:  case/assembly (board)
        B:  case/assembly (game DIMM)
        C:  cartridge
        D:  case/assembly (board + game kit)
        E:  communication board?
        F:  DIMM board
    D: (optional) unknown
    E: (optional) unknown
    F: (optional) part revision
    G: (optional) region:
        0: Japan
        1: USA
        2: Export/Others
        3: Korea
        4: Australia
        5: Japan again? (https://page.auctions.yahoo.co.jp/jp/auction/s838966167 / https://archive.is/mIPSU)
        6: USA again?   (https://segaretro.org/images/7/79/WaveRunnerGP_NAOMI_US_Manual_Standard.pdf, page 54)
        7: ?
        8: ?
    H: (optional) media type:
        D: DIMM
        N: NAND
 iiii: unknown, part revision?
    J: (optional) region:
        J: Japan
        U: USA
        E: Export
```

## Serial number

A specific identifier for a physical product. Seems to have been introduced around the NAOMI launch.

Format: `[A-Z]{4}-[0-9]{2}[A-Z][0-9]+`. The first part indicates the product type, second and third possibly the batch, and the fourth the identifier.

Known product types (tree view):

```
A  - game boards, keychips
 AA  - NAOMI
   H
 AB  - Hikaru (ROM board: BDXE)
 AC  - NAOMI 2
 AD  - Triforce
 AE  - Chihiro
 AF  - System SP/Aurora
   E
   G
 AG  - Lindbergh
   E
   R
 AH  - Lindbergh Red
 AI  - ?
 AJ  - Lindbergh Blue
 AK  - ?
 AL  - RingEdge
   E
   G - https://page.auctions.yahoo.co.jp/jp/auction/s838250888 / https://page.auctions.yahoo.co.jp/jp/auction/s841919444
 AM  - RingWide
   L
   K
 AN  - ?
 AO  - ?
 AP  - ?
 AQ  - ?
 AR  - ELEFUN
 AS  - RingEdge2
 AT  - ?
 AU  - ?
 AV  - Nu
   0 - Nu
   1 - Nu1.1
   2 - Nu2
 AW  - NuSX
   0 - NuSX
   1 - NuSX1.1
 AX  - ?
 AY  - ?
 AZ  - ?
 BA  - ?
 CA  - ALLS
   E - ALLS UX
   X - ALLS HX
 60  - Nu keychip
 61  - Nu/NuSX keychip
 63  - ALLS keychip
 67  - NuSX AMEX
 69  - Nu/NuSX keychip
 71  - ELEFUN keychip
 72  - RingEdge/RingWide/RingEdge2 keychip
 87  - Chihiro media board
B  - ROM boards
```

Example:
* `AAVE-01A912938`: Nu gameboard, serial number #912938
* `A72E-01U4539`: RINGEDGE keychip, serial number #4539

## Game ID

Seems to have been introduced around the start of ALL.NET and used from at least the NAOMI2 and Atomiswave onwards.

Format: `S[BD][A-Z]{2}`. `SC**` may be developer IDs?

Examples:
* `SBZZ`: 頭文字D ARCADE STAGE 8 インフィニティ
* `SDCH`: Mario & Sonic at the Rio Olympic Games

Seem to be allocated (semi-)sequentially and roll over when `Z` is reached.

Very early ALL.NET games (Such as VF4 and VF4 Evolution) do not include the S in their game ID.

## Media ID

Seems to have been introduced around the NAOMI launch.

Formats:
* `[A-Z]{3}-[0-9]{4}(-[A-Z0-9]+)*`: Used for install media. The first part indicates the medium type, the second part the identifier, and the third part a version/disc specification. Known medium types:
   - `GDS`: GD-ROM (NAOMI, SEGA)
   - `GDL`: GD-ROM (NAOMI, licensed)
   - `GDT`: GD-ROM (Triforce)
   - `GDX`: GD-ROM (Chihiro)
   - `CDP`: CD  ((NAOMI/Triforce/Chihiro)
   - `CDV`: DVD (NAOMI/Triforce/Chihiro/additional disc)
   - `DVP`: DVD (Lindbergh)
   - `DVR`: DVD (RINGEDGE/RINGWIDE)
   - `CDN`: DVD (Nu/NuSX)
   - `CDA`: DVD (ALLS)
* `MDA-[A-Z][0-9]{4}`: Used for flash and storage media. The first part indicates the medium type, the second part the identifier. Known medium types:
   - `G`: CompactFlash card (NAOMI/Triforce/Chihiro)
   - `C`: CompactFlash card (System SP/Lindbergh)
   - `S`: Secure Digital card
   - `H`: Hard drive
   - `E`: SSD
   - `U`: USB thumbdrive

Examples:
* `DVR-5033A`: RINGEDGE install DVD for 頭文字D ARCADE STAGE 8 インフィニティ
* `MDA-U0066`: RINGEDGE2 install USB for maimai MURASAKi

## Region

A two or three-letter identifier to indicate a region.

```
JPN / JP:  Japan
CHN / CN:  China
USA / US:  America
EXP / EX:  Export
COM /   :  Common (all bits)
      GL:  Global (all bits except JPN and CHN)`
```

## Role

A two-letter identifier to indicate the cabinet role.

```
ST = satellite: play cabinet
SV = server:    server cabinet
LV = live:      spectate cabinet
?? = terminal:  profile checking cabinet
```
