# WindEdge Data Centres
## Turning Scotland's Wasted Wind Into Green Compute

*All figures are referenced in the Sources & Assumptions section at the end of this document.*

---

## The Problem

**Scotland wastes over 900 GWh of wind energy every year.** [1]

Grid operators paid wind farms **£700 million+** [2] in 2023 to switch turbines off — electricity generated and immediately discarded because transmission lines couldn't carry it south. This is growing, not shrinking.

At the same time, GPU compute has never been more valuable or more expensive. AI training, inference, and scientific workloads are driving insatiable demand. Renting an H100 on AWS costs £8–12/hour. [3] And from 2026, enterprises face mandatory Scope 2 emissions reporting — creating real demand for compute that is provably powered by renewables, not just certificate-backed. [4]

---

## The Insight

**The wasted wind is the product.**

Wind farms located in high-curtailment areas of Scotland have a substation, land, and power available for next to nothing — because that power would otherwise be discarded. A modular GPU data centre at that substation can access electricity at an estimated **£5–20/MWh** [11] — approximately 85% below grid rate [10]. Combined with Scotland's cold climate (average ~8°C) [13] eliminating most cooling cost, the result is the world's cheapest genuinely renewable GPU compute.

---

## The Business Model

WindEdge's primary model is a build-and-manage service — designing and commissioning wind-adjacent GPU facilities for clients, earning a fixed build fee and ongoing management fee. As revenue grows, WindEdge builds and owns facilities directly. An alternative route to ownership is a seed raise, compressing the timeline without waiting for managed revenue to accumulate.

### Phase 0 — Self-Funded Pilot (Starting Now)

Buy **4 × RTX 5090 GPUs** (~£2,500 each = ~£10,000 total) and sell compute on **Vast.ai** and **RunPod** — the leading GPU rental marketplaces for AI workloads. No wind farm needed. No investors needed. Proves the revenue model with real data.

| | Estimate | Ref |
|-|----------|-----|
| Hardware (4 × RTX 5090 at ~£2,500 each) | ~£10,000 | [20] |
| Net revenue/GPU/hour on Vast.ai (minus electricity and 25% Vast.ai fee) | ~$0.40 | [18] |
| Occupancy | 85% | [18] |
| **Estimated annual net revenue (4 GPUs)** | **~£9,400/year** | [🔴] |

*Verify current rates on Vast.ai before committing.*

**Customer escalation from marketplace to direct:** Start with anonymous hourly listings on Vast.ai (zero sales effort). Use real utilisation and revenue data to approach direct clients — tech startups needing reserved GPU clusters, university research computing teams, AI companies wanting SLA-backed capacity. Larger enterprises, financial quant teams, and government institutions follow once track record is established.

### Phase 1 — Build-and-Manage Service (Primary Model)

WindEdge designs and commissions **100 kW modular GPU facilities** (~60 GPUs) for clients — wind farm operators, landowners, and private investors who want exposure to the AI infrastructure asset class without the capital required for a full data centre. The client owns the hardware. WindEdge provides everything else.

**What WindEdge delivers:**
- Standard facility design (container, battery, electrical connection, networking)
- EMS algorithm — the core IP — optimising battery, wind, and grid usage in real time
- GPU marketplace management across Vast.ai / RunPod
- Remote NOC monitoring from Edinburgh

**Revenue per managed facility:**

| Stream | Amount | Timing |
|--------|--------|--------|
| Build fee | £40,000–80,000 | One-off on completion |
| Revenue share | 10% of gross GPU revenue | Monthly recurring |

Estimated GPU revenue per 100 kW facility: £120,000–350,000/year [18 — verify]. WindEdge's 10% share: **£12,000–35,000/year** per facility [🔴 author estimate].

**Why this model works:**
- WindEdge doesn't own depreciating hardware — clients do
- Build fees fund operations from Year 1; no continuous equity raises needed
- The EMS algorithm and marketplace management are the moat — clients can't replicate this without WindEdge

### Phase 2 — Owned Facilities (Alternative / Long-Term)

Once the build-and-manage service is generating revenue, WindEdge builds and owns facilities directly at the highest-curtailment sites — capturing 100% of GPU revenue rather than 10%. Two routes: funded from accumulated managed-service revenue, or accelerated by a **seed raise (£300–600k)**. Either path reaches the same destination.

**Estimated unit economics — owned 100 kW facility:** [🔴 all author estimates]

| | Annual |
|-|--------|
| GPU revenue (~60 GPUs, 70% utilisation) | £150,000–300,000 |
| Energy + site costs | ~£66,000 |
| **EBITDA** | **£84,000–234,000** |

*Range reflects uncertainty in GPU market rates. Phase 0 pilot data will narrow this.*

---

## The EMS — Core IP

The Energy Management System is WindEdge's primary patent candidate. A real-time multi-objective optimisation algorithm that:

- Takes inputs: probabilistic wind generation forecast, live turbine SCADA data, battery state of charge, GPU marketplace demand signals, grid electricity spot price
- Outputs: battery charge/discharge commands, GPU load scheduling, grid import/export decisions
- Result: maximum GPU uptime and revenue regardless of wind variability

Designed by two CERN physicists who build exactly this class of real-time optimisation system for particle physics data processing daily.

---

## Why Now

