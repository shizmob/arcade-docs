# NAMCO identifiers.

This file describes the various identifiers and their formats that are used in products by NAMCO.

## Generic fields

### Region code

* `1`: JPN
* `2`: USA?
* `3`: EXP/ASIA?
* `5`: CHN
* `6`: 

### Cabinet role

* `LM`: live monitor?
* `NA`: normal?
* `TM`: terminal?
* `TW`: medal/card game?

## Part number

## Product code

Components:
- `$g`: game code, `[A-Z0-9]{3}`
- `$v`: version, `[0-9]`
- `$r`: revision, `[A-B]`
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
  * Used in System 256 case, HDD
  * Examples:
    - `TSF1-HA`: game code TSF, version 1, $u HA
- `$g$v$a$b$l-$c-$r`
  * Used in System 256 dongle
  * Examples:
    - `TSF1002-NA-A`: game code TSF, version 1, $a 0, $b 0, locale 2?, cabinet role normal, revision A
- `$g$v$a$b$l-$c-$t-$r`
  * Used in System N2
  * Examples:
    - `WM31003-NA-HDD0-A`: game code WM3, version 1, $a 0, $b 0, locale Export, cabinet role normal, type HDD, revision A
- `$g$v$a$b-$l-$c-$t-$r`
  * Used in System 369, ES1, ES2, ES2+, ES3, ES4
  * Examples:
    - `TG2100-2-LM-HDD0-A`: game code TG2, version 1, $a 0, $b 0, locale US, cabinet role live monitor, type hard drive, revision A
    - `PBN100-1-NA-MPRO-A`: game code PBN, version 1, $a 0, $b 0, locale Japan, cabinet role normal, type M production, revision A
    - `GCB100-1-TW-MPRO-B`: game code GCB, version 1, $a 0, $b 0, locale Japan, cabinet role TW, type M production, revision B
    - `GKE300-1-TM-DAT0-A`: game code GKE, version 3, $a 0, $b 0, locale Japan, cabinet role terminal, type data, revision A

## Dongle serial

Components:
- `$d`: drawing code, `[0-9]{4}`
- `$r`: [region code](#region-code), `[0-9]`
- `$a`: account code, `[0-9]`
- `$t`: title code, `[0-9]{2}`
- `$n`: serial number, `[0-9]{4}`

Formats:
- `a$d$r$a $t$na`
  * Examples:
    - `a274811 260532a`: drawing 2748, region Japan, account 1, title 26, serial number 0532
    - `a2793 13393143a`: drawing 2793, region Japan, account 3, title 39, serial number 3143

Unknowns:
- System 256 dongle (memory card): `a 026161 351019 a`

## Net ID

Components:
- `$x`: unknown, `[A-Z]`
  * `D`:
  * `E`:
  * `G`:
- `$a`: account code, `[0-9]`
- `$t`: title code, `[0-9]{2}`
- `$n`: serial number, `[0-9]{4}`

Formats:
- `AB$xN-$a$t$n`
  * Examples:
    - `ABGN-1260532`: unknown G, account 1, title 26, serial number 0532
    - `ABEN-3393143`: unknown E, account 3, title 39, serial number 3143
