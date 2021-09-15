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
  * `G`: Game
  * `H`: Hardware/Helper? e.g. card dispenser
* `$t`: Product type
  * `A`: ???
  * `C`: Conversion kit: Software/rom/art/dongle only
  * `E`: Conversion kit: Software + hardware
  * `K`: Cabinet manufactured by third party?
  * `L`: Redemption cabinet?
  * `M`: Cabinet?
  * `N`: Cabinet manufactured by third party?
  * `O`: Cabinet?
  * `P`: Cabinet?
  * `Q`: Cabinet
  * `S`: Medal cabinet (station?)
  * `U`: Conversion kit: Upgrade or utility: Hardware/art only
  * `X`: Conversion kit: Hardware/board?
  * `Z`: ???
* `$g`: Gamecode, identifies a game or series in [Konami's product portfolio](products.md)
  * Format: `yxx`
    * `y`: `A` + (project development start year - 2000) (`L`: 2011, `T`: 2019, etc.)
    * `xx`: Remainder, (incremental) game/product identifier
  * Example: `LDJ`
* `$d`: Destination, target locale/market
  * `A`: Asia
  * `C`: China
  * `E`: Europe
  * `H`: Asia (220V)
  * `J`: Japan
  * `K`: Korea
  * `T`: Asia (110V)
  * `U`: US
  * `Y`: Indonesia
* `$s`: Specification: Product type and game dependent, e.g. type of cabinet or hardware
  * `A`, `B`, `C`, ..., `Z`
  * コナステ streamed games use `N`
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

* [Products or packages](products.md) that can be acquired, e.g. bought or leased
* Format: `$p$t$g-$d$s`
* Example: [GQLDJ-JA](product/GQLDJ-JA.md)

### Serial number

* Source: stickers on hardware
* Format: `$g$t$d$s$n`
  * `$n`: A six-digit number, e.g. `038902`
* Example: `MBRQJA038902`, corresponds to [product identifier](#product-identifier) `*QMBR-JA`, number `038902`.

### Mcode, Contents Code

* Source: License dongle certificate CN, game data
* Format: `$g-$n`
  * `$n`: An three-digit number, e.g. `001`
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
* Format: `0120$x0$y`
  * `$x`: `1` or `2`
  * `$y`: 14-digit hex string
* Example: `0120100000000160B3D2`

### License ID

* Source: License dongle serial number
* Format: `012$x$y`
  * `$x`: `1` or `2`
  * `$y`: 8-digit numeric value
* Example: `012194810293`

### Account ID

* Source: Account dongle serial number
* Format: `012$x$y`
  * `$x`: `1` or `2`
  * `$y`: 8-digit numeric value
* Example: `012291862492`

### Hardware ID

* Source: MAC address
* Format: `0100$y`
  * `$y`: 12-digit hex string
* Example: `0100705CAD0365F2`

### Software ID

* Alias for License ID
* Format: `012$x$y`
  * `$x`: `1` or `2`
  * `$y`: 8-digit numeric value
* Example: `012194810293`

### Soft ID code

* Source: [Security code](#security-code) and [release code](#release-code) combined and shown in-game
  * Some games change the soft ID, for example jubeat: `GQL44JBA` (security code) -> `L44:J:F:A` (in-game)
* Format: `$g:$d:$s:$r:$e`
* Example: `PIX:J:B:A:2018073002`
