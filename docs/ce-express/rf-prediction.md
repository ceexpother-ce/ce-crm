# RF Prediction

## Requirements Before Running
1. **Network objects** — at least one cell with latitude, longitude, cell_name
2. **Geodata** — `elevation.tif` in GeoTIFF format, Projected CRS, NoData = -9999
3. **Antenna patterns** — imported .msi or .txt files assigned to cells
4. **Prediction model** — configured in the Prediction Models tool
5. **Workspace** — with geodata path set and correct coordinate system

## Run RF Prediction
1. Select your cells on the map
2. Open the **RF Prediction** tool
3. Set **Resolution**
4. Set **Best server count** (minimum 3)
5. Click **Calculate**
6. Results appear in **Prediction History** — green = complete, yellow = calculating

## Quick RF Prediction
For a fast single-cell preview:
1. Open the **Quick RF Prediction** tool
2. Hold `CTRL` and click the cell
3. Set Resolution to `1` for best quality
4. View results in **Layers → Prediction results**

> **Note:** Quick RF calculates field strength only. For RSRP, SINR, throughput — use the full RF Prediction tool.

## Output Fields
| Field | Unit | Description |
|---|---|---|
| RSRP | dBm | Reference Signal Received Power (1st–5th best server) |
| RS-SINR | dB | Signal to Interference + Noise Ratio |
| DL Throughput | Mbps | Estimated downlink throughput |
| UL Throughput | Mbps | Uplink throughput |
| Best Server ID | — | Identifier of the strongest serving cell |

## Publish to ArcGIS Portal
1. In **Prediction History**, hover over a completed result
2. Click the upload arrow **↑**
3. Confirm with **OK**
4. Result is published as a hosted feature layer on ArcGIS Enterprise Portal

## Related Topics
- [Prediction Models](rf-prediction.md)
- [Geodata & Rasters](geodata.md)
- [Antenna Patterns](antenna-patterns.md)
