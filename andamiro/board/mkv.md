# MKV

AKA MK5

* OS
  * Windows XP Embedded: revisions of [The Premiere 3](game/piu/prem3.md) and [The PREX 3](game/piu/prex3.md)
  * Linux: starting [Exceed](game/piu/exc.md)
* [PIUIO](io.md#MK5IO) connected to the ISA bus
* CPU
  * Intel Celeron 1 GHZ
  * Intel Celeron 1.3 GHZ
* RAM: 128 MB
* GPU (on-board)
  * Riva TNT 2, 32 MB
  * 
* Chipset
  * Nvidia NV11
  * VIA Apollo Pro133 AX (VT82C694X + VIA686B)
* BIOS
  * PhoenixBIOS 4.0 Release 6.0 
* Disk media
  * CDROM based for [The Premiere 3](game/piu/prem3.md) and [The PREX 3](game/piu/prex3.md)
  * DVD based for [Exceed](game/piu/exc.md) beta
  * HDD based for [Exceed](game/piu/exc.md) release and newer
* 7 segment display on the side shows current boot status/error codes
* EEPROM to store game settings and high scores. Size increased (doubled?) compared to [MK3](#mk-3)

## 7 segment status and error codes

This display next to the mainboard breakout connectors shows an 8-bit hex value indicating
different stages of the boot process and errors.

Errors are usually "stuck values". A healthy boot sequence has these numbers changing to show
it progresses through the different stages.

### Healthy boot sequence

The following is "transcribed" from a video recording of a healthy boot sequence (from power on
to game title screen). All values are 8-bit hex values.

* `FF`: Initial state shown right after power on
* `81`: ???
* `84`: ???
* `85`: ???
* `86`: ???
* `87`: ???
* `88`: ???
* `08`: ???
* `11`: ???
* `0C`: ???
* `28`: ???
* `2E`: ???
* `38`: ???
* `09`: ???
* `69`: ???
* `49`: ???
* `4A`: ???
* `59`: ???
* `52`: ???
* `60`: Video output over VGA shows the Andamiro logo on white background, the first actual video output
  visible
* `98`: ???
* `6A`: ???
* `00`: ???
* `01`: ???
* `C0`: ???
* `D2`: ???
* `00`-`99`/`00`: Progress counting upwards from 0 (`00`) to 100 (`00`)
* `FF`: ???
* `88`: ???
* `FF`: ???
* `88`: ???
* `A2`: booted from HDD, starting with Andamiro MKV bootloader stage and also stays when in-game

### Operating system/game booted

Once the display shows `A2`, it's also flickering.

The bottom segment of the first digit as well as the top left and bottom right segments of the
second digit are used as HDD, CPU and ??? indicators.

### Other codes

* `01`: In BIOS menu

### Errors

#### Stuck at FF right after power on

If the BIOS isn't loading, then it is stuck right after power on.

This might indicate that something is wrong with the power to the mainboard. Ensure you are using
the power distribution board of the MKV box and not have a ATX power supply connected directly to
the mainboard. It powers, but doesn't seem to like that and stays stuck here immediately.

#### Stuck at C0

Operating system not found.

This should also be visible on over VGA output with a message stating this on a connected screen.

#### Stuck on B0

CMOS checksum bad.

This should also be visible on over VGA output with a message stating this on a connected screen.

Probably the CMOS battery is empty, swap it, power cycle. Defaults are being loaded automatically.

## Misc

* USB keyboards work, e.g. to get into the BIOS by pressing F2 during boot
