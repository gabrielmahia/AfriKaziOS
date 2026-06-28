# Transport Coordination

## Coordination Gap
Matatu routes informally operated, not mapped.
Road condition data in ministry, not available to logistics planners.
Freight rates not aggregated. Last-mile logistics expensive.

## Data Sources
- OpenStreetMap (open) — road network
- Kenya Roads Board data (where available)
- Africa OSM community contributions
- Matatu route crowd-sourcing projects

## MCP Integration
- **usafiri-mcp** (active on PyPI) — transport coordination
- Target integration: soko-mcp (market access routing)

## Key Metrics
- Road accessibility index (% of population within Xkm of passable road)
- Informal route coverage (matatu network mapped %)
- Freight rate per corridor (agricultural produce to market)
- Last-mile cost (farm gate to county town)
- Road condition rating (passable / seasonal / impassable)

## Coordination Workflows
1. Route mapping: crowd-source GPS traces → matatu route database
2. Road condition: crowd-source reports → condition map → logistics routing
3. Freight: rate aggregation → price transparency for smallholder logistics
