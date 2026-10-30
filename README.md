# Cruise Companion offline maps

Public map data for Cruise Companion by Jenny. This repository contains map release metadata and licensing notices. PMTiles files are attached to GitHub Releases; application source and personal data are not included.

## Release 2026.10.30.1

- One 449,486,508-byte package combines a world overview through zoom 4 and all 232 cruise-port areas through zoom 12.
- 232 optional individual port-area files provide detail through zoom 13.
- The 233 map files total 1,455,622,254 bytes.
- Each port area is approximately 40 km wide, centered on a general port reference. It may not cover the airport and does not identify a verified boarding entrance.
- The app separately bundles its world overview and fonts for first launch. These downloads add optional detail.

See [the release manifest](releases/2026.10.30.1.json) for exact sizes, SHA-256 checksums, bounds and public download URLs. Check every downloaded file against its manifest. A file name contains its SHA-256; do not replace published file contents.

## Source and attribution

© OpenStreetMap contributors. The PMTiles databases are distributed under the [Open Database License 1.0](LICENSE). Retain attribution and provide the license when redistributing. See https://www.openstreetmap.org/copyright.

Source: Protomaps v4.14.3, public OpenStreetMap mirror at https://data.source.coop/protomaps/openstreetmap/v4.pmtiles. OSM replication snapshot: **2026-03-31T04:00:00Z**. This older snapshot is explicitly identified; do not assume current roads, facilities, entrances or navigation conditions.

The files were extracted with the official PMTiles CLI 1.31.2. The all-port package combines world zooms 0–4 and the union of 232 port-area bounds at zooms 5–12. Individual files extract those bounds through zoom 13. The manifest records the areas; the downloaded PMTiles contain the distributed map database.

No routing, live traffic, booking data or personal trip records are included. Source information: https://docs.protomaps.com/basemaps/downloads.
