# Monster Hunter Wilds mods — public releases

Release downloads and the Custom Mod Manager catalog for the REFramework mods by maydie13.
The source is developed privately; every release here is the exact archive that passed in-game
QA, copied byte-for-byte, with its checksums and a provenance file.

| Mod | Nexus page | What it does |
| --- | --- | --- |
| RNG Charm Crafting | https://www.nexusmods.com/monsterhunterwilds/mods/4900 | Craft the talisman you want from melding tickets through the game's own menus |
| Decoration QoL | https://www.nexusmods.com/monsterhunterwilds/mods/4954 | Six direct decoration melding lists, editable prices, better orb odds |
| Artian QoL | https://www.nexusmods.com/monsterhunterwilds/mods/4855 | Separate stat and skill rerolls for Artian and Gogma weapons |

All releases target Monster Hunter Wilds **1.42.0.2** (Steam build 24705561) with REFramework
nightly `88ece6b`. Later title updates are not supported until a release says so.

## Installing

Download the ZIP from the release's assets and import it into Fluffy Mod Manager as is, or
unpack `reframework/` (and `natives/` where present) into the game folder. Manual installs of
mods with a `natives/` folder need **Enable Loose File Loader** ticked in the REFramework menu.
Check the download against `SHA256SUMS.txt`. Each archive contains its own README.

## Custom Mod Manager

`cmm-repository.json` is the entry point for the Custom Mod Manager repository source; it points
to the current `v5/repository-catalog.json`. The catalog lists each release's archive size and
SHA-256, so the manager verifies every download against the accepted bytes before installing.

## Release layout

- Tag `<package-id>-v<version>`, for example `rng-charm-crafting-v2.0.3`.
- Assets: the accepted ZIP, `SHA256SUMS.txt`, `release-provenance.json` (source commit, producer
  manifest path, asset hashes).
- Published releases are never edited; a correction ships as a higher version.

Private-use mods by the same author are not published here.
