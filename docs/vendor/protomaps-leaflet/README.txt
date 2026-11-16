protomaps-leaflet 5.1.0 (BSD-3-Clause), https://github.com/protomaps/protomaps-leaflet, fetched from https://unpkg.com/protomaps-leaflet@5.1.0/dist/protomaps-leaflet.js on 2026-11-15.
Draws the Protomaps vector basemap (PMTiles, OpenStreetMap data, ODbL: attribution "Protomaps (c) OpenStreetMap" is shown on the map) in the viewer's Leaflet map.
flavor_plain.json = the library's "grayscale" colour table with this project's overrides (muted green open land, darker buildings, dark street names); see docs/index.html (plainBuild).
Not used with 4.0.1: that release expects an older Protomaps data layout and draws no roads or labels from current builds.
plain_style.js = the plain base map's paint and label rules (shared by the viewer and scripts/basemap_raster_job.html, which draws the zoomed-out picture tiles); flavor_plain.json = its colour table.
Two files on blob storage (aerial container): chicago_basemap.pmtiles (vector, zoom 0-15, used at zoom 0-9 and 17+) and chicago_basemap_raster.pmtiles (512 px WebP pictures, zoom 10-16; scripts/basemap_raster.py).
