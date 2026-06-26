# Image Asset Audit

Date: 2026-06-26

## Map

- `src/assets/images/map/emberwreath-map.webp` is present.

## Species

Expected pattern per species folder: one routine image, two class images using `{species}-class-{class}.webp`, and one reference image.

| Species folder | Found website-ready files | Count | Convention status |
| --- | --- | ---: | --- |
| `humans` | `human-routine.webp`, `human-class-monk.webp`, `human-class-thief.webp`, `human-reference.webp` | 4 | Folder has 4 assets, but filenames use `human` while the audited folder/species key is `humans`. |
| `zivari` | `zivari-routine.webp`, `zivari-bard.webp`, `zivari-ranger.webp`, `zivari-refernce.webp` | 4 | Folder has 4 assets, but class files are missing `class-` and reference is misspelled. |
| `veyr` | `veyr-routine.webp`, `veyr-class-paladin.webp`, `veyr-class-wizard.webp`, `veyr-reference.webp` | 4 | Matches convention. |
| `ferren` | `ferren-routine.webp`, `ferren-class-cleric.webp`, `ferren-class-paladin.webp`, `ferren-reference.webp` | 4 | Matches convention. |
| `aumari` | `aumari-routine.webp`, `aumari-class-druid.webp`, `aumari-class-monk.webp`, `aumari-reference.webp` | 4 | Matches convention. |
| `axali` | `axali-routine.webp`, `axali-class-fighter.webp`, `axali-class-sorcerer.webp`, `axali-reference.webp` | 4 | Matches convention. |
| `scolen` | `scolen-routine.webp`, `scolen-class-ranger.webp`, `scolen-class-thief.webp`, `scolen-reference.webp` | 4 | Matches convention. |
| `kelden` | `kelden-routine.webp`, `kelden-class-barbarian.webp`, `kelden-class-druid.webp`, `kelden-reference.webp` | 4 | Matches convention. |
| `thryss` | `thryss-routine.webp`, `thryss-class-bard.webp`, `thryss-class-fighter.webp`, `thryss-reference.webp` | 4 | Matches convention. |

## Islands

Island folders are present under `src/assets/images/islands/`. Each audited folder contains a `.gitkeep` plus one `.webp` image named after the island or region, not `{island}-hero.webp`. Missing `{island}-hero.webp` files are informational only because island hero images are not expected yet.

Current island image folders: `ashspine`, `breadbasket`, `breakwater`, `caelmere`, `cinderreach`, `frozenfang`, `greenwood`, `hollowdeep`, `rainwall`, `redwind`, `reedmere`, `saffra`, `stormhook`, `sunspire`, `tidefall-atolls`, `veiled-reefs`, `veilgarden`, `verdurain`, and `western-forbidden-caldera-sea`.

## Documentation alignment

`IMAGE-NAMING.md` documents lowercase kebab-case `.webp` assets, map filename `emberwreath-map.webp`, species assets as routine, two class images, and reference, plus future island hero names as `{island}-hero.webp`.

Current alignment issues:

- `src/assets/images/species/humans/` uses `human-*` file stems rather than `humans-*` if the folder name is treated as the species key.
- `src/assets/images/species/zivari/zivari-bard.webp` and `src/assets/images/species/zivari/zivari-ranger.webp` do not include `class-`.
- `src/assets/images/species/zivari/zivari-refernce.webp` appears to be a misspelling of `zivari-reference.webp`.
- Island `.webp` files currently use `{island}.webp`, while the documented future convention is `{island}-hero.webp`.
