# Governance and Rights — AfriKaziOS

## The Surveillance Risk

AI coordination infrastructure for Africa carries a documented and serious risk: the same
systems that improve health coordination, drought response, and agricultural planning can
be repurposed for surveillance, political targeting, and civil liberties violations.

This is not hypothetical. AI surveillance systems are already expanding across Africa.
Facial recognition in Uganda (Huawei). Social credit models exported from China.
Biometric voter registration data with unclear custody. CCTV networks with undisclosed
data retention and access policies.

Governance cannot be retrofitted. It must be in the architecture from the start.

---

## Principles

### 1. Data minimization
Collect the minimum data required for the coordination function.
Aggregate at the earliest possible point.
Never collect individual-level data when aggregate data serves the purpose.

### 2. Purposeful collection
Data collected for health coordination is not available for law enforcement.
Data collected for agricultural coordination is not available for tax enforcement.
Purpose limitation must be technically enforced, not just policy-stated.

### 3. Community ownership
Data about a community belongs to that community.
National aggregation rights must be explicitly negotiated, not assumed.
Opt-out must be technically possible.

### 4. Transparency over opacity
Every coordination decision made by an AI system must be explainable
in plain language to the person it affects.
Black-box decisions on resource allocation are not acceptable.

### 5. Offline sovereignty
A coordination system that requires cloud connectivity centralizes power.
Edge-capable, offline-first architecture distributes it.

---

## High-Risk Functions — Prohibited by Default

The following coordination functions are prohibited in AfriKaziOS unless
explicitly reviewed and approved against rights criteria:

1. **Individual movement tracking** — GPS-level location history on individuals
2. **Behavioral scoring** — Any scoring system that rates individuals for access to services
3. **Predictive policing** — Any function that predicts individual criminal behavior
4. **Political affiliation inference** — Any inference about political views from behavioral data
5. **Biometric identification** without explicit consent and purpose limitation

---

## Risk Assessment Framework

For any new coordination function, assess:

| Question | Required Answer |
|----------|----------------|
| Who controls the data? | Community / designated steward — not vendor, not government by default |
| What is the minimum data required? | Explicitly stated and enforced technically |
| Who has access? | Explicitly enumerated — no open access |
| What is the retention period? | Shortest that serves the coordination purpose |
| Can it be repurposed? | Technically prevented, not just policy-stated |
| What is the off-switch? | Explicit shutdown path — not just decommission plan |

---

## Legal Framework References

- **Kenya Data Protection Act 2019** — Binding for Kenya-deployed systems
- **African Union Convention on Cyber Security and Personal Data Protection** (Malabo Convention)
- **GDPR** — Applicable where EU-origin data or funding involved
- **IFC Performance Standard 2** — Labor and working conditions; relevant for CHW data

---

## Accountability

AfriKaziOS maintains this document and updates it as new coordination functions are designed.
Any deployment partner must acknowledge this governance framework before receiving access
to coordination infrastructure.

Violations are reported to: the relevant national data protection authority, community
representatives, and (where applicable) funding bodies.
