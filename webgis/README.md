# EO4DES WebGIS XYZ package

Raster GeoTIFFs converted to static Web Mercator XYZ tiles for GitHub Pages.

- XYZ CRS: EPSG:3857
- Tile size: 256 px
- Zoom levels: 10–15
- NoData: transparent
- LST visualization: 38–58 °C
- Thermal anomaly visualization: -20–+9 °C

Exact WGS84 extent:
- west: 18.032132580655
- south: 40.307150786973
- east: 18.313748210356
- north: 40.507855658669

The included `index.html` already uses:
- `Cesium.createWorldTerrain()`
- `data/lst/{z}/{x}/{y}.png`
- `data/thermal_anomaly/{z}/{x}/{y}.png`

Add/reproject these separately to EPSG:4326:
- `data/regioni.geojson`
- `data/statistiche_zonali_lecce.geojson`


## GeoJSON included

- `data/regioni.geojson`: 20 features
- `data/statistiche_zonali_lecce.geojson`: 21 features

The uploaded GeoJSON coordinates were checked and are compatible with longitude/latitude WGS84.
The zonal-statistics dataset includes `fid`: yes.
