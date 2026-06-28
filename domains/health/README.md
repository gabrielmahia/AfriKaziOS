# Health Coordination

## Coordination Gap
CHWs manage 500-3,000 households with paper registers.
Supply chain stockouts detected only at patient arrival.
Disease surveillance lags by weeks.
Referral network lacks real-time status.

## Data Sources
- DHIS2 (open source, national deployment) — aggregate facility data
- Kenya Health Information System
- WHO Global Health Observatory (open)
- HuggingFace: east-africa-health-historical-pd (PD baseline)

## MCP Integration
- **afya-mcp** (active on PyPI) — health coordination
- **afya-ya-akili-mcp** (active) — mental health
- **county-mcp** (active) — county health service directory

## Key Metrics
- CHW household coverage ratio (target: all households)
- Stockout days per essential medicine per facility
- Disease surveillance lag (field event → national alert)
- Referral completion rate (referred → received care)
- Maternal mortality ratio (county level)

## Coordination Workflows
1. CHW daily sync: offline field data → sync when connected → aggregate
2. Supply chain: facility report → county aggregate → procurement trigger
3. Outbreak detection: quorum threshold across CHW reports → alert
4. Referral: CHW flags → facility notified → transport coordinated
