# Garden model

An editable 3D model of the garden, which runs in any web browser with nothing to install.

- **Seasons:** a month slider changes the leaf colour, blossom, fruit and bare winter branches.
- **Growth:** a 0–30 year slider grows each plant towards its typical mature height and spread.
- **Light:** the sun position is calculated for the site and date, with shadows. There are presets from sunrise to dusk, and a sun-hours map shows full sun, part shade and shade.
- **Editing:** add, move and resize plants, trees, walls, fences, hedges, paths, patios, water features, pergolas, sheds and greenhouses.
- **Realistic mode:** leaf-by-leaf foliage, a physically based sky, textured surfaces and soft shadows. Turn it off on slower devices.
- **Versions:** save named versions of the plan and switch between them.

## Viewing

Open the GitHub Pages site for this repository, or open `index.html` directly in a browser. An internet connection is needed: the 3D engine (three.js r128) and fonts load from public CDNs.

## Where changes are saved

The site is static, so edits and saved versions are kept in the visitor's own browser (`localStorage`). They don't change this repository and aren't seen by anyone else. **Save → Reset to the shared plan** goes back to the plan published here. To keep a copy of a plan elsewhere, use **Save → Copy plan**.

## Updating the published plan

The published plan is the JSON inside the `<script id="plan-data">` tag in `index.html`. To publish changes:

1. Make the changes in the page, then use **Save → Copy plan**.
2. Replace the `plan` value inside `plan-data` with the copied text, and commit.

Shared options for visitors to compare go in the same block as a `versions` array: `[{"id": "...", "name": "Option A", "at": "2026-11-12T00:00:00Z", "plan": {...}}]`.

## Accuracy

The plot boundary was traced from the title plan at 1:1250, which shows the general line of the boundary rather than its exact position. The house comes from the floorplan. Existing trees, beds and outbuildings were placed from photographs and are approximate. Plant growth uses typical sizes and rates. Sun hours are for the 15th of each month, at ground level.
