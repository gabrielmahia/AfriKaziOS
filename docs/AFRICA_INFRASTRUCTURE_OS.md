# Africa Infrastructure OS — Architecture Document

## The Structural Problem

Every domain of African infrastructure coordination shares a common failure pattern:

1. **Data exists but is fragmented** — health records in DHIS2, agricultural data in paper ledgers, water quality in lab notebooks, transport data in ministry spreadsheets. Each source knows its domain. Nothing talks to anything else.

2. **Systems exist but don't communicate** — M-Pesa knows payment flows. NHIF knows insurance claims. County assemblies know budget allocations. The same person appears in all three systems with no shared identifier and no shared data.

3. **Knowledge exists but isn't actionable** — A community health worker 40km from a clinic knows which households have sick children. That knowledge has no path to the supply chain that stocks the clinic.

AfriKaziOS is the coordination layer. Not a replacement for existing systems — a connective tissue between them.

---

## The Composable Model

```
Raw signal (field data, satellite, market prices, health events)
        │
        ▼
Domain MCP servers (structured access layer)
        │
        ▼
Coordination layer (AfriKaziOS — cross-domain synthesis)
        │
        ▼
Decision support (AI agents, human decision-makers)
        │
        ▼
Action (resource allocation, alert, procurement, policy)
        │
        ▼
Feedback loop (outcome data flows back to raw signal layer)
```

Each layer is replaceable. The MCP servers can be swapped. The AI models can be swapped. The coordination protocols can evolve. What persists is the architecture.

---

## Domain Architecture

### Agriculture
**Coordination gap**: Farmers don't know current market prices before harvest decisions. Extension officers can't reach all farmers. Insurance claims take months after drought. Credit history doesn't travel across lenders.

**Infrastructure needed**:
- Real-time market price aggregation (mpesa-mcp payment flows as proxy)
- Weather and drought early warning (wapimaji-mcp + NASA NDVI)
- Parametric insurance triggers (bima-mcp + satellite data)
- Credit profile portability (sifa-mcp)

### Water
**Coordination gap**: Borehole status unknown centrally. Water quality tested infrequently. Drought declared after visible damage, not predictive. Water user associations lack data.

**Infrastructure needed**:
- Borehole network status monitoring
- Drought early warning (6-8 week horizon via NDVI anomaly)
- Water quality incident coordination
- Community water resource mapping

### Health
**Coordination gap**: Community Health Workers manage 500-3,000 households with paper registers. Supply chain stockouts not detected until patients arrive. Disease surveillance lags by weeks.

**Infrastructure needed**:
- CHW digital coordination tools (offline-first)
- Supply chain visibility (facility → county → national)
- Disease surveillance (real-time aggregate, privacy-preserving)
- Referral network coordination

### Education
**Coordination gap**: School enrollment data siloed by county. Teacher deployment not matched to enrollment. Learning outcomes not tracked longitudinally.

**Infrastructure needed**:
- Enrollment and attendance coordination
- Teacher-to-student ratio optimization
- Learning outcome longitudinal tracking
- Exam preparation resource distribution

### Transport
**Coordination gap**: Matatu routes not formally mapped. Road condition data in ministry, not available to logistics planners. Freight rates not aggregated.

**Infrastructure needed**:
- Informal transport route mapping (OSM + crowd-sourced)
- Road condition data integration
- Freight rate aggregation
- Last-mile logistics optimization

### Energy
**Coordination gap**: Grid connection wait times variable and opaque. Off-grid solar systems not aggregated for virtual power plant potential. Fuel price data not systematically collected.

**Infrastructure needed**:
- Grid connection status coordination
- Off-grid asset registry
- Energy access mapping
- Demand forecasting

### Procurement
**Coordination gap**: Public procurement opportunities not aggregated. Bid evaluation processes opaque. Vendor registration duplicated across entities.

**Infrastructure needed**:
- OCDS-aligned procurement data aggregation
- Vendor registry interoperability
- Bid alert and notification
- Procurement analytics

---

## The Leapfrog Thesis

Africa's infrastructure constraint is not bandwidth or capital — it is coordination.

Mobile phone penetration and M-Pesa demonstrated that Africa leapfrogged fixed-line telephony and traditional banking. The same pattern is available in every domain:

- Health: skip paper records → jump to AI-assisted CHW coordination
- Agriculture: skip agricultural extension offices → jump to AI-assisted market intelligence
- Transport: skip fixed route systems → jump to dynamic AI-assisted logistics

The constraint in each case is not technology. It is structured data and coordination protocols. AfriKaziOS is the protocol layer.

---

## Technology Stack

**Primary languages**: Python (MCP servers, data pipelines), TypeScript (A2A agents)
**AI frameworks**: Google ADK (agent coordination), MCP (tool interfaces)
**Data**: HuggingFace datasets (structured PD knowledge), PostgreSQL+pgvector (operational)
**Deployment**: Streamlit (field interfaces), FastAPI (coordination APIs)
**Edge**: USSD-compatible interfaces via Africa's Talking

---

## What This Is Not

- Not a centralized database
- Not a surveillance system
- Not dependent on any single AI provider
- Not a replacement for existing government systems
- Not requiring internet connectivity at the point of use
