What This Code Does

This is a Tree Equity Index (TEI) analysis tool for Nairobi, Kenya, built using Google Earth Engine (GEE) and Python. It measures how equitably tree canopy cover is distributed across urban settlements, factoring in environmental stress and population vulnerability.
The workflow in plain terms:
It identifies settled areas using two satellite datasets (ESA WorldCover and GHSL), overlays a 1km grid, then for each grid cell calculates four indicators: tree canopy cover, land surface temperature (heat stress), population density, and built-up surface fraction. These are normalized and combined into a single 0–100 score where higher = better tree equity.
The scoring formula weights the indicators like this:

Heat stress: 35%
Vegetation deficit: 30%
Population density: 20%
Built-up fraction: 15%

Results are visualised as choropleth maps (plain and basemap-overlaid) and can be exported as GeoJSON or CSV.

Many thanks to Seval Celik @sevalcelik majority of this code was adapted from what she had done 