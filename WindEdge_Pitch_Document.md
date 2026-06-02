# WindEdge Data Centres
## Turning Scotland's Wasted Wind Into the World's Greenest Compute

*All figures are referenced in the Sources & Assumptions section at the end of this document.*

---

## The Problem

**Scotland wastes over 900 GWh of wind energy every year.** [1]

When wind turbines generate more electricity than the transmission grid can carry south, National Grid ESO pays farm operators to switch off. In 2023 alone, those constraint payments exceeded **£700 million** [2] — electricity generated and immediately discarded.

At the same time, UK data centres pay **£100–140/MWh** [3] for electricity — their single largest operating cost at **40–60% of opex** [4]. And from 2026, UK Sustainability Disclosure Requirements oblige large enterprises to report Scope 2 emissions [5], creating urgent demand for verifiably renewable compute that the market currently cannot supply. Certificate-based "green" claims are widely criticised as greenwashing. Genuinely renewable compute — provable at the electron level — does not exist at commercial scale in the UK.

---

## The Opportunity

| Metric | Figure | Ref |
|--------|--------|-----|
| Scottish wind curtailed annually (2023) | 910 GWh | [1] |
| Projected curtailment by 2028 | 2,000+ GWh | [6] |
| Constraint payments to wind farms (2023) | £703m | [2] |
| UK data centre market (2024) | £5.3bn | [7] |
| UK data centre market growth rate | 12% CAGR | [7] |
| Green compute market growth rate | 19% CAGR | [8] |
| Enterprises facing mandatory Scope 2 reporting (2026) | All FTSE 350 + large private | [5] |

Curtailment is a structural and worsening problem. Grid upgrades are not projected to complete until 2030–2033 at the earliest [9]. WindEdge converts that stranded asset into revenue.

---

## The Solution

WindEdge deploys **modular, containerised data centres at wind farm substations** — consuming electricity directly at source, behind the turbine meter, before it touches the grid.

**Three advantages stack to create an unassailable cost position:**

**1. Energy at ~85% below market** [10]
Behind-the-meter connection allows negotiated access to curtailed wind at an estimated **£5–20/MWh** [11] versus **£100–140/MWh** [3] on the open market. Transmission charges — typically **£15–25/MWh** [12] for grid consumers — are eliminated entirely.

**2. Near-zero cooling cost**
Scotland's average ambient temperature of **~8°C** [13] enables free-air cooling for an estimated **~89% of operating hours** [14], achieving a Power Usage Effectiveness (PUE) design target of **1.05–1.10** [15]. The UK industry average is **1.58** [16]. This eliminates an estimated **£80–120k per MW per year** [17] in energy cost versus a London or Manchester facility.

**3. The strongest green claim available**
Customers' compute is powered by the wind turbine 200 metres away. This is verifiable at source, in real time — not a certificate representing renewable energy generated somewhere in the grid at some point in the past. No grid-connected competitor can make this claim at any price.

---

## How It Works

```
Wind Turbines
     │
     ▼
Wind Farm Substation
     │
     ├──► Grid export (when not curtailed)
     │
     └──► WindEdge site (consumes curtailed energy)
               │
               ├── Battery buffer (2–4 MWh)   ← bridges wind lulls
               ├── Grid tie-in (backup)        ← guarantees uptime
               └── IT Load hierarchy:
                     Priority 1: Colocation customers  (always on)
                     Priority 2: Managed HPC / GPU     (can pause)
                     Priority 3: AI training queues    (delay-tolerant)
                     Priority 4: Flexible mining       (instant-off)
```

WindEdge's proprietary **Energy Management System (EMS)** — the core IP — optimises battery charging, wind consumption, and load distribution in real time using wind generation forecasts, turbine SCADA data, grid electricity prices, and battery state of charge. The result: customers on Priority 1 experience **>99.9% uptime** despite being located at a wind farm.

---

## Business Model

### Revenue Streams

| Stream | Mechanism | Target % of Revenue |
|--------|-----------|-------------------|
| Colocation | Rack space + power rented to enterprises | 50% |
| Managed GPU / HPC | NVIDIA H100 clusters, billed hourly | 25% |
| Grid demand response | National Grid ESO pays for flexible load | 10% |
| Flexible mining | Absorbs surplus wind; marginal income | 15% |

*Revenue split is a modelling assumption — see [18].*

### Unit Economics — Per 1 MW Site (Steady State) [18]

| | Annual |
|-|--------|
| Revenue | £2,006,000 |
| Energy cost (curtailed wind + grid backup) | £214,000 |
| All site opex (connectivity, lease, O&M) | £349,000 |
| Central overhead allocation | £120,000 |
| **EBITDA** | **£1,537,000** |
| **EBITDA Margin** | **76.6%** |

*All unit economics figures are author projections based on the assumptions set out in [18]. They have not been validated against operational data.*

