# Geodata & Rasters

## Required Files
| File | Required | Description |
|---|---|---|
| `elevation.tif` | ✅ Yes | Digital Terrain Model (DTM) |
| `clutterClasses.tif` | Optional | Land use / clutter classification |
| `clutterHeight.tif` | Optional | Clutter height above terrain |

## Format Requirements
- **Format:** GeoTIFF
- **CRS:** Projected (not geographic/WGS84)
- **NoData value:** `-9999`
- All files must use the **same CRS** as the workspace

## Related Topics
- [Workspace](workspace.md)
- [RF Prediction](rf-prediction.md)
