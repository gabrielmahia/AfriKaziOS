# Water Coordination

## Coordination Gap
Borehole network status unknown centrally. Drought declared after visible damage.
Water quality tested infrequently. WASH data siloed by implementer.

## Data Sources
- NASA CHIRPS (open) — daily rainfall 0.05° resolution
- NASA MODIS NDVI (open) — vegetation index, drought proxy
- NOAA Africa Rainfall Estimates (open)
- Kenya Water Resources Authority data
- HuggingFace: africa-open-climate-data

## MCP Integration
- **wapimaji-mcp** (active, v0.x on PyPI) — drought intelligence
- wapimaji-mcp feeds: bima-mcp (parametric insurance triggers)

## Key Metrics
- Rainfall anomaly (vs 30-year baseline)
- NDVI anomaly (6-8 week drought early warning)
- Borehole operational status (crowd-sourced)
- Water point accessibility (walking distance)
- Groundwater level (where measured)

## Coordination Workflows
1. Drought early warning: NDVI anomaly → alert → parametric insurance trigger
2. Water point status: crowd-source → aggregate → routing for field teams
3. Water quality incident: field report → aggregate → county response