Payback per site: **3.5–4.5 years** [18]. 20-site portfolio target revenue: **£40m+** [18].

---

## Market & Competition

**No UK competitor currently executes this model.**

| Competitor | Model | Weakness |
|-----------|-------|---------|
| Equinix, Digital Realty | Large urban colocation | Grid energy; PUE 1.4+ [16]; certificate-only green claims |
| iomart | Scottish cloud hosting | Legacy infrastructure; no green product |
| Deep Green | Waste heat data centres | Small scale; cannot match wind curtailment volumes |
| Hyperscalers (AWS, Azure, GCP) | Everything | Require large-scale sites; ignore the small-scale edge gap [19] |

International analogues — Hydro66 (hydropower, Sweden), GreenMountain (fjord-cooled, Norway), Borealis (geothermal, Iceland) — prove the renewable-adjacent data centre model works at scale. The UK market is unserved.

---

## Intellectual Property

**Primary patent candidate:** The WindEdge EMS — a real-time multi-objective optimisation algorithm that controls physical electrical load switching using probabilistic wind forecasts, live turbine SCADA data, grid electricity spot prices, and battery state of charge as simultaneous inputs. The novel contribution is a control architecture that guarantees SLA-level uptime commitments while maximising revenue across four concurrent income streams. A prior art search will be commissioned before filing.

**Additional IP:**
- WINDEDGE trademark registration (UKIPO Classes 38, 42)
- Proprietary real-time carbon attribution methodology (trade secret) — enables per-job Scope 2 reporting for customers
- Site selection model and wind farm partnership playbook (trade secret)

---

## Traction

At concept and pre-incorporation stage. Completed to date:

- Full 5-year financial model and per-site unit economics
- Technical architecture design (electrical topology, EMS specification, connectivity strategy)
- Scottish planning and grid connection regulatory mapping (SSEN process, Scottish PDR analysis)
- IP strategy with patent candidate identified
- Competitive landscape — no direct UK competitor confirmed
- Priority wind farm operator targets identified: SSE Renewables, Vattenfall, RWE
- Anchor tenant prospects identified: EPCC Edinburgh, Scottish Government Digital, NHS National Services Scotland

---

## Team

**Thomas Travis — CEO & Co-Founder**
2nd year PhD student in particle physics at CERN (Imperial College London). Thomas's research is the full Run 3 VBF Higgs-to-invisible analysis — one of the LHC's flagship model-independent dark matter searches. He is introducing machine learning to this analysis for the first time, using a Lorentz-boosted neural network — an architecture that exploits the fundamental symmetry of special relativity as a structural prior — to separate detector noise and physics backgrounds from signal with sensitivity that conventional methods cannot achieve. This requires processing petabytes of collision data across the CERN Worldwide LHC Computing Grid, one of the largest distributed computing infrastructures ever built. He also completed two 5-month internships on Shell's oil trading floor, gaining direct experience in energy commodity markets and how large energy companies structure long-term supply agreements — directly applicable to negotiating wind farm PPAs. Thomas leads commercial strategy, wind farm partnerships, and fundraising.

**Sulayman Awan — CTO & Co-Founder**
2nd year PhD student in particle physics at CERN (Imperial College London). Sulayman's research is a model-agnostic search for anomalous high-multiplicity particle events consistent with SUEPs (Soft Unclustered Energy Patterns), a dark matter candidate class, using a Graph Transformer neural network on raw detector energy deposits combined with ABCDDisco — a pioneering background estimation method. Beyond physics, Sulayman completed two industry internships: quantitative research at Moore Capital on futures strategies and interest rate swaps, and carbon trading strategy at Altana Wealth. The Altana role is directly relevant — Sulayman understands how carbon is priced, structured, and traded at an institutional level, which informs WindEdge's green compute premium, carbon attribution methodology, and positioning in the fast-growing Scope 2 compliance market. He leads EMS algorithm development, the infrastructure platform, and site commissioning.

**Why this team:**
The founding pair covers every domain WindEdge depends on. Thomas brings energy commodity markets expertise from Shell's trading floor and the HPC systems depth of a researcher processing petabytes of collision data on the world's largest computing grid. Sulayman brings novel ML capability — building systems that find signals others miss — alongside carbon markets expertise from Altana Wealth that directly informs how WindEdge prices and structures its green compute product. Together they have worked inside Shell, Moore Capital, and Altana Wealth — three of the most relevant institutions in energy, quantitative finance, and carbon markets. Both are also the exact customer WindEdge serves, giving them first-hand knowledge of what institutions need from compute and why green provenance increasingly drives procurement.

---

## Funding & The Ask

**Seed round target: £2,400,000**

