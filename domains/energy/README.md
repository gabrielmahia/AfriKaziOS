# Energy Coordination

## Coordination Gap
Grid connection wait times opaque. Off-grid solar not aggregated. Fuel price data fragmented.

## Data Sources (Public Domain / Open)
- IRENA (open data) — renewable energy capacity by country
- World Bank Energy Atlas (open data)
- Kenya Power connection data (if available via KPLC API)
- AfDB infrastructure data

## MCP Integration
- No active MCP server yet — architecture phase
- Target: energy-mcp (planned)

## Key Metrics
- Grid connection wait time (proxy: KPLC queue data)
- Off-grid solar installed capacity (village level)
- Fuel price index (Nairobi / county seats)
- Load shedding frequency and duration

## Coordination Workflows
1. Off-grid asset registry → virtual power plant potential assessment
2. Grid extension priority scoring (population density + economic activity)
3. Fuel price alert system for logistics planning
