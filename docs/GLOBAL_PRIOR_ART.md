# Global Prior Art — Infrastructure Coordination Systems

Infrastructure coordination is not a new problem. Solutions exist across multiple continents.
Understanding prior art avoids reinvention and identifies what actually needs to be built new.

---

## Health

### DHIS2 (District Health Information System 2)
- **Origin**: University of Oslo, Norway
- **Deployment**: 40+ countries, including Kenya, Uganda, Tanzania, Rwanda
- **What it does**: Aggregate health facility reporting, disease surveillance, supply chain
- **What it doesn't do**: Real-time field data, CHW coordination, patient-level tracking
- **License**: Open source (BSD)
- **Lesson**: Aggregate reporting works at scale. Patient-level coordination doesn't yet.

### OpenMRS
- **Origin**: Partners in Health / Regenstrief Institute
- **Deployment**: 40+ countries, significant Kenya presence
- **What it does**: Electronic medical records for low-resource settings
- **Lesson**: Patient records can be digitized without cloud dependency.

### CommCare (Dimagi)
- **Origin**: MIT / Dimagi
- **Deployment**: 60+ countries
- **What it does**: Community health worker mobile data collection, offline-first
- **Lesson**: Offline-first CHW tools are viable and proven. Battery and data cost are real constraints.

---

## Agriculture

### FEWS NET (Famine Early Warning Systems Network)
- **Origin**: USAID
- **Deployment**: 35+ countries across Africa, Central America, Central Asia
- **What it does**: Food security early warning using satellite + ground truth
- **Lesson**: Satellite-based early warning is operational and saves lives when acted on.

### Digital Green
- **Origin**: Microsoft Research spin-off
- **Deployment**: India, Ethiopia, Ghana
- **What it does**: Video-based agricultural extension using peer-to-peer knowledge transfer
- **Lesson**: Peer video content in local languages outperforms expert-to-farmer transfer.

### Esoko / Farmerline
- **Origin**: Ghana
- **What it does**: Market price SMS alerts for smallholder farmers
- **Lesson**: Price information via SMS changes farmer bargaining behavior measurably.

---

## Water

### WaterAid / WASH systems
- Sector well-documented. Key constraint is monitoring — not technology but data collection at scale.

### mWater
- Mobile-first water quality monitoring. Offline-capable. Proven in field.

---

## Payments / Financial Coordination

### M-Pesa (Kenya / Safaricom)
- The canonical leapfrog case. No fixed infrastructure needed. Mobile money works at village level.

### GrameenPhone / bKash (Bangladesh)
- Parallel development — demonstrates the mobile money model is transferable.

---

## Civic / Government

### Ushahidi
- **Origin**: Kenya, 2008 election crisis
- **What it does**: Crowd-sourced crisis mapping
- **Lesson**: Kenya-origin civic tech can scale globally. Bottom-up data collection works.

### ODK (Open Data Kit)
- Open-source mobile data collection. Standard in global health and development.

### iHub / BRCK (Kenya)
- Local hardware and connectivity innovation. Demonstrates Africa-origin infrastructure R&D.

---

## AI / Coordination specifically

### Kimi Swarm / Multi-agent frameworks
- Demonstrates: agent coordination at scale is operationally viable.

### Sierra Leone teacher AI study (2024)
- AI responses used significantly less mobile data than web search.
- Locally relevant responses rated higher by teachers.
- **Direct implication**: AI can reduce bandwidth cost for last-mile knowledge access.

---

## What Doesn't Yet Exist

1. **Cross-domain coordination** — DHIS2 doesn't talk to kilimo-mcp. wapimaji-mcp doesn't inform bima-mcp at scale. The silos are domain-level, not national-level.

2. **MCP-native African infrastructure tools** — The MCP ecosystem is new (2024). African domain MCP servers are being built now. There is no prior art.

3. **Structured public domain African knowledge in AI-accessible formats** — This is being built (HuggingFace datasets). Prior art: none at this level of structure.

4. **Biomimicry-inspired resilience for African infrastructure coordination** — Novel. No prior art in this specific combination.