| Use of funds | £ | Basis |
|-------------|---|-------|
| Pilot site: 2 containers (400 kW IT load) | £1,100,000 | Vendor quotes [20] |
| Battery storage (2 MWh) | £400,000 | Vendor quotes [20] |
| Connectivity (fibre / microwave) | £120,000 | Market rates [20] |
| Initial IT infrastructure | £280,000 | Vendor quotes [20] |
| Legal (incorporation, PPA, planning) | £120,000 | Solicitor estimate [20] |
| Working capital (18 months runway) | £380,000 | Salary model [18] |
| **Total** | **£2,400,000** | |

*All capex figures are pre-engagement estimates. Formal quotes will be obtained before committing capital.*

**SEIS/EIS eligible** — UK investors receive 50% (SEIS) or 30% (EIS) income tax relief [21].

**Series A: £18,000,000** (target Month 30) — funds sites 3–12 and GPU cluster inventory [18].

**Exit paths:** Trade sale to hyperscaler or infrastructure fund at Year 6–8; comparable infrastructure transactions typically at 10–18x EBITDA [22].

---

## Immediate Next Steps

1. Approach SSE Renewables and Vattenfall under NDA for curtailment data on specific sites
2. Commission SSEN grid connection pre-application enquiry
3. Engage Scottish planning consultant for PDR assessment on candidate sites
4. Secure anchor tenant LOI (EPCC Edinburgh priority target)
5. File WINDEDGE trademark with UKIPO
6. Commission EMS prior art search before any public disclosure

---

## Sources & Assumptions

### Published Sources

**[1] Scottish wind curtailment volume**
National Grid ESO Balancing Mechanism Reporting System (BMRS): bmrs.elexon.co.uk. Annual curtailment volumes are calculable from the published BM data. Renewable UK and Scottish Renewables also publish annual curtailment summaries. The 900–910 GWh figure for 2023 is consistent with reported figures but **should be verified against the BMRS dataset before use in investor materials.**

**[2] Constraint payments £700m+ (2023)**
National Grid ESO publishes annual constraint cost data. Ofgem also reports on balancing costs in its annual State of the Energy Market report. 2023 was an unusually high year due to elevated gas prices inflating the cost of balancing actions. **Verify the exact figure at nationalgrideso.com or in Ofgem's most recent balancing report.**

**[3] UK data centre electricity cost £100–140/MWh**
Cornwall Insight and Ofgem publish large commercial electricity cost data. The range reflects variation by contract structure, location, and year. This figure includes energy, network charges, and levies. **Verify against Cornwall Insight's most recent commercial tariff tracker.**

**[4] Energy as 40–60% of data centre opex**
Widely cited in Uptime Institute Annual Global Data Centre Survey and Lawrence Berkeley National Laboratory reports on data centre energy use. **Source: Uptime Institute, Annual Global Data Centre Survey (most recent edition).**

**[5] UK Sustainability Disclosure Requirements (SDR) — Scope 2 reporting from 2026**
UK Financial Conduct Authority SDR policy statement PS23/16 and accompanying IFRS S1/S2 alignment. Large listed companies must report from accounting periods beginning on or after 1 January 2026. **Source: FCA PS23/16, gov.uk/government/publications/sustainability-disclosure-requirements.**

**[6] 2,000+ GWh curtailment by 2028**
⚠️ **Author extrapolation** from the 2020–2023 trend. SSEN Transmission's Network Development Plans (NDPs) discuss curtailment growth but the specific 2028 figure is not taken from a published projection. **Replace with the specific SSEN NDP projection if available, or frame as "estimated" in all materials.**

**[7] UK data centre market £5.3bn / 12% CAGR / £9.8bn by 2030**
JLL and CBRE both publish annual UK data centre market reports. The figures cited are consistent with analyst estimates from 2024/2025 reports. **Verify against the most recent JLL or CBRE UK Data Centre Report (available on request from JLL Research).**

**[8] Green compute / green data centre market 19% CAGR**
Grand View Research, "Green Data Center Market Size, Share & Trends Analysis Report." Grand View is a legitimate market research firm but CAGR figures from commercial research firms are indicative. **Cite as: Grand View Research, Green Data Center Market Report, [year]. Note that this is an analyst estimate, not audited data.**

**[9] Grid upgrade completion 2030–2033**
SSEN Transmission's Strategic Development Plans and Ofgem's RIIO-T2 and T3 regulatory frameworks. The Eastern HVDC link and Beauly–Stronelairg reinforcement projects have published completion timelines in this range. **Source: SSEN Transmission Strategic Wider Works programme, ssen-transmission.co.uk.**

**[10] ~85% energy cost advantage**
Calculated figure: (£120/MWh midpoint grid cost − £12/MWh midpoint curtailed wind cost) ÷ £120/MWh = 90%. Presented as "~85%" to be conservative. **This is an author calculation dependent on [3] and [11]. Not a published figure.**

