# Drought Response Workflow

## Trigger Conditions (Quorum Sensing Pattern)
Response triggers when ≥3 of the following signals are above threshold:

| Signal | Source | Threshold |
|--------|--------|-----------|
| NDVI anomaly | wapimaji-mcp / NASA | -0.15 below seasonal mean |
| Rainfall deficit | wapimaji-mcp / CHIRPS | <60% of 30-year mean |
| SPI (Standardized Precipitation Index) | NOAA | SPI-3 < -1.5 |
| Market price spike (maize) | soko-mcp | >30% above seasonal mean |
| CHW field reports | afya-mcp | >20% households flagging food insecurity |

## Response Cascade

```
QUORUM THRESHOLD MET
        │
        ├─► wapimaji-mcp: Issue drought alert (county level)
        │
        ├─► bima-mcp: Trigger parametric insurance evaluation
        │       └─► If SPI confirms: Initiate payout process
        │
        ├─► kilimo-mcp: Activate drought-resistant crop advisory
        │       └─► SMS/USSD to registered farmers in affected counties
        │
        ├─► afya-mcp: Activate malnutrition surveillance protocol
        │       └─► CHW household surveys prioritized
        │
        └─► county-mcp: Alert county water and agriculture offices
```

## Data Flow
1. Satellite data (NASA/NOAA) → wapimaji-mcp (daily update)
2. Market price data → soko-mcp (weekly update)
3. CHW reports → afya-mcp (on sync)
4. Quorum evaluation → coordination_event (drought_alert) → cascade

## Privacy
All data in this workflow is aggregate. No individual identification.
County-level minimum granularity for alerts.
