# arcade documentation

An open (to read and contribute) repository of arcade hardware and software documentation,
started from consolidating the various text files on my drives.

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
We're fairly certain on the accuracy of most of it, however do not take it as gospel and always measure before working on hardware!

A source tagging system is in the works, the preliminary version consists of adding the following information at the end of a line:

`#<type>:<info*>`

Types can be:
* `WEB`: website, info identifies the website in question
* `SCRAPE`: scrape, info identiies the source of the scrape
* `GAME`: game data, info identifies the data and location
* `MAME`: MAME sources, info identifies the driver filename
* `DOC`: official documentation, info identifies the producer and identifier of the document

Examples:
* `#WEB:http://kururusky.com/?p=1458`, a website source
* `#DOC:KONAMI:114946810000`, an official document source: the KONAMI beatmania IIDX 23 tricoro cabinet manua

In the meantime here are some major sources used:

* First-hand accounts, observations and research;
* Manuals and other official documentation;
* Photos from various sites, most notably [Yahoo! Auctions / ヤフオク!](https://auctions.yahoo.co.jp/) and [eBay](https://ebay.com);
* Direct conversations with trusted sources;
* [MAME](https://git.redump.net/mame/)'s inimitable documentation;
* [Callus Next's arcade board game information](http://callusnext.com/pcbs/);
* [Guru's rom dumping news](https://members.iinet.net.au/~lantra9jp1_nbn/gurudumps/);
* The [Redump database](http://redump.org/);
* Direct conversations with other sources;

Notable sources that are often incorrect and should not be solely relied upon:

* [System16](https://www.system16.com/)
* [Wikipedia](https://en.wikipedia.org) (yes, Japanese Wikipedia too!) and its million scrapers, clones and mirrors
