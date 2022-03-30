# GEC02-PWB(A)A

* aka "C02 IO" board
* GEC02-PWB(A)A
* PCB product: PN0000228708
* case/metal housing: PN0000246977
* case/box cover: PN0000246978
* Interface to main PCB: USB 1.1
* Compatible games: [C02](../software/C02.md), [D01](../software/D01.md), [E11](../software/E11.md),
[ECO](../software/ECO.md), [FDD](../software/FDD.md), [GLD](../software/GLD.md), [HDD](../software/HDD.md),
[I00](../software/I00.md), [JDJ](../software/JDJ.md), [JDZ](../software/JDZ.md), [KDZ](../software/KDZ.md),
[LDJ (only up to 24 included)](../software/LDJ.md)

## C02/D01 IO RJ45 to DIN8 connector pinout

This was created by using the [BIO2 sub IO board](../io.md#bio2-ldj-sub-io) to connect pre IIDX 25 cabinet
hardware to the [BIO2 IO board](../io.md#bio2). The two connector types from different generation IO boards, RJ45
on the [C02 IO](#c02-io) board and a round DIN8 connector on the [USBIO2](../io.md#usbio2) board are just
different connectors to the same hardware on the BIO2 sub IO board.

Therefore, any C02/D01 wired cabinet can be upgraded to IO2 wiring and vice versa by building
a RJ45 -> DIN8 or DIN8 -> RJ45 adapter cable.

The following connection information was traced on a original Konami BIO2 sub IO board.

RJ45 (female) connector, top view:

```text
plug insert
     |
     |
     v
|-----------|
|  Top view |
|           |
|   Pins    |    
|   7 5 3 1 |
|  8 6 4 2  |
|-----------|
```

DIN8 (female) connector, top view:

```text
plug insert
     |
     |
     v
|-----------|
|  Top view |
|   Pins    |    
|  3  1 2 6 |
| 7 4 5 8 9 |
|-----------|
```

The two connectors are interconnected on the PCB like this:

| RJ45 pins | DIN8 pins |
|-----------|-----------|
| 1         | 1         |
| 2         | 7         |
| 3         | 4         |
| 4         | 6         |
| 5         | 5         |
| 6         | 3         |
| 7         | 2         |
| 8         | 1         |
