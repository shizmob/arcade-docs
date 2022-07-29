# Dancing Stage Fusion dedicated cabinet JAMMA edge wiring

The Dancing Stage Fusion dedicated cabinet has different wiring than
classic Dancing Stage/Dance Dance Revoluion Machines that are either based
on 573 analog/digital hardware or Python 2 hardware.

The cabinet connects to the main PCB using two JAMMA edge 28-pin connectors.

The following sub-sections provide full pinouts taken from a stock
Dancing Stage Fusion dedicated cabinet. `NC` denotes to "not connected".

## Pinout primary 28-pin connector

This 28-pin connector is actually following the JAMMA specification.

### Top side pinout

```text
 1: NC
 2: GND
 3: +5V
 4: +5V
 5: NC
 6: +12V
 7: NC
 8: NC
 9: NC
10: NC
11: NC
12: Video red
13: Video blue
14: Video GND
15: Test switch
16: Coin switch
17: P1 start
18: P1 up
19: P1 down
20: P1 left 
21: P1 right
22: NC
23: P1 left select
24: P1 right select
25: NC
26: NC
27: NC
28: GND
```

### Bottom side pinout

```text
 1: GND
 2: GND
 3: NC
 4: NC
 5: NC
 6: +12V
 7: NC
 8: NC
 9: NC
10: NC
11: NC
12: Video green
13: Video sync
14: Service switch
15: NC
16: NC
17: P2 start
18: P2 up
19: P2 down
20: P2 left
21: P2 right
22: NC
23: P2 select left
24: P2 select right
25: NC
26: NC
27: GND
28: GND
```

## Pinout secondary 28-pin connector

This 28-pin connector is the same as the primary connector but does not
follow the JAMMA pinout specification.

The follow hardware is connected on this connector:

* +5V power source
* Serial cable to EXT I/O
* Lights I/O cable to AMP box

### Top side pinout

```text
 1: NC
 2: NC
 3: +5V (red)
 4: NC
 5: Jumper cable (brown) -> Connects to bottom pin 6
 6: NC
 7: EXT I/O serial TX (purple)
 8: NC
 9: NC
10: NC
11: NC
12: NC
13: NC
14: NC
15: NC
16: NC
17: NC
18: NC
19: NC
20: NC
21: NC
22: NC
23: NC
24: Lights P2 cabinet button lights (yellow-grey)
25: Lights P1 halo up (light blue)
26: Lights P2 halo down (grey)
27: GND for +5V (black)
28: NC
```

### Bottom side pinout

```text
 1: NC
 2: NC
 3: NC
 4: NC
 5: NC
 6: Jumper cable (brown) -> Connects to top pin 5
 7: EXT I/O serial RX (grey)
 8: EXT I/O serial GND (black)
 9: NC
10: NC
11: NC
12: NC
13: NC
14: NC
15: NC
16: NC
17: NC
18: NC
19: NC
20: NC
21: NC
22: NC
23: Lights P1 cabinet button lights (purple-grey)
24: Lights P2 halo up (green)
25: Lights P1 halo down (purple)
26: Lights GND (black)
27: NC
28: NC
```

## Lights I/O connector

Lights I/O connector that goes into the AMP box.
Pintout order: looking at the front of the connector, left to right:

```text
|       |--|      |
|-----------------|
|1 2 3 4 5 6 7 8 9|
|-----------------|

1: Earth (yellow-green)
2: P2 halo down (grey)
3: P1 halo down (purple)
4: P1 halo up (light blue)
5: P2 halo up (green)
6: P2 cabinet button lights (yellow-grey)
7: P1 cabinet button lights (purple-grey)
8: NC
9: GND (black)
```

## EXT I/O serial connector

Serial connector going to the EXT I/O board.
Pintout order: looking at the front of the connector, left to right:

```text
|     |
|-----|
|1 2 3|
|-----|

1: GND (black)
2: TX (purple)
3: RX (grey)
```

## Adapter secondary JAMMA connector to "classic" DDR wiring

With the secondary JAMMA connector being propriatary to the Dancing
Stage Fusion cabinet, you need a "breakout" adapter that splices
the JAMMA connector into the following separate connectors:

* `EHR-5` connector to COM1 on the PCB for the EXTIO
* +5V supply, likely via a 2-pin connector that works with your
  cabinet's internal power infrastructure
* `XMP-11V` connector to PORT1 on the PCB for lights

Note: Bass lights, P1/P2 pad lights as well as sensor multiplexing
is handled by the EXTIO board.

### COM1 breakout

Pinout for the `EHR-5` connector breaking out of the JAMMA connector.

Pintout order for `EHR-5`: looking at the front of the connector,
left to right:

```text
|         |
|---------|
|1 2 3 4 5|
|---------|

1: GND (black)
2: NC
3: NC
4: RX (grey)
5: TX (purple)
```

Mapping for breakout cable:

```text
JAMMA top: 7     -> EHR-5: 5
JAMMA bottom: 7  -> EHR-5: 4
JAMMA bottom: 8  -> EHR-5: 1
```

### Lights connector breakout

Pinout for the `XMP-11V` connector breaking out of the JAMMA connector.

Pintout order for `XMP-11V`: looking at the front of the connector,
left to right:

```text
|          |--|         |
|-----------------------|
|1 2 3 4 5 6 7 8 9 10 11|
|-----------------------|

1: NC
2: P1 halo up
3: P1 halo down
4: P2 halo up
5: P2 halo down
6: GND
7: NC
8: NC
9: P2 cabinet button lights
10: P1 cabinet button lights
11: GND
```

Mapping for breakout cable:

```text
JAMMA top: 24     -> XMP-11V: 9
JAMMA top: 25     -> XMP-11V: 2
JAMMA top: 26     -> XMP-11V: 5
JAMMA bottom: 23  -> XMP-11V: 10
JAMMA bottom: 24  -> XMP-11V: 4
JAMMA bottom: 25  -> XMP-11V: 3
JAMMA bottom: 26  -> XMP-11V: 6 + 11
```
