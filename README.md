# webapp-leaflet-boston-street-trees: Leaflet + GeoServer Web App

An interactive web map that allows users to click on any street tree in Boston and see the species.

## Tech Stack
- PostGIS
- GDAL / ogr2ogr
- GeoServer (WMS publishing)
- Leaflet

## Workflow
- Ingest street tree GeoJSON into PostGIS using ogr2ogr.
- Publish the tree layer as WMS through GeoServer.
- Build an interactive Leaflet web map with click-to-identify.
- Style tree points using a custom SLD.
- Provide two versions:
  - Full WMS version (main branch)
  - Public demo with local subset (External-access branch)

## Demo and Data
Live demo: https://dk32093.github.io/webapp-leaflet-boston-street-trees/

Street trees data: https://data.boston.gov/dataset/treekeeper-street-trees

![Closeup screenshot](<Screenshot1.png>)
![Medium zoom screenshot](<Screenshot2.png>)
![Zoomed out screenshot](<Screenshot3.png>)