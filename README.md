# CONUS Canopy Height — 3D blocks

Interactive Three.js visualization of continental-US forest canopy height as extruded voxel columns.

**Live:** https://evanapplegate.github.io/canopy_height_blocks

## Data
- **Source:** NASA GEDI L3 gridded canopy height (rh100 mean), 2019–2022, native 1 km, via [OpenTopography](https://portal.opentopography.org/).
- Resampled to ~3 km cells and clipped to the Natural Earth 50m US land polygon with the Great Lakes removed.
- ~906k land columns, aggregated on the fly into half / quarter / 1/8-res "big block" views.

## Features
- Four resolution tabs (1/8 → full).
- Perspective / orthographic projection.
- Sun azimuth / elevation / intensity, ambient, height exaggeration, color saturation — each with a slider + number entry.
- Cast shadows (cached shadow maps).
- Export current view as a 4K transparent PNG.

Everything is self-contained: `index.html` + `conus_ch_data.js` (the packed grid). Three.js loads from a CDN.
