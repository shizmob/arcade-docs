# NAMCO identifiers

This file describes the various identifiers and their formats that are used in products by NAMCO.

## Generic fields

### Game code

A sequence of three letters or numbers that identifies a specific NAMCO title. Example: `TE7` is Tekken 7.

### Region code

A single digit indicating the region for a specific release.

* `1`: JPN / (unreadable kanji)
* `2`: ASIA / 一般海外 ASIA
* `3`: EXP / EXP、NAI
* `4`: CHINA (https://www.ebay.co.uk/itm/165005792426?mkevt=1&mkcid=1&mkrid=710-53481-19255-0&campid=5338722076&toolid=10001)
* `5`: CHINA
* `6`: 

### Cabinet role

A sequence of two letters indicating the cabinet role for a specific release.

* `CT`: counter?
* `LM`: live monitor?
* `NA`: normal?
* `RS`: ?
* `ST`: station?
* `TM`: terminal?
* `TW`: medal/card game?

## Part number

## Product code

Components:
- `$g`: [game code](#game-code), `[A-Z0-9]{3}`
- `$v`: version, `[0-9]`
- `$r`: revision, `[A-B]`
- `$R`: revision, `[A-B][0-9]{2}`
- `$l`: [region code (locale)](#region-code), `[0-9]`
- `$a`: unknown, `[0-9]`
- `$b`: unknown, `[0-9]`
- `$c`: [cabinet role](#cabinet-role), `[A-Z]{2}`
- `$t`: type, `[A-Z]{4}`
  * `MPRO`: M production? (on ES2 HDD, ES4 HDD)
  * `HDD0`: HDD (on N2 case)
  * `DAT0`: data (on ES1 HDD)
- `$u`: unknown, `[A-Z]{2}`

Formats:
- `$g$v-$u`
  * Used in System 256 case & HDD
  * Examples:
    - `TSF1-HA`: game code TSF, version 1, $u HA
- `$g$v$a$b$l-$c-$r`
  * Used in System 256 dongle
  * Examples:
    - `TSF1002-NA-A`: game code TSF, version 1, $a 0, $b 0, locale 2?, cabinet role normal, revision A
- `$g$v$a$b$l-$c-$t-$r`
  * Used in early System N2
  * Examples:
    - `WM31003-NA-HDD0-A`: game code WM3, version 1, $a 0, $b 0, locale Export, cabinet role normal, type HDD, revision A
- `$g$v$a$b-$l-$c-$t-$r`
  * Used in System 369, late N2, ES1, ES2, ES2+, ES3, ES4
  * Examples:
    - `W3P100-2-NA-DAT0-A`: game code W3P, version 1, $a 0, $b 0, locale Asia, cabinet role standard, type data, revision A
    - `TTT103-3-ST-DAT0-A`: game code TTT, version 1, $a 0, $b 3, locale Export, cabinet role station, type data, revision A
    - `TG2100-2-LM-HDD0-A`: game code TG2, version 1, $a 0, $b 0, locale Asia, cabinet role live monitor, type hard drive, revision A
    - `PBN100-1-NA-MPRO-A`: game code PBN, version 1, $a 0, $b 0, locale Japan, cabinet role normal, type M production, revision A
    - `GCB100-1-TW-MPRO-B`: game code GCB, version 1, $a 0, $b 0, locale Japan, cabinet role TW, type M production, revision B
    - `GKE300-1-TM-DAT0-A`: game code GKE, version 3, $a 0, $b 0, locale Japan, cabinet role terminal, type data, revision A
- `$g$v$a$b-$l-$c-$t-$R`
  * Used in late ES3, ES4, BNA1
  * Examples:
    - `MHM200-1-NA-MPR0-C01`: game code MHM, version 2, $a 0, $b 0, locale Japan, cabinet role normal, type M production, revision C01
    - `T46430-1-CT-MPR0-F03`: game code T46, version 4, $a 3, $b 0, locale Japan, cabinet role CT, type M production, revision F03

## Dongle serial

Components:
- `$g`: game code, `[0-9]{4}`
- `$r`: [region code](#region-code), `[0-9]`
- `$c`: cabinet role, `[0-9]`
- `$t`: title code, `[0-9]{2}`
- `$n`: serial number, `[0-9]{4}`

Formats:
- `a$d$c$a $t$na`
  * Examples:
    - `a274811 260532a`: game #2748, region Japan, cabinet role 1, title 26, serial number 0532
    - `a2793 13393143a`: game #2793, region Japan, cabinet role 3, title 39, serial number 3143

Unknowns:
- System 256 dongle (memory card): `a 026161 351019 a`
- System N2 W3X (Asia) dongle: `a 026441 275842 a`

## Net ID

Components:
- `$x`: unknown, `[A-Z]`
  * `D`:
  * `E`:
  * `G`:
- `$c`: cabinet role, `[0-9]`
- `$t`: title code, `[0-9]{2}`
- `$n`: serial number, `[0-9]{4}`

Formats:
- `AB$xN-$a$t$n`
  * Examples:
    - `ABGN-1260532`: unknown G, cabinet role 1, title 26, serial number 0532
    - `ABEN-3393143`: unknown E, cabinet role 3, title 39, serial number 3143