**[11] Curtailed wind PPA rate £5–20/MWh**
⚠️ **Author estimate.** There is no published market price for bilateral behind-the-meter curtailment PPAs because these are private bilateral agreements. The range is based on the economics of curtailment payments (operators are being paid to waste the energy, so any price above zero is better than their alternative) and published PPA market data from LevelTen Energy and Modo Energy. **Must be framed as an estimated range, not a market price, in all materials.**

**[12] NUoS transmission charges £15–25/MWh in Scotland**
Ofgem publishes the Transmission Network Use of System (TNUoS) tariffs annually. Scottish generation zones face some of the highest charges in the UK. **Source: Ofgem TNUoS tariff schedule, ofgem.gov.uk/check-if-energy-price-is-fair/transmission-network-use-of-system-charges.**

**[13] Scotland average ambient temperature ~8°C**
Met Office UK climate averages. Scotland's average annual mean temperature varies by location: Highlands typically 7–9°C, lowlands 9–10°C. 8°C is a reasonable representative figure for Highland wind farm sites. **Source: Met Office UK Climate Averages, metoffice.gov.uk/research/climate/maps-and-data/uk-climate-averages.**

**[14] ~89% free cooling hours**
⚠️ **Author calculation.** Derived from the ASHRAE standard free-cooling threshold (inlet air temperature below ~18°C wet bulb) applied to Met Office climate data for Scottish Highland sites. This is a rough estimate; a formal psychrometric analysis using site-specific hourly Met Office data would be required before use in engineering specifications. **Frame as "estimated" or "subject to site-specific analysis."**

**[15] PUE design target 1.05–1.10**
ASHRAE TC 9.9 guidelines for cold-climate data centres and published case studies from Schneider Electric and Vertiv for free-air-cooled container deployments in northern European climates. GreenMountain (Norway) publishes a PUE of 1.15 for its fjord-cooled facility as a comparable. **This is a design target, not a measured figure. Actual PUE will depend on site conditions and must be verified through commissioning.**

**[16] Industry average PUE 1.58**
Uptime Institute Annual Global Data Centre Survey. The 2023 survey reported a global average PUE of approximately 1.58. **Source: Uptime Institute, Annual Global Data Centre Survey 2023, uptimeinstitute.com. Verify against the most recent survey edition.**

**[17] Cooling energy cost saving £80–120k per MW per year**
⚠️ **Author calculation.** Derived by comparing cooling energy consumption at PUE 1.05–1.10 (5–10% of IT load on cooling) versus PUE 1.4–1.6 (30–40% on cooling) at an assumed electricity cost of £120/MWh, across 1 MW of IT load operating continuously. The range reflects uncertainty in the energy price and PUE assumptions. **This is an illustrative calculation, not a quoted figure.**

**[18] Unit economics, financial model, and all derived financial figures**
⚠️ **Author model.** All financial projections — revenue per site, EBITDA margin, 5-year P&L, payback period, portfolio revenue targets — are outputs of an internal financial model built by the founding team. Key assumptions: colocation price £170/kW/month, 70% utilisation at steady state, curtailed wind at £15/MWh, grid backup at £100/MWh for 10% of hours. These assumptions have not been validated against operational data and will change materially as the business develops. **Do not present as forecasts; present as model outputs subject to assumptions.**

**[19] Hyperscaler minimum site scale**
Industry knowledge based on publicly reported hyperscaler data centre projects. AWS, Google, and Microsoft typically develop campuses of 100MW+ and have not publicly announced sub-10MW co-location arrangements. **No single citable source; this is an industry observation.**

**[20] Capex figures (containers, battery, connectivity, legal)**
⚠️ **Pre-engagement estimates.** Container data hall costs are based on published vendor pricing from Schneider Electric and Vertiv for comparable specifications. Battery costs are based on published Tesla Megapack and CATL pricing (approximately £150–200/kWh installed, 2024). Legal estimates are based on solicitor conversations. **All capex figures require formal quotes before being used in funding materials.**

**[21] SEIS/EIS tax relief rates**
HMRC published guidance: 50% income tax relief for SEIS, 30% for EIS. SEIS limit £250,000 per company; EIS limit £5,000,000 per year. **Source: HMRC SEIS and EIS guidance, gov.uk/guidance/seed-enterprise-investment-scheme-background.**

**[22] Exit multiples 10–18x EBITDA**
⚠️ **Author estimate** based on publicly reported data centre infrastructure transactions. Infrastructure funds typically apply 12–18x EBITDA for stabilised assets; strategic acquirers have paid higher multiples in competitive processes. The range is illustrative and actual exit multiples will depend on market conditions at the time of exit. **No single source; treat as a directional estimate.**

---

*WindEdge Data Centres Ltd — Confidential*
*Contact: Thomas Travis — [YOUR EMAIL]*
*June 2026*
