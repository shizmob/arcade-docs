# Konami Identifiers

This file describes the various identifiers and their formats that are used in products by Konami.

## Sources

* [bemaniwiki](http://bemaniwiki.com/)
* Game/cabinet manuals
* MAME
* Various sources around the internet
* Game data

## Format

The format of each identifier/ID is described as a perl/php/shell-style string with `$` denoting
that a variable is resolved, e.g. `$a` "resolve variable a". Additionally, a more complex regex
string is provided to constrain the format properly.

### Variables and values

The following variables are used across the different identifiers and can denote the listed values:

* `$p`: Product category
  * `B`: Consumer hardware
  * `C`: Consumer hardware, cards
  * `G`: Arcade games
  * `H`: Hardware? e.g. card dispenser
  * `M`: Consumer games
  * `R`: Consumer games
  * `V`: Consumer games
  * `Y`: Consumer hardware?
* `$t`: Product type
  * Category `B`:
    * `H`: LCD game
  * Category `C`:
    * `F`: Fanclub cards
    * `M`: こなみるく (KonaMilk) cards
    * `T`: BEMANI POCKET
  * Category `G`:
    * `C`: Conversion kit: Software/rom/art/dongle only
    * `E`: Conversion kit: Software + hardware
    * `G`: Gambling/slot/casino hardware/board?
    * `K`: Cabinet manufactured by third party?
    * `L`: Redemption cabinet?
    * `M`: Cabinet?
    * `N`: Cabinet manufactured by third party?
    * `O`: Cabinet?
    * `P`: Cabinet?
    * `Q`: Cabinet
    * `S`: Medal cabinet (station?)
    * `U`: Conversion kit: Upgrade or utility: Hardware/art only
    * `V`: Cabinet (System GV)
    * `X`: Hardware/board?
    * `Y`: ???
    * `Z`: ???
  * Category `H`, `Y`:
    * `A`: ???
    * `B`: TV game
    * `C`: CD-rom?
    * `O`: hardware?
  * Category `M`:
    * `E`: Windows 95 (floppy, cdrom)
    * `F`: Mac
  * Category `R`:
    * `A`: MSX, PC-98, X68000 (Floppy)
    * `C`: MSX (Cartridge), Famicom
    * `D`: NES (North America, Europe)
    * `E`: GB (prototype?)
    * `G`: SNES (North America)
    * `H`: SNES (Europe)
    * `I`: Wii (Japan)
    * `K`: GB, GBC, GBA (Japan)
    * `L`: Switch (Japan)
    * `Q`: Gamecube (Japan)
    * `R`: 3DS (Japan)
    * `S`: Super Famicom
    * `U`: Controllers
    * `V`: Famicom
    * `Y`: DS (Japan)
    * `Z`: Nintendo 64 (Japan)
  * Category `V`:
    * `C`: Dreamcast (Japan)
    * `F`: PS4 (Japan)
    * `K`: Xbox 360 (Japan)
    * `M`: Xbox (Japan)
    * `N`: PS Vita (Japan)
    * `P`: PSP (Japan)
    * `S`: Saturn (Japan)
    * `T`: PS3 (Japan)
    * `W`: PS2 (Japan)
    * `X`: PS1 (Japan)
    * `Z`: 3DO (Japan)
* `$g`: Gamecode, identifies a game or series in [Konami's product portfolio](products.md)
  * Format: `yxx`
    * `y`: `A` + (project development start year - 2000) (`L`: 2011, `T`: 2019, etc.)
    * `xx`: Remainder, (incremental) game/product identifier
  * Example: `LDJ`
* `$d`: Destination, target locale/market
  * `A`: Asia
  * `C`: China
  * `E`: Europe
  * `H`: Hong Kong (Asia 220V; software is often/always? A-region)
  * `J`: Japan
  * `K`: Korea
  * `S`: Singapore? (Asia 220V; software is often/always? A-region)
  * `T`: Taiwan (Asia 110V; software is often/always? A-region)
  * `U`: US
  * `Y`: Indonesia
* `$s`: Specification: Product type and game dependent, e.g. type of cabinet or hardware
  * `A`, `B`, `C`, ..., `Z`
  * コナステ streamed games use `N`
  * In some [System 573](boards.md#system-573) and [Firebeat](boards.md#firebeat) games, rental cabinets (at the time referred to as e-Amusement: not the online network!) use `R`
* `$r`: Software revision. Modern games utilizing the extension part pinned this to the value `A`
  * `A`, `B`, `C`, ..., `Z`
* `$e`: Extension/release date of the software
  * Format: `yyyymmddnn`
    * `yyyy` = year, e.g. `2020`
    * `mm` = month, e.g. `11` for November
    * `dd` = day of month, e.g. `03`
    * `nn` = release number on the day, e.g. `00`, `01`, ...
    * Older games may omit `nn`, example: `FK9:J:A:A:20060217`
  * Example: `2018073002`

## Identifiers

### Product identifier

[Packages](products.md) that can be acquired, e.g. bought or leased.

* Format: `$p$t$g-$d$s`
* Example: [GQLDJ-JA](product/GQLDJ-JA.md)

### Part number

Usually indicated with `PN` or `PWB`. Any kind of specific part, manual or anything else that can be acquired.

* Source: stickers or labels on product
* Formats:
  - A: `$g$N` (game-specific part)
  - B: `$T$N` (generic part)
  - C: `$L` (used from roughly 1998 onwards)
  - D: `$M0000` (used from roughly 2005 onwards)
* Variables:
  - `$T`: part type, known values:
    * `30`: button, switch, joystick
    * `35`: power supplies, transformers
    * `40`: monitors, glass, bezels
  - `$N`: A three-digit number, e.g. `205`
  - `$L`: An eleven-digit number, e.g. `00000058559`
  - `$M`: An eight-digit number, e.g. `11003358`
* Examples:
  - `A00400`: format A; the US Police 911 (`A00`) operator's manual
  - `0000068482`: format C; the US DanceDanceRevolution GN845-UC operator's manual
  - `110033580000`: format D; the US DanceDanceRevolution GQMDX-UD operator's manual

### Serial number

* Source: stickers on hardware
* Formats:
  - A: `$N`
  - B: `$g$N`
  - C: `$g $t$d$s $S` (maybe not a serial number?)
  - D: `$g$t$d$s$N`
* Variables:
  - `$N`: A six-digit number, e.g. `038902`
  - `$S`: A four-digit number, e.g. `0104`
* Examples:
  - `812169`: number `812169`, found on `533` (Sexy Parodius)
  - `FDH EUA 0104`: corresponds to [product identifier](#product-identifier) `*EFDH-UA` (DanceDanceRevolution SuperNOVA), number `0104`; found on EXTIO
  - `FDHKUA012905`: corresponds to [product identifier](#product-identifier) `*KFDH-UA` (DanceDanceRevolution SuperNOVA), number `012905`: found on EXTIO
  - `MBRQJA038902`: corresponds to [product identifier](#product-identifier) `*QMBR-JA` (REFLEC BEAT), number `038902`

### ROM identifier

* Source: stickers and labels
* Formats:
  - `$p $R$N`
  - `$p $d$s $R$N`
* Variables:
  - `$R`: A single letter
    * Sometimes indicates revision (`$r`)
    * In modern PC setups, replaced with `*` on a case sticker
  - `$N`: Two digits
    * Indicates the type of ROM
* Examples:
  - `700 A01`: System 573 (`700`) BIOS ROM
  - `C23 EA A02`: Dancing Stage EuroMIX2 (`C23`) game CD-ROM

### Mcode, Contents Code

* Source: License dongle certificate CN, game data
* Format: `$g-$N`
  * `$N`: An three-digit number, e.g. `001`
* Example: `PIX-001`

### Security code

* Source: License dongle certificate subjectAltName
* Format: `$p$t$g$d$s$r`
* Example: `GQPIXJBA`

### Release code

* Source: Game data
* Format: `$e`
* Example: `2018073002`

### System ID

* Source: Account dongle certificate CN
* Format: `0120$X0$Y`
  * `$X`: `1` or `2`
  * `$Y`: 14-digit hex string
* Example: `0120100000000160B3D2`

### License ID

* Source: License dongle serial number
* Format: `0121$X`
  * `$X`: 8-digit numeric value
* Example: `012194810293`

### Account ID

* Source: Account dongle serial number
* Format: `0122$X`
  * `$X`: 8-digit numeric value
* Example: `012291862492`

### Hardware ID

* Source: MAC address
* Format: `0100$X`
  * `$X`: 12-digit hex string
* Example: `0100705CAD0365F2`

### Software ID

* Alias for License ID

### Soft ID code

* Source: [Security code](#security-code) and [release code](#release-code) combined and shown in-game
  * Some games change the soft ID, for example jubeat: `GQL44JBA` (security code) -> `L44:J:F:A` (in-game)
* Format: `$g:$d:$s:$r:$e`
* Example: `PIX:J:B:A:2018073002`
