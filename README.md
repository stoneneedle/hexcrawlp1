# Hexcrawl Prototype 1

### By James Groth

This program is hoped to eventually have more features, but for now I'm just trying to build a hexagonal tilemap with HexagonTools ( https://github.com/mpalmerlee/HexagonTools ) that uses Perlin noise ( https://github.com/josephg/noisejs ) to generate terrain.

This still isn't accomplished yet. To get there, I think I need to:

1. Get the Perlin noise to do its thing, outputting a value of some kind that represents the elevation of the tile.
2. Assign each Perlin noise elevation value to a tile in the hex grid. Maybe I should even modify the HT.Hexagon objects so that each one always has a Perlin noise elevation value upon generation. Or maybe I should leave the basic hexagon tool alone, and apply the Perlin noise value to the output.
3. Generate JSON output representing a hexagonal tilemap with all the properties of the tilemap.
4. Draw the tilemap, with Perlin noise above a certain value being mountain tiles, within a range being plains tiles, and below a certain range coastal/ocean tiles.
