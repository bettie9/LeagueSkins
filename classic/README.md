# League Classic

[← Back to LeagueSkins](../README.md)

**72 champions · 1,716 skins, chromas and variants · Patch 16.19**

These packages apply skins to the `Jade_*` champions in **League Classic**. They are built from the installed game's Classic assets.

**They are not Classic appearance mods for normal LoL champions.** For regular LoL, use the [normal skin library](../skins/).

## Install

In **Sunshine 0.13.0 or later**, open **Skin Changer → Classic → Browse Classic Skins**. Install your selection, enable it and use **Apply & Inject** with LTK.

For a manual download, open a champion folder, choose a `.fantome` file and use **Download raw file**. Import it into your mod manager without extracting it. The [catalog](index.json) maps each numeric filename to its skin name.

Enable **one package per champion**. Disable other normal or Classic packages for the same champion before testing, since they can modify the same WAD archive. Start a League Classic game with the corresponding Classic champion.

## Find a skin

Packages use this layout:

```text
classic/<Jade champion>/<full Jade skin id>.fantome
```

For example, [Dynasty Ahri](Jade_Ahri/60103001.fantome) targets **Jade_Ahri**, whose champion ID is `60103`. Its skin ID is `60103001`.

[index.json](index.json) contains:

- Champion IDs, names and their normal LoL counterparts.
- Skin names, chroma relationships and artwork URLs.
- Package paths relative to `classic/`, plus SHA-256 hashes.
- The destination skin slots covered for each champion.

Packages target slot `0` and the available `300`–`399` Classic slots recorded in the catalog. This covers Classic selections that load a slot other than the normal default slot.

## Validation and limitations

For the 16.19 catalog:

- All 1,716 packages passed BIN/WAD structural, dependency and byte-preservation checks.
- One package per champion passed a combined **72-WAD build with LTK Overlay 0.9.5**, with no missing linked BINs or checksum mismatches.
- **Dynasty Ahri** and **Annie-Versary** trial packages were confirmed working in game. This is not an in-game verification of every published skin or chroma.

Some pets or alternate forms have no matching per-skin asset. Those packages use the available parent-skin or base-form asset. Twisted Fate slot 35 has no public catalog name and is listed as **Twisted Fate (Variant 35)**.

New game patches may require updated packages. Test the model, movement, attacks, abilities and recall in a League Classic custom game before relying on a package.

## Report an issue

Include the exact package link, League patch, mod manager and injection method, and confirm that the test used a **League Classic champion**. Describe the affected appearance or ability, or when the crash occurred.

[Open an issue](https://github.com/bettie9/LeagueSkins/issues/new) · [Discord](https://discord.gg/8zsgZUxVgW)
