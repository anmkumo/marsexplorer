# MARS EXPLORER — Complete Frontend Prototype

An educational planetary research workspace focused initially on Jezero Crater.

## Included features
- Responsive mission overview dashboard and navigation
- Interactive Mars-style coordinate map (synthetic demonstration grid)
- Mission and rover catalogue with search and status filters
- NASA Image and Video Library live image search
- Click-to-select map coordinates
- Route waypoint builder and approximate spherical distance calculation
- Local research observation notebook
- Mission report preview and TXT download
- Local saved work and JSON export

## Run on Windows
1. Extract the ZIP archive.
2. Open the extracted folder in VS Code.
3. Install the VS Code Live Server extension.
4. Right-click `index.html` and choose **Open with Live Server**.
5. Keep an internet connection for Leaflet and NASA image search.

## Scientific integrity
The map grid is synthetic artwork, not a NASA scientific basemap. NASA Mars Trek provides WMTS map layers, but connecting those layers requires verifying the exact service endpoint, layer identifier, tile matrix, CRS/projection, coverage, attribution and terms. This prototype does not invent a tile URL or claim that the illustrative grid is scientific data.

NASA Image Library search uses `https://images-api.nasa.gov/search`. The legacy NASA Mars Rover Photos API is archived and is not used here. Review each image's original NASA metadata before using it as scientific evidence.

Route distance uses a spherical Mars radius approximation and straight-line segments. It is not terrain-aware, does not account for rover capabilities or hazards, and is not suitable for operational navigation.

## GitHub
Create a public repository named `mars-explorer`, then run in the VS Code terminal:
```bash
git init
git add .
git commit -m "Build Mars Explorer research workspace"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/mars-explorer.git
git push -u origin main
```
