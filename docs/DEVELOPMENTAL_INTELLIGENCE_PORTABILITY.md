# Developmental Intelligence Portability

**Date:** 2026-09-09  
**Purpose:** ensure AfriKaziOS can express radically different African local phenotypes without baking one ecology, language, or institution into the core.

## Core rule

AfriKaziOS should not implement "the African environment" because no such singular environment exists.

Use:

```text
conserved coordination contracts
+ local environment manifest
+ domain specialist modules
+ current reality state
+ human authority
→ locally competent phenotype
```

Murang'a, Turkana, Bunyala, the Sahel, Lagos, Kinshasa, Cape Town, island/coastal systems, refugee settings and informal settlements must be treated as distinct operating environments sharing interoperable infrastructure rather than as variants of one canonical deployment.

## Stable developmental interfaces

Prefer a small set of reusable contracts across domains:

- identity / actor;
- location / spatial scope;
- time / freshness;
- authority / jurisdiction;
- evidence / provenance;
- environment state;
- resource constraints;
- uncertainty;
- action;
- human escalation;
- outcome / feedback.

These are developmental bottlenecks: stable interfaces through which many local phenotypes can be composed.

## Plastic versus canalized behavior

**Canalized behavior** should remain stable across environment changes:

- safety boundaries;
- provenance requirements;
- permission checks;
- uncertainty representation;
- audit logging;
- destructive-action safeguards;
- human authority boundaries.

**Plastic behavior** should respond to environment:

- language and code-switching;
- relevant crops/livestock;
- hydrology and climate;
- local institutions;
- transport constraints;
- market structure;
- available communications;
- specialist tools and datasets.

Do not let plastic local context silently alter canalized governance behavior.

## Environment manifest requirement

A deployable workflow should declare its assumptions rather than hide them in prompts or code.

Minimum manifest fields:

```yaml
environment_id:
location_scope:
languages:
livelihoods:
ecological_regime:
infrastructure_modes:
authoritative_sources:
available_tools:
offline_requirements:
human_authorities:
known_failure_modes:
last_verified:
```

Unknown values stay UNKNOWN.

## Portability test

No domain workflow should be called a reusable African rail until it is attacked with an ecologically distant second environment.

For every transfer measure:

- core files changed;
- local/context files changed;
- new data required;
- new tools required;
- human validation time;
- compute cost;
- capability retained;
- failure modes introduced.

The target is not zero localization. The target is **localization without architectural reinvention**.

## Niche construction

When a workflow repeatedly fails because the environment is poorly represented, do not default to a bigger model.

Ask whether the better move is to change the environment the intelligence operates in:

- expose a missing API;
- standardize a local form;
- create a shared geospatial layer;
- instrument a water point;
- digitize an extension handbook;
- collect governed local speech;
- create a validated local atlas;
- improve a feedback channel.

Making reality easier to observe can create more durable capability than making the model better at guessing.

## Relationship to the Evolution Lab

The canonical theory and executable research scaffold live in `gabrielmahia/nature-ai-evolution-lab`:

- `docs/DEVELOPMENTAL_INTELLIGENCE_RESEARCH_2026-09-09.md`
- `src/research/developmental.py`
- `data/research/environment-manifests-v0.json`
- `data/research/capability-genome-v0.json`

AfriKaziOS should consume the contracts and prove them in institutional/domain systems. It should not duplicate the model-evolution selection logic.
