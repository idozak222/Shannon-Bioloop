# 🔁 6. Shannon BioLoop
*Voice: environmental innovator — pragmatic, startup-savvy*

A challenge brief to prototype a **circular bio-economy atlas** for the Shannon Basin.

---

## Background
The Shannon Basin’s agri-industrial ecosystem produces abundant organic by-products—dairy residues, crop waste, timber offcuts, and municipal organics. Under **Ireland’s Circular Economy Strategy**, these can become new revenue streams through **local bio-loops**.

**Context refs**
- Circular Economy Strategy 2022–2023  [[link]][ces]
- Teagasc Anaerobic Digestion (AD) Portal  [[link]][teagasc-ad]

---

## Problem
Design a **geospatial map of resource loops**—connecting waste producers, processors, and end-users—to surface feasible circular-economy pilots (e.g., biogas co-ops, fibre crops for insulation, reuse hubs, compost exchanges).

**Key questions**
- What feedstocks exist, where, and at what volumes/seasonality?
- Which processors and off-takers are viable within realistic logistics radii?
- Which loops pencil out on unit economics and regulatory feasibility?

---

## Expected Outcomes
1. **Shannon BioLoop Atlas**  
   - Public, browsable map (web) + source data (CSV/GeoJSON)  
   - Layers: feedstocks, processors, logistics corridors, demand nodes

2. **Loop Micro-Economics Sheets**  
   - CAPEX/OPEX, yields, transport assumptions, sensitivity ranges

3. **Regulatory Checklists**  
   - Permits, compliance steps, standards, and relevant authorities

> The Atlas serves as a **teaching aid**, **research reference**, **investment teaser**, and a **prototype** for circular-enterprise hubs.

---

## Difficulty
**Intermediate** — data synthesis + stakeholder mapping.

---

## Scope
**Includes**
- Organics (agri/forestry/municipal), material reuse, logistics mapping

**Excludes**
- Heavy-industry planning

---

## Resources
- National Waste Management Plan 2024–2030  [[link]][nwm-2430]
- Bord na Móna Peatlands Climate Action Scheme  [[link]][bnm-pcas]
- Enterprise Ireland Green Transition Fund  [[link]][ei-gtf]

---

## Inspiration
**Kalundborg Symbiosis (Denmark)** shows that waste-as-resource ecosystems can sustain rural economies while cutting emissions.

---

## Deliverables & Milestones
- **M1 – Data framing (Week 1–2)**  
  Schema, sources list, data license proposals; initial county-level inventory
- **M2 – Atlas MVP (Week 3–4)**  
  Base map with feedstock + processor layers (GeoJSON), simple proximity logic
- **M3 – Loops pack (Week 5–6)**  
  5–8 candidate loops with micro-econ sheets + regulatory checklists
- **M4 – Readout (Week 7)**  
  Demo map, summary note, and next-step pilot shortlist

---

## Implementation Hints
- **Stack**: QGIS for wrangling → export GeoJSON → MapLibre/Leaflet for web map  
- **Data model**: `nodes.csv` (type, coords, capacity), `edges.csv` (flow, cost, distance), `loops.yml` (assumptions)  
- **Assumptions**: standardize units (t/yr, m³/yr); include min/avg/max ranges

---

## Contributing
Issues and PRs welcome. Please:
- Cite sources in `/sources/README.md`
- Include a changelog entry and data dictionary updates
- Follow coding style in `/web/CONTRIBUTING.md`

---

## License
TBD (suggestion: **ODbL** for data, **CC BY 4.0** for docs, **MIT** for code)

---

## Maintainers
TBD — add contact and governance notes.

---

[ces]: <ADD_OFFICIAL_URL>
[teagasc-ad]: <ADD_OFFICIAL_URL>
[nwm-2430]: <ADD_OFFICIAL_URL>
[bnm-pcas]: <ADD_OFFICIAL_URL>
[ei-gtf]: <ADD_OFFICIAL_URL>
