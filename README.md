# Next Turn map tiles

Offline road-map tiles for the **Next Turn** iPhone app (an audio rally co-driver for everyday
roads), covering **Great Britain, Northern Ireland and Malta**. Rebuilt regularly from
OpenStreetMap extracts; each [release](../../releases) holds one build.

## Contents of a release

- `index.json`: the format (`NTMAP1`), the engine version, when it was built, the OpenStreetMap
  data date, and for every 0.1° tile (named by its south-west corner, e.g. `51.5,-0.1`) the pack
  file, byte offset and length.
- `p_<south>_<west>.bin`: the gzipped tiles of one 1° square, one after another. Each tile is a
  gzipped JSON road network (drivable roads split at junctions, and named places).

## Licence

© OpenStreetMap contributors. This data is made available under the
[Open Database Licence (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).
Any rights in individual contents of the database are licensed under the
[Database Contents Licence](https://opendatacommons.org/licenses/dbcl/1-0/).
See [openstreetmap.org/copyright](https://www.openstreetmap.org/copyright).

Source extracts: [Geofabrik](https://download.geofabrik.de/) (openstreetmap.fr as a mirror).
