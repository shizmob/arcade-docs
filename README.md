# arcade documentation

An open (to read and contribute) repository of arcade hardware and software documentation.

## Scope

This repository aims to document both arcade hardware and software to the extent that it's necessary and useful.
This is not a hard and fast rule: listing every single software revision changes for every game may be out of scope and quickly bloat the repository,
but full PCB descriptions and pinouts may be useful for repair.

There's no hard boundary or ruleset yet, but please keep in mind whether the you're not directly duplicating another source's effort
(for instance, Bemaniwiki is pretty good at documenting Konami software changes).
If you're unsure, just send in a pull request and we'll see what we can work out!

Note that we won't accept copyrighted materials or anything that could get us into trouble:
(self-made) pictures are fine, but please don't contribute manuals or similar copyrighted content.
They're extremely useful, but due to DMCA limitations this is sadly not the place for them.

Finally, this is not the place for contents that directly and solely help bootleggers:
while security details for arcade systems are useful and important for preservation,
consider the age of the system and whether it is still under active support from its manufacturer or distributor first,
as well as whether parts of that security system are still relevant for newer, more current, systems.

## Sources

Due to the origin of this repository, there is almost no information of the sources of the information contained within it right now.
**We're fairly certain on the accuracy of most of it, however do not take it as gospel and *always* measure before working on hardware!
You are *solely* responsible for working on your own, and especially other peoples', cabinets.**

A source tagging system is in the works, the preliminary version consists of adding the following information at the end of a line:

`#<type>:<info*>`

Types can be:
* `WEB`: website, info identifies the website in question
* `SCRAPE`: scrape, info identiies the source of the scrape
* `GAME`: game data, info identifies the data and location
* `MAME`: MAME sources, info identifies the driver filename
* `DOC`: official documentation, info identifies the producer and identifier of the document

Examples:
* `#WEB:http://kururusky.com/?p=1458`, a website source;
* `#SCRAPE:sega:arcade-history`, a scrape source (SEGA's [arcade history](https://sega.jp/history/arcade) page);
* `#GAME:namco:PBN100-1-NA-MPRO-A:AMCUS/AMConfig.ini`, a game data source (`AMConfig.ini` in Pokemon Battle Network);
* `#MAME:namcops2`: a MAME source (the `namcops2.cpp` driver comments);
* `#DOC:konami:114946810000`, an official document source: the KONAMI beatmania IIDX 23 tricoro cabinet manual (doc #114946810000);

In the meantime here are some major sources used:

* First-hand accounts, observations and research of hardware and software;
* Manuals and other official documentation;
* Photos from various sites, most notably [Yahoo! Auctions / ヤフオク!](https://auctions.yahoo.co.jp/) and [eBay](https://ebay.com);
* Direct conversations with trusted sources;
* [MAME](https://git.redump.net/mame/)'s inimitable documentation;
* [BEMANIWiki 2nd](bemaniwiki.com/);
* [Callus Next's arcade board game information](http://callusnext.com/pcbs/);
* [Guru's rom dumping news](https://members.iinet.net.au/~lantra9jp1_nbn/gurudumps/);
* The [Redump database](http://redump.org/);
* Direct conversations with other sources;

Notable sources that are often incorrect and should not be solely relied upon:

* [System16](https://www.system16.com/);
* [Wikipedia](https://en.wikipedia.org) (yes, Japanese Wikipedia too!) and its million scrapers, clones and mirrors;


## License

The contents herein, insofar they are original and copyrightable, are licensed under the following license:

```
            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

 Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.
```

By contributing, you agree that your contributions will be licensed under the WTFPL as well.
