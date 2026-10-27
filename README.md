# Survivor Incognito — Subnautica: Below Zero Atlas

An unofficial, interactive **2D atlas for Subnautica: Below Zero**, created for the Survivor Incognito website. Maps combine source-derived game terrain and biome classifications with separately sourced community location references.

**Status:** Public beta / review build. The atlas is useful as a reference, but **underground routes, cave clearances and some location coordinates have not been verified in-game**.

## Open the atlas

Open **`index.html`** in your browser, or visit the URL provided by GitHub Pages after the repository is published. The map images and other assets are embedded in the HTML, so no separate image folders or game data are needed to host the site.

## Main features

- Nine regions: Sector Zero, Glacial Basin, Arctic Spires, Twisty Bridges, Lily Pads / Tree Spires, Deep Purple Vents, Lilypads Crevice, Crystal Caves and Fabricator Caverns.
- Two views of the deep cave systems: **Simplified map** for a broad 2D view and **Source traces** for the original, denser voxel observations. These are different presentations of sampled geological evidence, **not confirmed navigation routes**.
- Terrain relief, game-derived biome classifications, optional biome labels, near-depth views and exact-depth horizontal voxel slices.
- **47 searchable reference locations**, including stations, wrecks, cave entrances and hidden story sites.
- Spoiler controls, selection cards, grouped markers on crowded screens and optional search limited to the current region.
- Copyable in-game-style **X, Y, Z coordinates**, a coordinate finder, mobile region switching, pinch-to-zoom and expanded map view.
- Reference panels for the cave systems and western land regions, including documented region-level connections without invented tunnel lines.

## Data sources and interpretation

- **`CompiledOctreesCache.zip`** supplied the voxel terrain sampled to create the relief and cave images.
- **`biomeMap.bin`** supplied the 1,024 × 1,024 grid of biome classifications, at approximately 4 m per map sample.
- **`biomes.csv`** supplied biome names.
- **Community map and coordinate references** supplied named location markers. These are separate from the original game-file terrain and can conflict or need correction.

The simplified cave view groups several depth samples into a more readable overview. Neither that view nor the detailed source traces establish continuous traversable passages. Rectangular unsurveyed areas reflect gaps in data coverage, not safe open water. In particular, Crystal Caves and Fabricator Caverns should not be treated as verified cave floorplans.

Some published location coordinates disagree, including the Crystal Caves Cache, Fabricator Base, Glacial Connection exit and Glacial Bay Bridge. The atlas flags uncertainty where known. The starting Drop Pod does not have one fixed location.

No external community map artwork is included; the relief, biome display and cave artwork are derived from the supplied files.

## GitHub Pages setup

1. Create a **public** repository, such as `subnautica-below-zero-atlas`.
2. Upload **`index.html`** and **`README.md`** to the top level of the repository, on the `main` branch.
3. Under **Settings → Pages**, choose **Deploy from a branch**, then select `main` and `/(root)`. Save.
4. Open the Pages URL displayed in the repository settings, then check region switching, map images, coordinates, spoiler controls and both cave-view modes on your phone.
5. To use a custom subdomain, configure it under GitHub Pages and create the corresponding DNS CNAME record with your DNS provider. Wait for DNS verification and HTTPS provisioning before announcing the final address.

## Limitations and feedback

This is an unofficial fan project and is not affiliated with Unknown Worlds. The maps are an exploration aid, not a guarantee of safe routes or correct depth readings. Please verify disputed coordinates or cave passages in-game before relying on them. Corrections are welcome through the repository's GitHub Issues page once enabled.

## Reference reading

- [Unknown Worlds: Terrain data format](https://unknownworlds.com/en/news/terrain-data-format)
- [Subnautica Wiki: Sector Zero Map](https://subnautica.fandom.com/wiki/Sector_Zero_Map)
- [Subnautica Wiki: Crystal Caves](https://subnautica.fandom.com/wiki/Crystal_Caves)
- [Subnautica Wiki: Fabricator Caverns](https://subnautica.fandom.com/wiki/Fabricator_Caverns)