| Force | Effect |
|-------|--------|
| Scottish curtailment growing year-on-year [1] | More sites, lower energy costs |
| GPU compute demand at record highs | Higher marketplace rates, better utilisation |
| Mandatory Scope 2 reporting from 2026 [4] | Clients pay premium for verifiable green compute |
| RTX 5090 affordable enough to bootstrap | Pilot provable for ~£25,000 |
| No UK competitor executing this model | First-mover advantage in wind farm relationships |

---

## Market

| Metric | Figure | Ref |
|--------|--------|-----|
| UK data centre market (2024) | £5.3bn | [7] |
| Market growth rate | ~12% CAGR | [7] |
| Green compute market growth | ~19% CAGR | [8] |
| Direct UK wind-adjacent competitors | Zero | Competitive research |

---

## Team

**Thomas Travis — CEO & Co-Founder**
2nd year PhD in particle physics at CERN (Imperial College London). Leads the full Run 3 VBF Higgs-to-invisible analysis — a flagship model-independent dark matter search — introducing Lorentz-boosted neural networks to the analysis for the first time, processing petabytes of collision data on the CERN Worldwide LHC Computing Grid. Two 5-month internships on Shell's oil trading floor: energy commodity markets, PPA structuring, how large energy companies value long-term supply agreements. Leads commercial strategy, wind farm partnerships, fundraising.

**Sulayman Awan — CTO & Co-Founder**
2nd year PhD in particle physics at CERN (Imperial College London). Pioneering ML research: Graph Transformer networks on raw detector energy deposits combined with ABCDDisco background estimation for a model-agnostic dark matter search (SUEPs). Two industry internships: quant research at Moore Capital (futures strategies, interest rate swaps) and carbon trading strategy at Altana Wealth — directly informing WindEdge's green compute pricing and carbon attribution methodology. Leads EMS algorithm development, GPU marketplace integration, and site commissioning.

**Why this team:**
Thomas and Sulayman sit at the intersection of every domain WindEdge requires: HPC infrastructure (CERN grid), energy markets (Shell), carbon markets (Altana Wealth), quantitative finance (Moore Capital), and frontier ML (both PhDs). They are also the exact customer WindEdge serves — researchers who process petabytes of data daily and know first-hand what GPU compute costs and why green provenance increasingly drives procurement.

---

## Funding

### Phase 0 — No external capital required
~£25,000 self-funded. RTX 5090s, Vast.ai provider account. Start generating revenue immediately.

### Seed — £300,000–600,000 (after pilot validation)

| Use of funds | Amount |
|-------------|--------|
| First owned wind-adjacent facility (100 kW) | £200,000–350,000 |
| Battery storage (~500 kWh) | £80,000–100,000 |
| Legal (PPA, lease, incorporation) | £60,000–80,000 |
| Working capital | £80,000–120,000 |
| **Total** | **£420,000–650,000** |

**SEIS/EIS eligible** — 50% (SEIS) or 30% (EIS) income tax relief for UK investors. [21]

**Why raise after the pilot:**
The seed conversation is transformed when WindEdge walks in with 3 months of real GPU revenue data rather than a spreadsheet model. The pilot de-risks the single biggest investor concern — whether the GPU marketplace revenue is real.

---

## Sources & Assumptions

### Published Sources

**[1] Scottish wind curtailment 900+ GWh (2023)**
National Grid ESO Balancing Mechanism Reporting System (BMRS): bmrs.elexon.co.uk. Verify exact figure from published BM data.

**[2] Constraint payments £700m+ (2023)**
National Grid ESO annual constraint cost data; Ofgem State of the Energy Market report. Verify at nationalgrideso.com.

**[3] AWS H100 GPU pricing £8–12/hour**
AWS published on-demand pricing for GPU instances, converted to per-GPU equivalent at prevailing GBP/USD. Verify at aws.amazon.com/ec2/pricing.

**[4] UK SDR Scope 2 reporting from 2026**
FCA PS23/16; gov.uk/government/publications/sustainability-disclosure-requirements.

**[7] UK data centre market £5.3bn / 12% CAGR**
JLL and CBRE annual UK Data Centre Market Reports (2024/2025). Verify against most recent editions.

**[8] Green compute 19% CAGR**
Grand View Research, Green Data Center Market Report. Analyst estimate — treat as indicative.

**[10] ~85% energy cost advantage**
🔴 Calculated from [11] and grid cost estimates. Not a published figure.

**[11] Curtailed wind PPA rate £5–20/MWh**
🔴 Author estimate. No published market price for bilateral curtailment PPAs (private agreements). Always frame as estimated range, not a market price.

**[13] Scotland average ambient temperature ~8°C**
Met Office UK Climate Averages. metoffice.gov.uk. Verify for specific candidate sites.

**[18] RTX 5090 / GPU marketplace revenue estimates**
🔴 Author estimates based on current Vast.ai and RunPod listed rates for comparable GPU classes. These rates change frequently with GPU supply/demand. **Verify current rates on both platforms before making any financial commitments or presenting these figures to investors or clients.**

**[20] RTX 5090 hardware cost ~£2,500–3,000**
⚠️ Approximate retail pricing in UK as of 2026. Subject to availability and market conditions.

**[21] SEIS/EIS relief rates**
HMRC published guidance. gov.uk/guidance/seed-enterprise-investment-scheme-background.

**All unit economics, revenue projections, and financial model figures**
🔴 Author model estimates. Not validated against operational data. Phase 0 pilot will provide the first real data to replace these assumptions.

---

*WindEdge Data Centres Ltd — Confidential*
*Contact: Thomas Travis — [YOUR EMAIL]*
*June 2026*
