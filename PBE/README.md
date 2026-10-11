# PBE skins for live League

Five skins and 28 chromas from PBE 16.21, packaged for live **16.20.824.8524**.
All 33 packages were reported tested and working by the maintainer on October 11, 2026.
League Classic / Jade Karma is excluded.

| Skin | Main package | Chromas |
| --- | ---: | ---: |
| [True Damage Know My Name Akali](Akali/True%20Damage%20Know%20My%20Name%20Akali.fantome) | 15.49 MB | [6](Akali/True%20Damage%20Know%20My%20Name%20Akali/) |
| [Prestige True Damage Know My Name Ekko](Ekko/Prestige%20True%20Damage%20Know%20My%20Name%20Ekko.fantome) | 14.10 MB | [1](Ekko/Prestige%20True%20Damage%20Know%20My%20Name%20Ekko/) |
| [True Damage Know My Name Qiyana](Qiyana/True%20Damage%20Know%20My%20Name%20Qiyana.fantome) | 12.11 MB | [8](Qiyana/True%20Damage%20Know%20My%20Name%20Qiyana/) |
| [True Damage Know My Name Senna](Senna/True%20Damage%20Know%20My%20Name%20Senna.fantome) | 15.71 MB | [8](Senna/True%20Damage%20Know%20My%20Name%20Senna/) |
| [True Damage Know My Name Yasuo](Yasuo/True%20Damage%20Know%20My%20Name%20Yasuo.fantome) | 11.95 MB | [5](Yasuo/True%20Damage%20Know%20My%20Name%20Yasuo/) |

## Use

1. Download the individual `.fantome` using **Download raw file**, then import it into Sunshine.
2. Enable **one PBE package at a time**, including across champions. These packages include different private shader tables and can overwrite each other's additions.
3. Select the champion's **default skin** in League.

Every chroma is standalone; do not enable its main skin package alongside it.
You do not need a PBE installation. Covers use the official skin splash art;
chromas share their parent skin's cover and identify their color in the name.

The files target the game version above. Recheck compatibility after a League update.
The regular Sunshine catalog does not automatically list this separate PBE collection;
import these files manually.

## Validation and source

Archive integrity, package identity, file dependencies, BIN hashes and shader programs
were checked for all 33 packages. Separate LTK overlay checks passed for the five main
skins and Ekko Vivid. Runtime acceptance is the maintainer's report; no per-ability
checklist was recorded. Embedded build metadata describes checks at build time and
may predate that runtime acceptance.

Ekko's optimized package is 14.10 MB (19.72% smaller), with all 377 decoded game
payloads identical to its previously accepted package. No texture, animation or
shader data was removed for that size reduction.

[Index and checksums](index.json) · [SHA-256 file list](SHA256SUMS.txt)

Game assets were read from Riot's official CDN using [CDTB](https://github.com/CommunityDragon/CDTB).
The pinned source manifest is [252D54B2713A1DBA](https://lol.secure.dyn.riotcdn.net/channels/public/releases/252D54B2713A1DBA.manifest).
Artwork and game assets belong to Riot Games.
