# East Africa Coordination Infrastructure — Portfolio Brief

*Private. Not for public distribution. For institutional audience.*

---

## The Coordination Problem

Africa's development infrastructure has a persistent architectural gap: data exists but does not flow to decision-makers at the point and time of decision.

A drought early warning system fires six weeks before harvest failure becomes visible. Six weeks is actionable time for:
- Parametric insurance payouts to reach farmers before losses occur
- Drought-resistant crop advisories to reach extension workers
- Community health workers to activate malnutrition surveillance
- County health offices to begin procurement of nutrition supplements

None of this happens automatically. The tools exist. The data exists. The coordination layer between them does not.

This portfolio addresses that gap.

---

## What Has Been Built

### Protocol Layer (32 MCP Servers)

All live on PyPI at [pypi.org/user/gmahia](https://pypi.org/user/gmahia/):

| Domain | Servers | Function |
|--------|---------|----------|
| Finance | mpesa-mcp, kra-mcp, faida-mcp, mkopo-mcp, sifa-mcp | M-Pesa payments, tax, capital markets, credit, reputation |
| Water | wapimaji-mcp | Drought intelligence, satellite data |
| Agriculture | kilimo-mcp, bima-mcp, soko-mcp | Coordination, insurance, market prices |
| Health | afya-mcp, afya-ya-akili-mcp | Primary care, mental health |
| Education | elimu-mcp | School coordination |
| Transport | usafiri-mcp | Route and logistics |
| Land | ardhi-mcp | Registry coordination |
| Language | swahili-civic-nlp, tafsiri-mcp | NLP, translation |
| Civic | county-mcp, fomu-mcp, haki-ya-kazi-mcp | County services, procurement, labor |
| Coordination | africa-coord-bus | Cross-domain event routing |

### Coordination Layer

[`africa-coord-bus`](https://github.com/gabrielmahia/africa-coord-bus) — the event bus connecting the 32 servers.

Built-in routing rules cascade drought signals, disease outbreaks, price spikes, and flood alerts to the appropriate domain tools automatically. Offline-first design: events persist to a local queue and replay when connectivity restores.

### Knowledge Layer (9 HuggingFace Datasets)

All public domain, structured for AI access:

- `east-africa-agricultural-pd` — USDA, Kew Gardens 1910–1925
- `swahili-historical-corpus-pd` — Krapf, Taylor, Steere 1870–1891
- `east-africa-health-historical-pd` — Colonial medical records 1895–1922
- `east-africa-legal-historical-pd` — Customary law records pre-1928
- `africa-historical-maps-pd` — LoC, National Archives, Kew 1688–1925
- `africa-open-climate-data` — NASA, NOAA, USDA (open license)
- `military-strategy-classics` — Sun Tzu, Clausewitz, Jomini (decision support)
- `philosophy-classics-structured` — Structured PD philosophical frameworks
- `african-kingdoms-history` — Pre-colonial African historical record

### Architecture Layer (AfriKaziOS — private)

Private repository documenting:
- 7-domain coordination architecture
- Global prior art (DHIS2, CommCare, FEWS NET, Ushahidi)
- Governance and civil liberties framework
- Biomimicry-inspired resilience patterns (13 patterns documented and implemented)

---

## Standards and Recognition

- **DPGA Listed**: mpesa-mcp (GID0093741, Under Review), swahili-civic-nlp (GID0093743, Under Review)
- **Glama Listed**: All 32 servers indexed
- **Product Hunt**: mpesa-mcp launched
- **MIT License**: All MCP servers and coordination infrastructure (OSI-approved)

---

## Alignment with Nairobi AI Ecosystem

The coordination stack is structurally positioned for the Nairobi AI hub policy environment:

- All tools target Kenya-specific coordination problems
- Swahili language infrastructure (swahili-civic-nlp, tafsiri-mcp)
- DPGA-aligned governance and open source licensing
- Public domain knowledge datasets grounded in East African context
- Offline-first design for low-connectivity environments

The portfolio is not a product. It is infrastructure — the protocol layer that future applications, institutions, and local developers can build on.

---

## Technical Validation

- 32 PyPI packages live and installable
- africa-coord-bus smoke tested: drought alert triggers 5 downstream actions correctly
- wapimaji-mcp v0.1.3: coordination publishing integrated
- coord-cascade-demo: live Streamlit demonstration
- ops-shield: 13 biomimicry defensive AI patterns complete

---

## Contact

contact@aikungfu.dev

*This document is private. Do not distribute publicly.*
