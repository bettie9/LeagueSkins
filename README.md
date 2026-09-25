<h1 align="center">LeagueSkins</h1>

<p align="center">Skins, chromas, emotes and wards for League of Legends and League Classic.</p>

<p align="center">
  The package library behind <a href="https://github.com/bettie9/Sunshine"><strong>Sunshine</strong></a>.
</p>

<p align="center">
  <a href="https://github.com/bettie9/Sunshine/releases/latest"><strong>Download Sunshine</strong></a> ·
  <a href="#browse-the-library">Browse packages</a> ·
  <a href="classic/README.md">Classic guide</a> ·
  <a href="https://discord.gg/8zsgZUxVgW">Discord</a>
</p>

## Browse the library

Download individual `.fantome` packages here, or browse and install them directly in Sunshine.

| Collection | Packages | Coverage | Catalog |
| --- | ---: | --- | --- |
| [Champion skins](skins/) | 9,688 | Skins, chromas and forms for 173 normal LoL champions | [index.json](index.json) |
| [League Classic](classic/) | 1,716 | Skins, chromas and variants for 72 Classic champions | [classic/index.json](classic/index.json) |
| [Emotes](emotes/) | 2,057 | Replacements for the default thumbs-up emote | [emotes-index.json](emotes-index.json) |
| [Wards / Totems](wards/) | 265 | Replacements for default ward and trinket appearances | [wards-index.json](wards-index.json) |

*Library snapshot: September 25, 2026. Normal skin catalog: 16.19.1. Classic catalog: 16.19. Counts include individual variants; older duplicate download names are excluded.*

**Choose the collection for your game mode.** Packages in `skins/` target normal LoL champions. Packages in `classic/` target the `Jade_*` champions used by League Classic; they do not turn normal LoL champions into their Classic versions.

## Use with Sunshine

1. Install [Sunshine](https://github.com/bettie9/Sunshine/releases/latest) and configure your League installation in **Settings → Game setup**.
2. Open **Skin Changer**, choose **Skins**, **Classic**, **Emotes** or **Totems**, then browse and install your selection.
3. Enable your packages and use **Apply & Inject** before starting the game.

Sunshine **0.13.1 and later** uses this repository and **LTK Patcher** automatically. The **Classic** tab requires Sunshine **0.13.0 or later**.

For normal champion skins, select the champion's **default skin** in League. Emote packages replace the **default thumbs-up emote**; equip it in your emote wheel. Enable one replacement per champion, one emote and one ward package at a time to avoid conflicting overrides.

Kayle skins and chromas evolve with levels, Kayn follows his in-game transformation, and Spirit Guard Udyr retains its stance progression. Pulsefire Ezreal changes appearance when R is ranked up. Separate Stage/Form downloads keep the selected appearance. Immortalized Tristana Stage 3 also supports **Ctrl+5** mask switching.

The main **DJ Sona** package includes DJ music and **Ctrl+5** form/music switching, including while moving. Enable music in League's audio settings to hear the soundtrack.

## Download a package manually

1. Open the collection above and find the `.fantome` file you want.
2. Open the file on GitHub and choose **Download raw file**.
3. Import the downloaded `.fantome` into Sunshine or a mod manager that supports the format, such as LTK Manager.
4. Enable it using a patcher compatible with your installed game version.

You only need the packages you want; downloading or cloning the entire repository is unnecessary for installation. Leave the `.fantome` file intact when importing it.

Examples: [Dynasty Ahri for normal LoL](skins/Ahri/Dynasty%20Ahri.fantome) · [Dynasty Ahri for League Classic](classic/Jade_Ahri/60103001.fantome).

## Compatibility and updates

- Game patches can change assets, hashes and dependencies. Check the catalog's patch and [recent commits](https://github.com/bettie9/LeagueSkins/commits/main/) when troubleshooting; rebuilds may arrive after the game update.
- A successful download or import does not guarantee that every model, animation or effect works in game. Test a new package in a practice or custom game for the intended mode.
- Package compatibility and patcher compatibility are separate. An older patcher is not a guaranteed fix for a broken package.
- Classic packages have their own targets and validation notes. Read the [Classic guide](classic/README.md) before using them outside Sunshine's Classic browser.

## Report a problem

[Report a broken package or request a missing skin/form](https://github.com/bettie9/LeagueSkins/issues/new/choose), or join [Discord](https://discord.gg/8zsgZUxVgW). The issue forms ask for the package, game version and a short description. Screenshots or a short clip help with visual problems.

For problems with Sunshine itself, use the [Sunshine issue tracker](https://github.com/bettie9/Sunshine/issues). You can export support logs from **Settings → Support → Save support logs**; review them before sharing.

<details>
<summary><strong>Repository layout and catalogs</strong></summary>

```text
skins/<champion>/<skin>.fantome
skins/<champion>/<base skin>/<chroma or form>.fantome
classic/<Jade champion>/<full skin id>.fantome
emotes/<emote>.fantome
wards/<ward>.fantome
```

The regular catalog groups skins, chromas and forms by champion. Emote and ward catalogs provide each package's filename.

The Classic catalog includes champion identities, target slots, artwork, parent-skin relationships and package SHA-256 hashes. Its package `path` values are relative to `classic/`.

Use the catalogs when resolving downloads: display names can contain punctuation or differ from filenames. URL-encode path segments when constructing raw download URLs.

</details>

## Credits

- [Sunshine](https://github.com/bettie9/Sunshine) — package builds and app integration.
- [CommunityDragon](https://communitydragon.org) — catalogs, artwork references and asset hash data.
- [LtMAO](https://github.com/tarngaina/LtMAO) and [ritobin](https://github.com/moonshadow565/ritobin) — tooling used by the skin-building pipeline.

---

LeagueSkins is an independent project and is not affiliated with or endorsed by Riot Games. League of Legends, its characters and game assets belong to Riot Games. Cosmetic changes are local to your client.
