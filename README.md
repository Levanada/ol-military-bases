# Global Military Areas

## [Live Example](https://cdgis.com/?layers=global-military-bases&lng=-116.551137&lat=37.330197&zoom=7.85&bearing=0.00&pitch=0.00&style=dark&terrain=0)

Global military areas extracted from [OpenStreetMap](https://www.openstreetmap.org/) as Mapbox Vector Tiles.

Feel free to download and host the tiles yourself, or load them directly from the CDN URL below.

<img width="2155" height="432" alt="image" src="https://github.com/user-attachments/assets/2d4a5912-220a-4b04-87c5-dd6e6ef239cd" />

## Usage

XYZ tile template:

```text
https://cdn.jsdelivr.net/gh/Levanada/ol-military-bases@main/tiles/{z}/{x}/{y}.pbf
```

Example:

```text
https://cdn.jsdelivr.net/gh/Levanada/ol-military-bases@main/tiles/7/17/29.pbf
```

Compatible with MapLibre GL, Mapbox GL, OpenLayers, deck.gl `MVTLayer`, and other MVT clients.

> **Note:** Tiles are gzip-compressed. Many CDNs (including jsDelivr) serve the raw gzip bytes without a `Content-Encoding: gzip` header. Clients must decompress before parsing, or configure their tile server to advertise gzip encoding.

## r12 Changes
- Increased maximum zoom from 13 to 14.
- Data generated/validated on 2026-08-05.

## Specs

| | |
| --- | --- |
| **Format** | Mapbox Vector Tiles (`.pbf`) |
| **Compression** | Gzip |
| **Scheme** | XYZ |
| **Zoom** | 0–14 |
| **Coverage** | Global |
| **Source** | OpenStreetMap (`landuse=military`, `military=*`) |

## License

This repository does not add a separate license for the tile packaging.

OpenStreetMap data is available under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/). If you use this dataset, you must follow ODbL attribution and share-alike requirements.
