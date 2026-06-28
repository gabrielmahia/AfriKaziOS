# AfriKaziOS

> AI-supported institutional coordination infrastructure for Africa — health, water, energy, agriculture, transport, education, procurement.

**Private research and architecture repository.**

---

## Mission

African infrastructure coordination suffers from the same structural problem across every domain:

- Data exists but is not structured for AI access
- Systems exist but do not communicate with each other  
- Knowledge exists but is not actionable at the point of decision

AfriKaziOS is the architecture for closing those gaps — domain by domain, protocol by protocol.

## Architecture

```
AfriKaziOS
├── domains/          # Domain-specific coordination layers
│   ├── energy/
│   ├── water/
│   ├── health/
│   ├── agriculture/
│   ├── transport/
│   ├── education/
│   └── procurement/
├── docs/             # Architecture, prior art, governance
├── schemas/          # Shared data schemas (JSON Schema / Pydantic)
├── workflows/        # Coordination workflow definitions
└── reports/          # Analysis and research
```

## Domains

| Domain | Status | MCP Integration | Key Data Sources |
|--------|--------|----------------|-----------------|
| Agriculture | Active | kilimo-mcp, wapimaji-mcp | USDA PD, Kew Gardens PD, NASA NDVI |
| Water | Active | wapimaji-mcp | CHIRPS, TRMM, NOAA |
| Health | Architecture | afya-mcp | WHO, county-mcp |
| Education | Planning | elimu-mcp | National exam data, DHIS2 |
| Transport | Planning | usafiri-mcp | OSM, infrastructure surveys |
| Energy | Research | — | IRENA, AfDB data |
| Procurement | Research | — | Kenya PPRA, OCDS |

## Design Principles

**1. Offline-first.** Coordination tools must work with intermittent connectivity.
Infrastructure decisions are often made in the field, not at a desk.

**2. Public domain where possible.** Historical knowledge is free.
Structuring it for AI access is the work.

**3. Model-agnostic.** The coordination layer must work regardless of which LLM
is used — Gemini, Claude, GPT, or open-weight models running locally.

**4. Biomimicry as architecture.** Immune systems, mycelial networks, and ant
colonies solve coordination problems at scale without central control.
African infrastructure faces the same challenge.

**5. Governance built in.** Not retrofitted. Civil liberties and data sovereignty
considerations are part of the architecture, not compliance afterthoughts.

## Related Public Repositories

- [mpesa-mcp](https://github.com/gabrielmahia/mpesa-mcp) — payments
- [wapimaji-mcp](https://github.com/gabrielmahia/wapimaji-mcp) — water/drought
- [kilimo-mcp](https://github.com/gabrielmahia/kilimo-mcp) — agriculture
- [swahili-civic-nlp](https://github.com/gabrielmahia/swahili-civic-nlp) — language

---

*Private repository. Architecture and research.*
