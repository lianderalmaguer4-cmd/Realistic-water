# Changes from Realistic Water 1.2.4 (by Skaffy)

Original: https://github.com/sskaffy/Realistic-Water

- Added `WaterPresets` and the `/water preset low|balanced|high` command (op only, like the other /water commands).
  - low: resolution 4, 2 substeps, 3 solver iterations, 8 coarse sweeps, surface subdivision 1, whitewater off,
    sand resolution 8 / 8 substeps / 16 grains, 100 leaves per block.
  - balanced: resolution 5, 3 substeps, 4 solver iterations, 10 coarse sweeps, sand resolution 10 / 12 substeps / 24 grains, 150 leaves per block.
  - high: the original defaults.
- `Vk.closeQuietly`, `WaterRenderer.close`, `PressureSolver.close`, `SurfaceMesher.close`: failures when closing resources are logged at debug level instead of being ignored.
- Fork metadata: name, description, authors and links in `fabric.mod.json`; version `1.2.4-opt.1`.

Not changed: simulation, rendering, physics, networking and every other file.
Not verified: no compilation or in-game test was possible when these edits were made.
