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

## Latest skin update

Missing ability screen effects have been restored for Immortalized Tristana
and Ahri, Space Groove Teemo, T1 Yunara, Eclipse Eternal Aspect Diana and
Soul Fighter Samira. Re-download the affected packages to get these fixes.

Additional forms, weapon choices and level appearances are now available,
including matching chromas. Find them inside each skin's folder and choose
the appearance you want.

Immortalized Tristana, Ahri and Kai'Sa now have the correct **Stage 2**
appearance and separate **Stage 3** packages. Browse
[Tristana's forms](skins/Tristana/Risen%20Legend%20Tristana/),
[Ahri's forms](skins/Ahri/Risen%20Legend%20Ahri/) or
[Kai'Sa's forms](skins/Kaisa/Risen%20Legend%20Kai'Sa/).

The regular skin library has been rebuilt with fixes for MVP T1 Miss Fortune,
Super Galaxy Rumble, Sunken Shadows Lucian, Revenant Reign Viego, Heartseeker
Jinx, Infernal Nasus and Arcade Hecarim.

Viego's upgraded forms are available from spawn and switch with **Ctrl+5**;
automatic possession-based selection is not supported. Arcade Hecarim's R
rider colors can repeat or appear in a different order from the original.

Want to build your own packages? Use [League Skin Fantome Builder](https://github.com/bettie9/league-skin-fantome-builder).

## Use with Sunshine

1. Install [Sunshine](https://github.com/bettie9/Sunshine/releases/latest) and configure your League installation in **Settings → Game setup**.
2. Select **Sunshine** under **Skin source** to prefer this repository for regular skins.
3. Open **Skin Changer**, choose **Skins**, **Classic**, **Emotes** or **Totems**, then browse and install your selection.
4. Enable your packages and use **Apply & Inject** before starting the game. Sunshine uses **LTK Patcher** by default.

The **Classic** tab requires Sunshine **0.13.0 or later**. Classic packages, emotes and wards always download from this repository, independently of the preferred source for regular skins.

For normal champion skins, select the champion's **default skin** in League. Emote packages replace the **default thumbs-up emote**; equip it in your emote wheel. Enable one replacement per champion, one emote and one ward package at a time to avoid conflicting overrides.

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

[Open a package issue](https://github.com/bettie9/LeagueSkins/issues/new) or join [Discord](https://discord.gg/8zsgZUxVgW). Include:

- The package's repository link and the affected skin or chroma.
- Your League patch and whether you are playing normal LoL or League Classic.
- Your mod manager version and injection method.
- What happened: import failure, unchanged appearance, missing effects or a crash, plus any steps that reproduce it.

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
