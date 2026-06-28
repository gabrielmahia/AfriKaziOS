# Agriculture Coordination

## Coordination Gap
Farmers don't know market prices before harvest decisions.
Extension officers can't reach all farmers.
Insurance claims take months after drought.
Credit history doesn't travel across lenders.

## Data Sources
- NASA NDVI / MODIS (open) — crop health monitoring
- USDA FAS (open) — production estimates
- FEWS NET (USAID open) — food security zones
- HuggingFace: east-africa-agricultural-pd — crops, soil, water (PD)
- HuggingFace: africa-open-climate-data — climate baseline

## MCP Integration
- **kilimo-mcp** (active) — agricultural coordination
- **wapimaji-mcp** (active) — drought intelligence
- **bima-mcp** (active) — parametric crop insurance
- **soko-mcp** (active) — market prices

## Key Metrics
- Market price information lag (field price vs farmer knowledge)
- Extension officer reach ratio (farmers reached / total farmers)
- Insurance payout lag (trigger event → payment)
- Crop calendar adherence (actual planting vs optimal planting date)
- Post-harvest loss rate

## Coordination Workflows
1. Price alert: soko-mcp price scrape → SMS/USSD alert to registered farmers
2. Drought trigger: wapimaji-mcp NDVI anomaly → bima-mcp parametric payout
3. Extension: kilimo-mcp route optimization → CHW-style household coverage
4. Credit: sifa-mcp payment history → portable credit profile
