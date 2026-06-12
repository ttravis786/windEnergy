# WindEdge Data Centres
## Comprehensive Business Plan
### Version 1.0 — May 2026

---

> *Turning Scotland's wasted wind into the world's greenest compute.*

---

## Table of Contents

1. [Executive Summary](#1-executive-summary)
2. [Company Overview](#2-company-overview)
3. [The Problem & Market Opportunity](#3-the-problem--market-opportunity)
4. [The Solution](#4-the-solution)
5. [Market Analysis](#5-market-analysis)
6. [Business Model & Revenue Streams](#6-business-model--revenue-streams)
7. [Technical Architecture](#7-technical-architecture)
8. [Operations Plan](#8-operations-plan)
9. [Go-to-Market Strategy](#9-go-to-market-strategy)
10. [Financial Model](#10-financial-model)
11. [Team & Hiring Plan](#11-team--hiring-plan)
12. [Funding Requirements](#12-funding-requirements)
13. [Risk Register & Mitigation](#13-risk-register--mitigation)
14. [Regulatory & Legal Framework](#14-regulatory--legal-framework)
15. [Sustainability & ESG](#15-sustainability--esg)
16. [Exit Strategy](#16-exit-strategy)
17. [Appendices](#17-appendices)

---

## 1. Executive Summary

### The Business

WindEdge Data Centres Ltd's **primary model is a build-and-manage service**: WindEdge designs and commissions modular GPU data centres (100 kW, ~60 GPUs) for clients — wind farm operators, landowners, and private investors — charging a fixed build fee and a 10% ongoing management fee for running the EMS algorithm and GPU marketplace. Clients own the hardware; WindEdge provides the expertise. As the company generates revenue and establishes track record, an **alternative path opens**: WindEdge builds and owns facilities directly at the highest-curtailment sites, capturing 100% of revenue. This owned-facility path can be reached either through accumulated build-and-manage revenue or, if appropriate, a seed raise to accelerate it.

### The Insight

Scotland curtailed **over 900 GWh of wind electricity in 2023** — power that was generated and immediately discarded because the transmission grid could not carry it south. Wind farm operators were paid **over £700 million** in constraint payments that year to switch their turbines off. This is not an edge case; curtailment is structurally worsening as Scotland's wind capacity grows far faster than grid upgrade timelines. The key insight is that the energy cost advantage — accessing curtailed wind at an estimated £5–20/MWh versus £100–140/MWh on the grid — dramatically improves the economics of GPU compute, creating a product that is both cheaper and greener than any grid-connected competitor.

### The Phased Approach

- **Phase 0 (now)**: Buy 4 RTX 5090 GPUs (~£2,500 each = ~£10,000 total), list on Vast.ai and RunPod. Estimated ~$0.40/GPU/hour net (minus electricity cost and 25% Vast.ai fee) at 85% occupancy = ~£9,400/year. Proves the GPU marketplace model with real data before approaching wind farm operators or investors.
- **Phase 1 (Year 1–2)**: Build-and-manage service. Clients fund the hardware; WindEdge charges a build fee (£40–80k) and 10% of ongoing GPU revenue. Asset-light, fast to scale.
- **Phase 2 (Year 2–3)**: Own 2–3 facilities directly at the highest-curtailment Scottish sites, capturing 100% of GPU revenue. Two routes: (a) funded from accumulated build-and-manage revenue, or (b) a seed raise (£300–600k) to reach this point faster.
- **Phase 3 (Year 3+)**: Mixed portfolio — managed facilities provide steady recurring income; owned facilities generate the majority of profit.

### The Ask

WindEdge's primary path to owned facilities is through accumulated build-and-manage revenue — no external capital required to reach Phase 2. An alternative is to raise **£300,000–600,000** in seed funding after the Phase 0 pilot to accelerate directly to an owned facility, compressing the timeline without waiting for managed revenue to accumulate. Either path reaches the same destination; the raise simply gets there faster.

### Headline Numbers (5-Year Forecast, Author Model)

| Metric | Year 1 | Year 2 | Year 3 | Year 5 |
|--------|--------|--------|--------|--------|
| Managed facilities | 0 | 3 | 10 | 30 |
| Owned facilities | 0 | 1 | 2 | 5 |
| Build fee revenue | £0 | £180k | £600k | £1,125k |
| Recurring managed revenue (10%) | £0 | £45k | £250k | £900k |
| Owned facility revenue | £0 | £180k | £400k | £1,500k |
| **Total Revenue** | **~£9.4k*** | **~£405k** | **~£1,250k** | **~£3,525k** |
| Headcount | 2 | 4 | 10 | 25 |

*Phase 0 pilot net GPU revenue only (4 × RTX 5090, ~$0.40/GPU/hour net at 85% occupancy). All figures are author model estimates — see Appendix F.*

---

## 2. Company Overview

### Vision

Some notes. Assume curtailed energy is free the payback time of a battery is 3 years (600k per 2MWh)

A world where compute infrastructure is no longer a driver of climate change, but is powered entirely by energy that would otherwise go to waste.

### Mission

To build the UK's most cost-efficient and genuinely sustainable compute network by co-locating modular data centres with Scottish wind infrastructure.

### Legal Structure

- **Entity**: WindEdge Data Centres Ltd
- **Incorporation**: Companies House, Scotland
- **Registered office**: Edinburgh (TBC)
- **Structure**: Private limited company, converting to PLC at Series B if pursuing public markets
- **Subsidiaries**: WindEdge Energy Ltd (holds PPAs and grid contracts separately from compute operations — cleaner for investors and regulatory purposes)

### Values

1. **Radical transparency** — every customer gets a real-time carbon dashboard; no greenwashing
2. **Reliability first** — renewable does not mean unreliable; uptime is non-negotiable
3. **Fair partnership** — wind farm operators share in upside, not just lease income
4. **Scottish-first hiring** — remote and island communities get jobs, not just infrastructure

---

## 3. The Problem & Market Opportunity

### 3.1 The Curtailment Crisis

Scotland is one of the windiest territories in Europe. As of 2025, Scotland has approximately 15 GW of installed wind capacity — onshore and offshore — representing around 30% of the UK's total. The Scottish Government's target is to reach the equivalent of 100% of Scotland's electricity demand from renewables by 2030.

The problem is structural: **electricity generation capacity has grown far faster than transmission infrastructure**. The network bottleneck is primarily the Anglo-Scottish interconnector — the high-voltage lines that carry power from Scotland to English demand centres. When these lines are congested (which is increasingly frequent), National Grid ESO instructs Scottish wind farms to curtail — to switch off or reduce output — while simultaneously paying gas and coal plants in England to generate instead. This is called "constraint balancing."

**The scale of this waste:**

| Year | Scottish Wind Curtailment | Constraint Cost to Bill Payers |
|------|--------------------------|-------------------------------|
| 2020 | 480 GWh | £283m |
| 2021 | 612 GWh | £401m |
| 2022 | 780 GWh | £594m |
| 2023 | 910 GWh | £703m |
| 2024 (est.) | 1,050+ GWh | £800m+ |

This trend will worsen. SSEN's own modelling projects that without significant grid investment (completion dates 2030–2033 at earliest), curtailment will reach 2,000+ GWh annually by 2028.

**The curtailment is not evenly distributed.** Specific wind farms — particularly in the Highlands and Islands — are curtailed for 30–60% of their potential generation hours. These are precisely the sites where WindEdge deploys.

### 3.2 The Data Centre Energy Problem

Energy is the dominant operating cost in conventional data centres, typically representing 40–60% of total opex. UK grid electricity for large commercial consumers runs at approximately £80–120/MWh depending on contract structure, plus balancing charges, network use of system (NUoS) charges, and climate change levies.

Large hyperscalers (AWS, Google, Microsoft) have negotiated bespoke PPAs that reduce their effective rate to £40–60/MWh. Smaller operators pay full rate. WindEdge can access curtailed wind at **£5–20/MWh** through direct bilateral agreements with wind farm operators — energy the operators would otherwise be paid to waste.

The elimination of transmission charges is equally important. Grid-connected consumers pay NUoS charges that vary by region but in Scotland can reach £15–25/MWh on top of energy cost. WindEdge, consuming behind the substation meter, pays **zero transmission charges**.

**Effective all-in energy cost comparison:**

| Operator type | Effective energy cost/MWh |
|--------------|--------------------------|
| Typical UK colocation | £100–140 |
| Hyperscaler with PPA | £55–75 |
| **WindEdge (curtailed wind)** | **£15–35** |

This creates an **85–90% energy cost advantage** that is structural, not cyclical.

### 3.3 The Green Compute Premium

Enterprise sustainability reporting is no longer voluntary. The UK's Sustainability Disclosure Requirements (SDR), aligned with IFRS S1/S2, require large companies to report Scope 2 emissions (electricity consumption) from 2026. The EU's CSRD affects UK companies with EU operations. This regulatory pressure is creating genuine willingness to pay for compute that demonstrably reduces Scope 2 emissions.

The key distinction is **quality of green claims**:

- **Renewable Energy Certificates (RECs/REGOs)**: A company buys certificates representing renewable generation somewhere in the grid, at some time, and claims their consumption is "green." This is widely criticised as greenwashing because the certificates may represent wind power generated in summer while the data centre runs on coal in winter.
- **24/7 Carbon-Free Energy (CFE)**: Matching consumption to generation on an hourly basis. Google and Microsoft have committed to this standard.
- **At-source direct wire**: WindEdge's model — the electrons running through the server literally came from the turbine 200 metres away. This is the strongest possible green claim and cannot be replicated by grid-connected operators at any price.

Research by LevelTen Energy and Wood Mackenzie consistently finds that enterprise buyers will pay **10–25% premium** for verifiable at-source renewable compute versus grid-connected competitors with certificate-based claims.

---

## 4. The Solution

### 4.1 The Core Concept

WindEdge deploys containerised, modular data centres at wind farm substations. Each site consists of:

- One or more **data hall containers** (20–40ft shipping container form factor, purpose-built)
- **Battery energy storage** to buffer wind intermittency
- A **direct electrical connection** to the wind farm's MV/LV substation
- A **grid tie-in** as backup power and for selling excess capacity as demand response
- **Dark fibre or microwave backhaul** to the nearest internet exchange or carrier PoP

The data centre consumes power that would otherwise be curtailed. When curtailment is not occurring and power is grid-priced, the flexible load (cryptocurrency mining / AI training queues) is reduced, and the site draws minimally from the grid — maintaining uptime for colocation customers.

### 4.2 Why Containers

Modular containerised data centres have matured significantly. Companies like Schneider Electric, Vertiv, and purpose-built Scottish suppliers like Data Centre Systems now produce Tier 3-equivalent IT environments in 20–40ft containers:

- **Planning speed**: Containers on existing industrial/wind farm land typically fall under permitted development rights or Class 6 prior approval (Scotland), avoiding full planning applications
- **Relocatability**: If a wind farm decommissions or a better site emerges, the asset moves
- **Scalability**: Add containers as demand grows; no stranded large-scale build
- **Financing**: Each container is a discrete, mortgageable asset — simpler for lenders
- **Speed to market**: 12–16 weeks from order to operational versus 18–36 months for a traditional build

### 4.3 The Flexible Load Architecture

The key innovation is the **load hierarchy** that makes intermittent wind compatible with commercial SLAs:

```
Power availability (high) ──► Priority 1: Colocation customers (always on, SLA-protected)
                               Priority 2: Managed HPC jobs (can be paused/rescheduled)
                               Priority 3: GPU training workloads (queued, delay-tolerant)
                               Priority 4: Crypto mining (instant-off, absorbs all surplus)
Power availability (low)  ──► Shed Priority 4 → 3 → 2, never touch Priority 1
```

Battery storage (2–4 MWh per site) bridges gaps of 15–60 minutes — sufficient for most wind variability events. The grid tie-in covers extended low-wind periods. The result is **>99.9% uptime** for colocation customers despite being located at a wind farm.

### 4.4 The Customer Value Proposition

**For enterprise colocation customers:**
- 10–25% below-market pricing driven by energy cost advantage
- PUE of 1.05–1.10 (world-class; most UK providers are 1.4–1.6)
- Verifiable at-source renewable power with real-time dashboard
- Contributes directly to Scope 2 zero — not just offsets

**For HPC / AI compute customers:**
- Managed GPU clusters at lower cost than hyperscaler equivalents
- Green compute credentials for AI ESG reporting
- Scottish location advantageous for data sovereignty (UK jurisdiction, GDPR compliant)

**For wind farm operators (partners, not just landlords):**
- Additional revenue from otherwise-curtailed energy
- Potential revenue share or equity stake in WindEdge
- Grid services income (demand response contracts improve their own grid relationship)
- Local employment and community benefit

---

## 5. Market Analysis

### 5.1 Total Addressable Market (TAM)

The UK data centre colocation market was valued at **£5.3 billion in 2024** and is projected to grow at 11–13% CAGR to reach **£9.8 billion by 2030** (JLL, Cushman & Wakefield, 2025 reports). Drivers include:

- AI/ML workload explosion — training and inference compute demand tripling every 18 months
- Public sector cloud migration under GDS mandates
- Financial services regulatory requirements for UK-domiciled data
- Edge computing proliferation (sub-20ms latency requirements for IoT, autonomous systems)

Globally, the green data centre market specifically is projected at **$140 billion by 2030** (Grand View Research), growing at 19% CAGR — significantly faster than the overall market.

### 5.2 Serviceable Addressable Market (SAM)

WindEdge's initial SAM is defined by:
- UK enterprises with active Scope 2 reduction targets (FTSE 350, large private companies)
- Public sector bodies under government net-zero mandate
- AI/ML companies needing cost-effective GPU compute
- Scottish and Northern English enterprises preferring low-latency local hosting

This segment represents approximately **£1.2 billion** of the UK colocation market.

### 5.3 Serviceable Obtainable Market (SOM)

A realistic 5-year target of **£8–12 million annual revenue** represents under 1% of SAM — highly achievable with 20 operational sites. This is a land-grab opportunity; there is no direct competitor currently executing this model in the UK.

### 5.4 Competitive Landscape

| Competitor | Model | Weakness vs. WindEdge |
|-----------|-------|----------------------|
| Equinix, Telehouse | Large-scale urban colo | Grid energy, high PUE, no green premium |
| Digital Realty | Hyperscale campuses | Grid energy, 18–36 month build times |
| Kao Data | UK sustainable DC | Grid + REGOs only, not at-source |
| iomart | Scottish cloud provider | Legacy infrastructure, high PUE |
| Hyperscalers (AWS, Azure, GCP) | Everything | Need 100MW+ sites; ignore <5MW gaps |
| Blockchain/crypto miners at wind farms | Flexible load only | No colocation product; no network |

**Direct competitors executing WindEdge's model in Scotland: zero.**

There are analogues in Iceland (geothermal-adjacent compute) and Norway (hydro-adjacent), but the UK market is unserved. The first mover who builds customer relationships and wind farm partnerships erects a durable barrier: wind farm operators will not sign with two competing data centre companies for the same turbine cluster.

### 5.5 Target Customer Segments

**Segment 1: Enterprise Sustainability-Driven Colocation**
- Profile: FTSE 350 companies, financial services, law firms, consultancies with active Scope 2 targets
- Buying trigger: Board-level ESG commitments, incoming SDR reporting requirements
- Deal size: £50k–£500k/year
- Sales cycle: 6–12 months
- Priority targets: Standard Life Aberdeen, Baillie Gifford, Wood Group, Sky, Channel 4 (Scottish ops)

**Segment 2: Public Sector / Government**
- Profile: Scottish Government, NHS Scotland, universities, MOD
- Buying trigger: Crown Commercial Service green procurement frameworks, data sovereignty requirements
- Deal size: £100k–£2m/year (multi-year contracts)
- Sales cycle: 12–24 months (procurement processes)
- Priority targets: Scottish Government Digital, University of Edinburgh (EPCC), NHS National Services Scotland

**Segment 3: AI / HPC Compute Renters**
- Profile: AI startups, research institutions, film/VFX studios, financial quant teams
- Buying trigger: GPU scarcity, cost of hyperscaler GPU instances, green AI narrative
- Deal size: £20k–£300k/year
- Sales cycle: 2–6 months
- Priority targets: Skyscanner, Intelligent Growth Solutions, Edinburgh AI cluster, Heriot-Watt

**Segment 4: Telecoms / Edge**
- Profile: BT, Vodafone, Virgin Media O2 needing distributed edge nodes
- Buying trigger: 5G edge compute rollout, O-RAN disaggregation
- Deal size: £200k–£1m/year per site
- Sales cycle: 18–36 months
- Priority targets: BT Wholesale, Vodafone Business

**Segment 5: Private Investors / Asset Owners**
- Profile: High-net-worth individuals, family offices, angels, small funds who want exposure to the AI infrastructure asset class but cannot afford a hyperscale data centre (£50m+)
- Buying trigger: A 100 kW facility at ~£200–350k all-in is an accessible, tangible asset that generates monthly GPU income with no operational involvement; renewable infrastructure also appeals to ESG-conscious private capital
- Deal size: One facility per client (~£200–350k capex funded by investor); WindEdge earns the build fee + 10% ongoing revenue share
- Sales cycle: 1–3 months (faster than enterprise; decision is personal capital not committee approval)
- Priority targets: Tech-sector angels, energy-sector family offices, property investors seeking yield from a new asset class
- Why it works: The investor funds the hardware; WindEdge provides the expertise, algorithm, and marketplace relationships. The investor owns a real, depreciating asset generating real cash flow — not a software licence.

---

## 6. Business Model & Revenue Streams

WindEdge operates a three-stream model that evolves in phases. All financial figures below are author model estimates and have not been validated against operational data — see Appendix F.

### 6.1 Stream A: Phase 0 Pilot — GPU Marketplace (Bootstrapped)

Before approaching any investors or wind farm operators, WindEdge validates the GPU revenue model with a small self-funded pilot.

- **Hardware**: 4 × NVIDIA RTX 5090 GPUs (~£2,500 each = ~£10,000 total)
- **Platforms**: Vast.ai, RunPod — list GPUs for rent by the hour on the open marketplace
- **Estimated net revenue**: ~$0.40/GPU/hour net (minus electricity cost and 25% Vast.ai fee) at 85% occupancy [🔴 benchmarked against current Vast.ai listings — verify before committing]
- **Estimated annual net revenue (4 GPUs)**: ~£9,400/year
- **Purpose**: Proves GPU marketplace revenue with real operational data before any wind farm build
- **Customer escalation**: Start on anonymous marketplace (no sales effort); use revenue data to move to direct contracted relationships with tech startups, university research computing teams, and AI companies needing reserved capacity

### 6.2 Stream B: Build-and-Manage Service (Asset-Light, Scalable)

WindEdge designs, commissions, and manages 100 kW modular GPU data centres for clients. The client owns the hardware; WindEdge provides the expertise and the ongoing management.

**What WindEdge delivers:**
1. Standard 100 kW facility design (container, battery, electrical connection, networking)
2. EMS algorithm — optimises battery charge/discharge between wind, grid, and GPU load in real time
3. GPU marketplace management — listing, dynamic pricing, uptime monitoring across Vast.ai / RunPod etc.
4. NOC remote monitoring from Edinburgh
5. Regular performance reporting and algorithm updates

**Revenue per managed facility:**

| Item | Amount | Timing |
|------|--------|--------|
| Build fee (design, project management, commissioning) | £40,000–80,000 | One-off on completion |
| Ongoing revenue share | 10% of gross GPU revenue | Monthly |

**Estimated ongoing revenue per 100 kW managed facility:**
- ~60 RTX 5090-class GPUs
- Estimated GPU revenue: £120,000–350,000/year [🔴 highly variable — depends on GPU model, platform rates, and utilisation. Verify on Vast.ai before presenting to clients]
- WindEdge 10% share: **£12,000–35,000/year per facility** [🔴 author estimate]

**Why clients pay:**
Without WindEdge, a wind farm operator or landowner with a substation and some land cannot convert that into GPU revenue. WindEdge provides the entire stack — design, build, algorithm, marketplace. The 10% fee buys them a passive income stream with no operational involvement.

### 6.3 Stream C: Owned Facilities (High Margin, Long-Term)

At the 2–3 highest-curtailment wind sites, WindEdge owns and operates facilities directly, capturing 100% of GPU revenue rather than 10%. These are funded from accumulated build fees and a small equity raise.

**Unit economics per owned 100 kW facility (steady state):** [🔴 all author estimates]

| Item | Annual |
|------|--------|
| GPU revenue (~60 GPUs, 70% util) | £150,000–300,000 |
| Energy cost (curtailed wind, estimated £15/MWh) | £13,000 |
| Energy cost (grid backup, 10% hours) | £8,000 |
| Connectivity | £18,000 |
| Site lease | £12,000 |
| O&M | £15,000 |
| **EBITDA** | **£84,000–234,000** |

*Wide range reflects uncertainty in GPU pricing and utilisation. Phase 0 pilot data will narrow this significantly.*

### 6.4 Why This Structure Is Better Than Full Asset Ownership

| | Original model | New model |
|--|---------------|-----------|
| Capital to start | £2,400,000 | ~£25,000 |
| Time to first revenue | 18+ months | Weeks |
| Hardware risk | WindEdge | Client (managed stream) |
| Revenue per facility | 100% | 10% managed / 100% owned |
| Scale mechanism | Raise equity | Build fees fund next build |
| Proof of concept | Requires investor capital | Self-fundable |

---

## 7. Technical Architecture

### 7.1 Site Selection Criteria

Not every wind farm is suitable. WindEdge uses a scoring matrix:

| Criterion | Weight | Ideal |
|-----------|--------|-------|
| Curtailment rate | 30% | >30% of generation hours curtailed |
| Distance to fibre PoP | 25% | <30km from BT or Jisc PoP |
| Road access | 15% | HGV-accessible year-round |
| Grid connection capacity | 15% | Substation capacity for 5+ MW |
| Wind farm operator relationship | 15% | Operator with existing commercial flexibility |

**Candidate sites (initial research):**

- Bhlaraidh Wind Farm (Glen Moriston) — SSE Renewables, high curtailment, near A82
- Corriegarth Wind Farm (Strathdearn) — SSE Renewables, 130 MW, Inverness-adjacent fibre
- Viking Wind Farm (Shetland) — Vattenfall, highest curtailment in UK, unique island edge case
- Clyde Wind Farm (Lanarkshire) — ScottishPower Renewables, excellent motorway access, Glasgow fibre proximity
- Stronelairg Wind Farm (Inverness-shire) — SSE Renewables, 228 MW, known high curtailment

### 7.2 Electrical Architecture

```
Wind Turbines
     │
     ▼
MV Collector Substation (33kV)
     │
     ├──► [Grid Export] ──► National Grid (when not curtailed)
     │
     └──► [WindEdge Connection] ──► Site Substation (11kV/400V)
               │
               ├──► Battery Storage System (2–4 MWh, CATL/Tesla Megapack)
               │
               ├──► Grid Tie-In (backup, demand response)
               │
               └──► IT Load Distribution (UPS → PDU → Rack)
```

**Key electrical design decisions:**

- **Connection voltage**: 11kV step-down to 400V (3-phase) — standard for container DC
- **UPS**: Double-conversion online UPS, N+1 redundancy per container
- **Battery sizing**: Target 60-minute bridge at full load; covers >95% of wind lull events
- **Generator backup**: Diesel genset on standby for extended outages (grid + battery failure)
- **Power metering**: Revenue-grade sub-metering per rack for customer billing and green reporting

### 7.3 Data Hall Containers

**Specification (per 20ft container module):**

| Parameter | Specification |
|-----------|-------------|
| IT load capacity | 200 kW |
| Cooling type | Direct air-cooled (fresh air economisation) |
| PUE target | 1.05–1.10 |
| Rack density | 10 kW average, 30 kW max |
| Rack count | 20 x 42U racks |
| Connectivity | 2 x 100GbE uplinks, IB fabric for HPC |
| Physical security | ISO 27001-aligned, CCTV, biometric access, mantrap |
| Fire suppression | Novec 1230 clean agent |
| Operating temp | 18–27°C (ASHRAE A2 class) |
| Humidity | 20–80% RH |
| Seismic | Rated for Scottish ground conditions |
| IP rating | IP55 for external components |

**Cooling strategy:**

Scotland's average annual ambient temperature of ~8°C enables free air cooling (economisation) for the majority of the year. A psychrometric analysis of Scottish Highland sites shows:

- **Free cooling hours**: ~7,800 of 8,760 annual hours (89%)
- **Mechanical cooling hours**: ~960 hours (11%), primarily July–September
- **Result**: Cooling energy represents only ~5–10% of IT load (PUE 1.05–1.10) vs. 30–40% for conventional sites (PUE 1.4+)

This alone saves **£80–120k per MW per year** in energy cost versus a London or Manchester facility.

### 7.4 Connectivity Architecture

Connectivity is the primary technical challenge for remote Scottish sites. WindEdge's tiered approach:

**Tier 1: Dark fibre (preferred)**
- Negotiate IRU or lease on existing BT Openreach, SSE fibre, or Jisc Janet routes
- Typical rural Scottish fibre: £500–2,000/month for 1GbE; £2,000–8,000/month for 10GbE
- Latency to Edinburgh: 10–40ms depending on site

**Tier 2: Microwave point-to-point**
- For sites >30km from fibre, licensed microwave (10–80 GHz) provides 1–10 GbE
- Cost: £15,000–40,000 capex per link, £500–1,500/month spectrum licence
- Latency impact: +1–3ms per hop

**Tier 3: Starlink Business (emergency/management)**
- Used for out-of-band management only (IPMI, KVM-over-IP, DCIM)
- 150–300 Mbps, high latency — unsuitable for customer traffic
- Cost: £140/month per site; no long-term commitment

**Connectivity redundancy:**
- All sites must have at least two independent connectivity paths
- Automatic failover via BGP with 30-second convergence target
- Management plane always on separate OOB path

### 7.5 Data Centre Infrastructure Management (DCIM)

WindEdge will deploy a purpose-built DCIM platform (based on open-source OpenDCIM / Netbox with custom energy management layer) providing:

- Real-time power draw per rack, per customer
- Carbon intensity dashboard (gCO2/kWh, updated every 5 minutes)
- Wind forecast integration (Met Office API) for load planning
- Automated load shedding / restoration sequences
- Customer-facing portal with live sustainability metrics
- API integration with National Grid ESO for demand response dispatch

---

## 8. Operations Plan

### 8.1 Operational Model

WindEdge operates a **hub-and-spoke model**:

- **Hub (Edinburgh)**: Central NOC, sales, finance, engineering, software
- **Regional clusters**: Sites grouped geographically with a Regional Operations Manager per 5-site cluster
- **Wind farm partner staff**: Local wind farm O&M teams trained to provide basic hands-on support (hardware swap, visual inspection) under SLA

This model keeps headcount lean. A 20-site portfolio can be operated by ~45 people, compared to 150+ for a traditional multi-site colocation provider.

### 8.2 Standard Operating Procedures

**Site construction and commissioning (per site):**
1. Weeks 1–4: Electrical connection design, grid application, planning pre-application
2. Weeks 5–16: Container manufacture and fit-out (off-site)
3. Weeks 17–20: Site groundworks, cable laying, substation connection
4. Weeks 21–24: Container delivery, crane placement, power-up
5. Weeks 25–28: IT infrastructure installation, connectivity commissioning
6. Week 29: Customer acceptance testing, go-live

Total: ~7 months from contract to customer go-live per site.

**Ongoing operations:**
- 24/7 remote monitoring from Edinburgh NOC
- Automated alerting and self-healing where possible (power management, cooling)
- Monthly physical inspection by Regional Ops Manager
- Quarterly full audit (power, connectivity, physical security, fire systems)
- Annual third-party audit for ISO 27001 / SOC 2 Type II compliance

### 8.3 Energy Management

Energy management is WindEdge's core operational differentiator. The Energy Management System (EMS) runs continuously:

1. **Forecast**: Pull 72-hour wind forecast from Met Office and wind farm SCADA
2. **Schedule**: Pre-schedule flexible loads (GPU training queues, mining) to match forecast generation
3. **Dispatch**: Real-time load control — automated relay switching within 500ms
4. **Report**: Generate carbon and energy reports for customers and grid operators
5. **Optimise**: ML model continuously improves forecast accuracy and load scheduling

### 8.4 Customer Onboarding

**Colocation:**
- Remote hands provisioning: rack, cable, power, IP allocation
- Cross-connect provisioning: 1–5 business days
- Customer portal access: self-service after onboarding call
- Dedicated account manager for customers >100 kW

**Managed HPC:**
- GPU cluster provisioning: 24–48 hours
- Kubernetes/SLURM job scheduler access
- API-first: customers integrate via REST or CLI

### 8.5 Maintenance and Hardware Refresh

- Hardware refresh cycle: 4–5 years for servers, 8–10 years for containers, 10–15 years for electrical infrastructure
- Spares holding: critical components (drives, NICs, PSUs) held at regional hub
- Vendor support: Dell ProSupport, APC/Schneider Electric service contracts
- End-of-life: Full WEEE-compliant recycling; documented chain of custody for data destruction

---

## 9. Go-to-Market Strategy

### 9.0 Phase 0 — Bootstrap (Now, Before Any Funding)

**Objective**: Prove GPU marketplace revenue with self-funded pilot. Generate real data to de-risk the investor conversation.

**Actions:**
- Purchase 4 × RTX 5090 GPUs (~£2,500 each = ~£10,000 total)
- Register as a provider on Vast.ai and RunPod
- Run GPUs 24/7, monitor utilisation and revenue per GPU-hour
- Document everything: uptime, revenue, customer types, demand patterns
- Target: 3 months of operational data showing real $/GPU/hour and utilisation rates

**Customer escalation during Phase 0:**
- Months 1–3: Anonymous marketplace listings on Vast.ai / RunPod (zero sales effort — price competitively and let the platform bring customers)
- Months 3+: Use real revenue data to approach direct clients — tech startups needing reserved GPU capacity, university research computing teams, AI companies wanting contracted uptime guarantees rather than marketplace availability
- Year 2+: Contracted enterprise and institutional customers who need verifiable green provenance and SLA commitments that marketplace listings cannot provide

**Success metric**: Real revenue data that validates (or refutes) the GPU marketplace model before approaching wind farm operators or investors.

### 9.1 Phase 1 — Prove It (Months 1–18)

**Objective**: First managed-service client signed; first wind farm PPA in progress; Phase 0 pilot data in hand.

**Activities:**

*Using Phase 0 pilot data (Months 1–3):*
- Present real GPU revenue data to first prospective client (wind farm operator or landowner)
- The pitch: "Here is what 10 GPUs earned per month on Vast.ai. Here is what 60 GPUs at your site, on curtailed wind, would earn — and what you keep after our 10% fee."

*First managed facility build (Months 4–12):*
- Sign build agreement and 10% revenue share contract with first client
- Deliver 100 kW facility: container, battery, electrical connection, networking
- Commission EMS algorithm; integrate with wind farm SCADA
- List client's GPUs on Vast.ai / RunPod under management

*Second managed facility (Months 10–18):*
- Use build fee income from Facility 1 to fund operations during Facility 2 build
- Refine standard design; reduce build time

**Phase 1 success metrics:**
- Phase 0 pilot generating measurable GPU revenue (real figure, not a model)
- One managed facility operational with client GPU revenue flowing
- One wind farm PPA agreed at <£20/MWh (estimated)
- WindEdge revenue (build fee + 10% share): >£60,000

### 9.2 Phase 2 — Scale (Months 18–42)

**Objective**: 6 sites operational; managed GPU product launched; Series A fundraise

**Activities:**

*Site rollout:*
- Sites 3–6: Apply learnings from pilot; reduce build timeline to 5 months
- Geographic spread: 2 Highland, 1 Borders, 1 island (Orkney or Shetland)
- Target second wind farm operator partnership

*Product expansion:*
- Launch managed GPU cluster (H100 nodes) — target AI/ML customers
- Launch demand response product — register with National Grid ESO
- Launch customer sustainability dashboard (API access for ESG reporting)

*Sales and marketing:*
- Hire dedicated enterprise sales team (2 AEs)
- Attend Scottish Tech Summit, Data Centre World, Climate Tech VC conferences
- Case study publication with anchor customers
- Target public sector frameworks (Crown Commercial Service, Scotland Excel)

*Fundraise:*
- Series A: £18 million (target close Month 30)
- Use: Sites 7–12, GPU inventory, NOC expansion, sales team

### 9.3 Phase 3 — Platform (Months 42–60+)

**Objective**: 20 sites; distributed compute platform; acquisition conversations

**Activities:**

*Platform product:*
- Launch "WindEdge Cloud" — compute-as-a-service API compatible with AWS/GCP interfaces
- Enable hyperscaler overflow — white-label capacity to Microsoft Azure or similar
- Develop proprietary AI inference product (latency-sensitive workloads, UK data residency)

*Geographic expansion:*
- Evaluate Welsh wind (Pen y Cymoedd, Mynydd y Gwair)
- Evaluate Irish wind (interconnector arbitrage opportunity)

*M&A and partnerships:*
- Strategic partnership with BT for network integration
- Acquisition of small Scottish managed service provider for customer base

### 9.4 Sales Strategy

**Direct enterprise sales:**
- Primary channel for Year 1–3
- Target: CTO, Head of Infrastructure, Head of Sustainability (often separate buyers who need to align)
- Sales cycle: 6–18 months for enterprise; 2–6 months for SME/startup

**Channel partnerships:**
- IT resellers and MSPs (Computacenter, Softcat — both have Scottish presence)
- Sustainability consultancies (advise clients on Scope 2 solutions)
- Law firms and financial advisers (introduce clients with data needs)

**Government and public sector:**
- Register on Crown Commercial Service G-Cloud framework
- Scotland Excel supplier registration
- Direct relationship with Scottish Enterprise (also a potential grant funder)

**Digital marketing:**
- SEO targeting "green data centre Scotland", "sustainable colocation UK", "renewable compute"
- LinkedIn thought leadership content (curtailment explainers, Scope 2 guides)
- No paid advertising in Year 1 — budget better spent on events and direct outreach

### 9.5 Pricing Strategy

| Product | Price | Rationale |
|---------|-------|-----------|
| Colocation (kW/month) | £155–185 | 10–15% below UK market; above breakeven even at 50% utilisation |
| Managed GPU (H100/hour) | £3.50–5.50 | 40–50% below AWS/Azure equivalent |
| Bare metal server (1U/month) | £200–350 | Market rate; green premium justified |
| Connectivity (1GbE/month) | £300–800 | Market rate; cross-connect fees standard |
| Demand response (kW capacity) | Auction-based | National Grid ESO market rate |

---

## 10. Financial Model

### 10.1 Key Assumptions

**Revenue assumptions:**
- Average selling price: £170/kW/month (colocation)
- Utilisation ramp: 30% (Month 1) → 70% (Month 18) → 80% (Month 36+) per site
- GPU revenue starts Year 3; assumed 60% utilisation at £4.50/GPU-hr
- Demand response revenue: £25,000/site/year from Year 3

**Cost assumptions:**
- Energy (curtailed wind): £15/MWh average across portfolio
- Energy (grid backup, 10% of hours): £100/MWh
- Connectivity: £4,000/month/site average (mix of fibre and microwave)
- Site lease: £2,000/month/site
- Staff costs: fully loaded including NI, pension

**Capex assumptions:**
- Container (200 kW IT, fitted): £400,000 per unit
- Battery storage (2 MWh): £400,000 per site
- Electrical connection works: £150,000 per site
- Networking/backhaul: £80,000 per site
- IT hardware (servers, GPUs, networking): £500,000 per MW of IT load
- Total capex per 100 kW managed facility (client-funded): ~£200,000–350,000
- Total capex per 1 MW owned facility: ~£2.5–3.5 million [🔴 author estimate — component breakdown in Appendix]

**Financing:**
- Phase 0: ~£10,000 self-funded (4 × RTX 5090 GPUs)
- Seed: £300,000–600,000 equity (after pilot validation; funds first 1–2 owned facilities)
- Debt: Project finance considered from Year 3 once track record established

### 10.2 Five-Year P&L Projection

| | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|-|--------|--------|--------|--------|--------|
| **Sites operational (year-end)** | 0 | 2 | 6 | 12 | 20 |
| **IT capacity (MW)** | 0 | 2 | 6 | 12 | 20 |
| | | | | | |
| **Revenue** | | | | | |
| Colocation | £0 | £504k | £1,587k | £3,628k | £6,883k |
| Managed GPU | £0 | £0 | £310k | £893k | £1,680k |
| Flexible mining | £0 | £126k | £154k | £198k | £252k |
| Demand response | £0 | £50k | £150k | £300k | £500k |
| **Total Revenue** | **£0** | **£680k** | **£2,201k** | **£5,019k** | **£9,315k** |
| | | | | | |
| **Operating Costs** | | | | | |
| Energy (wind + grid) | £0 | £214k | £643k | £1,286k | £2,143k |
| Connectivity | £0 | £96k | £288k | £576k | £960k |
| Site leases | £0 | £48k | £144k | £288k | £480k |
| O&M (local staff) | £0 | £90k | £270k | £540k | £900k |
| Insurance | £0 | £36k | £108k | £216k | £360k |
| Software & licences | £0 | £24k | £48k | £72k | £96k |
| **Total Opex** | **£0** | **£508k** | **£1,501k** | **£2,978k** | **£4,939k** |
| | | | | | |
| **Gross Profit** | **£0** | **£172k** | **£700k** | **£2,041k** | **£4,376k** |
| **Gross Margin** | — | 25% | 32% | 41% | 47% |
| | | | | | |
| **Central Overhead** | | | | | |
| Salaries (central team) | £420k | £540k | £780k | £1,200k | £1,620k |
| Edinburgh office/NOC | £60k | £72k | £96k | £120k | £150k |
| Sales & marketing | £80k | £120k | £180k | £240k | £300k |
| Legal & compliance | £60k | £80k | £100k | £120k | £140k |
| G&A | £40k | £60k | £80k | £100k | £120k |
| **Total Overhead** | **£660k** | **£872k** | **£1,236k** | **£1,780k** | **£2,330k** |
| | | | | | |
| **EBITDA** | **-£660k** | **-£700k** | **-£536k** | **£261k** | **£2,046k** |
| **EBITDA Margin** | — | — | — | 5% | 22% |
| | | | | | |
| Depreciation & amortisation | £0 | £300k | £900k | £1,800k | £3,000k |
| **EBIT** | **-£660k** | **-£1,000k** | **-£1,436k** | **-£1,539k** | **-£954k** |

*Note: EBIT negative through Year 5 due to depreciation of rapid asset build-out. Cash EBITDA turns positive in Year 4. With project finance replacing equity from Year 3, equity IRR improves significantly.*

### 10.3 Cashflow Summary

| | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|-|--------|--------|--------|--------|--------|
| EBITDA | -£660k | -£700k | -£536k | £261k | £2,046k |
| Capex | -£1,800k | -£1,800k | -£7,200k | -£10,800k | -£12,000k |
| Equity raised | £2,400k | £0 | £18,000k | £0 | £0 |
| Debt raised | £0 | £0 | £2,000k | £5,000k | £5,000k |
| Debt service | £0 | £0 | -£200k | -£700k | -£1,200k |
| **Net cash movement** | **-£60k** | **-£2,500k** | **+£12,064k** | **-£6,239k** | **-£6,154k** |
| **Cash balance (year-end)** | **£2,340k** | **-£160k*** | **£11,904k** | **£5,665k** | **-£489k*** |

**Note**: Asterisked figures indicate Series A must close before cash out. Timing is critical; fundraise should begin Month 24 for Month 30 close.

### 10.4 Funding Requirements

**Phase 0 — Self-funded pilot (no investors required)**

| Use of funds | Amount |
|-------------|--------|
| 4 × RTX 5090 GPUs (£2,500 each) | ~£10,000 |
| Networking / hosting setup | £1,000–2,000 |
| Vast.ai / RunPod provider registration | £0 |
| **Total** | **~£10,000–12,000** |

*This phase requires no external investors and can begin immediately.*

**Seed Round: £300,000–600,000 (after pilot validation)**

Raised after the Phase 0 pilot has generated real revenue data — removing the largest single risk for investors.

| Use of funds | Amount |
|-------------|--------|
| First owned 100 kW wind-adjacent facility | £200,000–350,000 |
| Battery storage (500 kWh) | £80,000–100,000 |
| Legal (PPA, lease, incorporation) | £60,000–80,000 |
| Working capital (12 months) | £80,000–120,000 |
| **Total** | **£420,000–650,000** |

*Note: The managed-service build fees (£40–80k per facility) fund WindEdge's operations from Year 1 onward and reduce dependence on equity. A formal Series A may not be required if the managed-service cash flow is sufficient.*

### 10.5 Key Financial Metrics

| Metric | Target |
|--------|--------|
| Payback period (per site) | 3.5–4.5 years |
| Gross margin (steady state) | 50–60% |
| EBITDA margin (Year 5) | 22% |
| Revenue per employee (Year 5) | £207k |
| Customer acquisition cost (enterprise) | £15,000–40,000 |
| Customer lifetime value (enterprise, 3yr) | £540,000–1,800,000 |
| LTV:CAC ratio | 20:1–45:1 |

---

## 11. Team & Hiring Plan

### 11.1 Founding Team (Required)

The founding team requires a specific combination of expertise not commonly found together. WindEdge should recruit across these roles:

**CEO / Co-Founder**
- Background: Energy infrastructure or data centre operations; commercial/BD focus
- Key relationships: Wind farm operators, enterprise IT buyers, Scottish Enterprise
- Salary: £80,000 + equity

**CTO / Co-Founder**
- Background: Data centre engineering, power systems, or distributed systems
- Responsibilities: Technical architecture, site design, DCIM platform
- Salary: £80,000 + equity

**Head of Energy / Co-Founder (or early hire)**
- Background: Energy trading, PPA structuring, grid services
- Responsibilities: Negotiate wind PPAs, manage grid relationships, optimise energy cost
- Salary: £75,000 + equity
- Note: This role is unusual and critical. Finding someone who understands both energy markets and data centre operations is the single hardest hire.

**CFO (Month 6–12)**
- Background: Infrastructure finance, project finance
- Responsibilities: Fundraising, financial modelling, project finance from Series A
- Salary: £70,000 + equity

**Linus Deluca-Perry — Founding Business Strategist**
Business Analyst at BlackRock's Transformations Office, where he leads large-scale change programmes across the firm, managing significant workstreams and becoming a subject matter expert across complex business areas. Physics BSc from Imperial College London. He is also the founder of LDP Solar, where he developed and patented an elevated agri-solar mounting system enabling dual land use — demonstrating the ability to take a technical idea from concept to patent application to commercial pilot independently. His execution track record at BlackRock and his hands-on experience founding a renewable energy technology company give WindEdge a commercial lead with both institutional credibility and entrepreneurial proof. He leads commercial strategy, investor relations, and business development.

**Ye He — Founding Engineer and Technical Advisor**
2nd year PhD student at CERN (Imperial College London), measuring the top quark mass using simulation-based inference on the CMS experiment — the first application of this technique in CMS. Her work involves building complete GPU-accelerated analysis workflows for large-scale datasets across the CMS collaboration. Her direct experience designing and operating high-performance GPU pipelines is directly applicable to WindEdge's GPU marketplace infrastructure and EMS integration. She contributes as a technical advisor on GPU architecture, workflow design, and HPC pipeline optimisation.

### 11.2 Hiring Plan

| Role | When | Salary |
|------|------|--------|
| Site Engineer (x1) | Month 8 | £45,000 |
| NOC Analyst (x1) | Month 12 | £38,000 |
| Enterprise Sales (x1) | Month 14 | £55,000 + commission |
| Regional Ops Manager (x1) | Month 18 | £55,000 |
| DevOps / Software (x1) | Month 18 | £60,000 |
| Enterprise Sales (x2) | Month 24 | £55,000 + commission |
| Site Engineers (x2) | Month 24 | £45,000 |
| Marketing Manager (x1) | Month 24 | £50,000 |
| Finance Analyst (x1) | Month 24 | £42,000 |

*Post-Series A: 20+ additional hires across engineering, operations, sales*

### 11.3 Advisory Board

WindEdge should establish an advisory board covering:

- **Wind energy**: Former senior SSE Renewables or Vattenfall executive
- **Data centre operations**: CTO/COO from Tier 3 UK colocation provider
- **Scottish policy**: Former Scottish Enterprise or Scottish Government senior official
- **Enterprise sales**: Former VP Sales from enterprise tech company
- **ESG/sustainability**: Sustainability expert from Big 4 or specialist consultancy

Advisors compensated with 0.1–0.25% equity (4-year vest) in lieu of cash.

---

## 12. Funding Requirements

### 12.1 Investment Thesis for Investors

WindEdge represents an infrastructure investment with the following characteristics:

**Defensive moat**: Energy cost advantage is structural — curtailment is growing, not shrinking. Competitors cannot replicate <£20/MWh energy cost without replicating WindEdge's site-by-site partnership model, which takes years to build.

**Growing market**: Data centre demand is growing 11–13% annually; green compute demand grows 19% annually. WindEdge sits at the intersection.

**Regulatory tailwind**: UK SDR, EU CSRD, and government AI compute strategy all drive demand directly to WindEdge's product.

**Asset-backed**: Every pound invested creates tangible infrastructure assets (containers, battery, servers) that can be sold or refinanced.

**Acquisition optionality**: Multiple plausible acquirers (hyperscalers, large telcos, infrastructure funds) as the portfolio scales.

### 12.2 Comparable Transactions

| Company | What they do | Raised / Valuation |
|---------|-------------|-------------------|
| Etix Everywhere (France) | Modular edge DCs | €80m raised (2022) |
| Hydro66 (Sweden) | Hydropower-adjacent DC | £35m Series B (2021) |
| Datacenter One (Germany) | Green colo | €50m (2023) |
| Deep Green (UK) | Waste heat DCs | £30m Series A (2023) |
| Iceotope (UK) | Liquid cooling for edge | £30m Series B (2022) |

WindEdge's model is closest to Hydro66 (renewable energy arbitrage) and Deep Green (modular, unusual location thesis). Both have demonstrated investor appetite.

### 12.3 Proposed Seed Terms (Indicative)

- Raise: £2,400,000
- Structure: SEIS/EIS-eligible (significant tax advantage for UK investors)
- Pre-money valuation: £4,000,000–6,000,000 (to be negotiated)
- Investors: Scottish Enterprise co-investment, angel investors, climate-focused VCs
- Targeted close: Q4 2026

**SEIS/EIS eligibility**: WindEdge should qualify for SEIS (up to £250k) and EIS (up to £5m) given it is a new UK company in an eligible sector. This gives investors 50% (SEIS) or 30% (EIS) income tax relief plus CGT exemption — materially improving effective returns.

---

## 13. Risk Register & Mitigation

### 13.1 Critical Risks

**Risk 1: Wind farm operator refuses partnership**
- Likelihood: Medium
- Impact: High (delays entire plan)
- Mitigation: Approach 10+ operators simultaneously; curtailment creates strong economic incentive for them; offer revenue share or equity; engage SSE Renewables' innovation team (known to be receptive); fall-back to constrained grid sites if direct wire not achievable

**Risk 2: Connectivity cost prohibitive for remote sites**
- Likelihood: Medium
- Impact: High (undermines unit economics for rural sites)
- Mitigation: Site selection criteria weight fibre proximity heavily; microwave as fallback; Project Gigabit (UK government rural broadband) may subsidise infrastructure; Starlink adequate for some low-latency-tolerance workloads

**Risk 3: Energy intermittency causes SLA breach**
- Likelihood: Low
- Impact: Very High (customer loss, reputation damage)
- Mitigation: 4-layer power resilience (wind → battery → grid → diesel genset); SLA credits capped at 3 months' fees; force majeure clauses for extreme weather; insurance coverage

**Risk 4: Regulatory change (grid pricing, planning law)**
- Likelihood: Low
- Impact: Medium
- Mitigation: Engage proactively with Ofgem and DESNZ; behind-the-meter arrangements generally more stable than grid-connected; planning risk minimal for modular/industrial sites

**Risk 5: Competition from well-funded player**
- Likelihood: Low (2–3 years), Medium (3–5 years)
- Impact: Medium
- Mitigation: First-mover advantage in wind farm relationships; each partnership is exclusive for the site; build customer switching costs (long contracts, integrated systems); scale aggressively once funded

**Risk 6: GPU market volatility (AI compute demand drop)**
- Likelihood: Low (near term)
- Impact: Medium
- Mitigation: GPU revenue is 25% of total — colocation is the anchor; hardware depreciated over 4–5 years; GPU market has structural multi-year demand from hyperscalers alone

**Risk 7: Key person dependency**
- Likelihood: Medium
- Impact: High
- Mitigation: Four co-founders across technical, commercial, and financial domains reduces single-point dependency; document all processes from Day 1; advisory board provides continuity; key person insurance for founding team

### 13.2 Risk Matrix

```
IMPACT
HIGH   │ [Risk 1]  [Risk 3]  [Risk 5]  [Risk 7]
       │
MED    │           [Risk 2]  [Risk 4]  [Risk 6]
       │
LOW    │
       └─────────────────────────────────────────
           LOW        MED        HIGH     LIKELIHOOD
```

---

## 14. Regulatory & Legal Framework

### 14.1 Energy Regulation

**Power Purchase Agreement (PPA) structure:**
- Direct bilateral PPA with wind farm operator
- Behind-the-meter consumption — does not flow through the grid and is not subject to NUoS charges
- Requires Ofgem to confirm exemption from licensed supply obligations (standard for on-site generation PPAs)
- Metering: Ofgem-approved revenue-grade meters required for accurate billing

**Grid connection:**
- Backup grid connection through SSEN (Scottish and Southern Electricity Networks)
- Applicable charges: DUoS (Distribution Use of System) on grid-sourced units only
- Demand response registration: National Grid ESO Demand Flexibility Service; requires aggregator licence or direct registration

**Renewables traceability:**
- Apply for Renewable Energy Guarantees of Origin (REGOs) for wind-sourced units (optional — WindEdge's direct wire claim is stronger)
- Develop proprietary carbon reporting methodology, validated by third party (e.g., Carbon Trust)

### 14.2 Data Centre Regulation

**UK Data Centre Security and Resilience Act (2025):**
- Mandatory registration for data centres >1 MW IT load
- Minimum security standards (physical, cyber, personnel)
- Incident reporting obligations within 24 hours of significant outage
- WindEdge must register each site individually

**GDPR / UK GDPR:**
- All data processing activities documented in Article 30 register
- DPA registered with ICO
- Data centre services: WindEdge is a data processor; customers are controllers
- Standard contractual clauses in all customer agreements
- No transfer of customer data outside UK without explicit consent

**ISO 27001 / SOC 2 Type II:**
- Target ISO 27001 certification for first site within 12 months of go-live
- SOC 2 Type II report required for enterprise and US customers — commission in Year 2
- These are effectively prerequisites for enterprise and public sector sales

### 14.3 Planning and Land Use

**Scottish planning system:**
- Modular containers on existing industrial/wind farm land: typically Class 6 prior approval (Scotland), not full planning permission
- Works on existing grid substation: permitted development in most cases
- Environmental impact: Below EIA thresholds for small modular deployments; however, visual impact assessment advisable for Highland sites
- Building warrant: Required for electrical works; Scottish Building Regulations compliance

**Land lease:**
- 15–25 year ground lease with wind farm operator (aligned to turbine operating life)
- Rent review: CPI-linked, typically 5-yearly
- Break clauses: Seek 5-year tenant break; operator may require 10-year minimum
- Relocation provision: Right to relocate containers within site boundary

### 14.4 Corporate and Commercial

**Key contracts required:**
1. Wind farm PPA and grid connection agreement
2. Ground lease
3. Customer colocation agreements (standard terms + SLA)
4. Connectivity IRU or lease
5. Equipment supply contracts (containers, UPS, batteries)
6. O&M agreements with wind farm operators
7. Employment contracts, IP assignment agreements for all staff
8. Directors' and Officers' insurance, public liability, professional indemnity

---

## 15. Sustainability & ESG

### 15.1 Environmental Impact

WindEdge's core environmental proposition is straightforward: **every kWh of compute is powered by wind energy that would otherwise be wasted.** This is additive decarbonisation — not just substituting renewable for fossil, but consuming energy that had zero alternative use.

**Carbon accounting:**
- Each site should generate annual carbon reports using GHG Protocol Scope 1/2/3 methodology
- Scope 2 emissions for WindEdge operations: near-zero (grid backup ~10% of hours, using REGO-backed tariff)
- Customers report zero Scope 2 from WindEdge-hosted compute
- Target: PAS 2060 carbon neutrality certification for first site by Year 2

**Additional environmental considerations:**
- Container manufacturing: source from suppliers with ISO 14001 certification
- Battery chemistry: lithium iron phosphate (LFP) preferred over NMC for safety and lower cobalt content
- End-of-life: committed recycling partnerships for hardware (Tier 1 ITAD); battery recycling per WEEE
- Water use: zero-water cooling (free air only); significant advantage over hyperscalers using evaporative cooling

### 15.2 Social Impact

**Local employment:**
- Prioritise hiring from wind farm communities (Highlands, Islands)
- Train local wind farm O&M staff for data centre remote hands — adds a skill set to communities with limited employment options
- Living wage commitment for all directly employed and contractor staff

**Community benefit:**
- Negotiate community benefit fund contribution with wind farm operators (standard in Scottish wind development)
- Consider offering discounted connectivity or compute to local schools, NHS facilities co-located near sites

**Data sovereignty:**
- Scottish-hosted, UK-jurisdiction data provides genuine alternative to US hyperscalers
- Relevant for Scottish public sector, NHS, universities, law firms

### 15.3 Governance

- **Board diversity**: Target 40% gender diversity on board from Series A
- **Advisory board transparency**: Published list of advisors and their interests
- **Environmental reporting**: Annual sustainability report from Year 2, aligned to TCFD and GRI standards
- **Anti-bribery**: Strict no-gifts policy; all third-party relationships documented

---

## 16. Exit Strategy

WindEdge's investors should expect returns via one of the following paths:

### Path 1: Trade Sale (Most Likely, Year 5–8)

**Potential acquirers:**

| Acquirer type | Strategic rationale | Indicative multiple |
|--------------|-------------------|-------------------|
| Hyperscaler (Microsoft, Google, AWS) | Acquires Scottish green edge capacity; meets 24/7 CFE targets | 8–15x EBITDA |
| Large UK colocation (Equinix, Digital Realty) | Acquires green product capability and Scottish market | 10–15x EBITDA |
| Infrastructure fund (Macquarie, Brookfield) | Stable, asset-backed, growing revenue; infrastructure IRR profile | 12–18x EBITDA |
| Large telco (BT, Vodafone) | Edge compute network; green credentials | 8–12x EBITDA |
| Wind farm operator (SSE, Vattenfall) | Vertical integration of curtailment value | 6–10x EBITDA |

At Year 5 EBITDA of £2m and 12x multiple → **£24m enterprise value**. With £20m invested (seed + Series A), this represents a 1.2x return — acceptable for infrastructure but below VC targets. However:

- If EBITDA target is hit at Year 5 (£2m) on the path to £10m+ at Year 7, the multiple and trajectory make a Year 7 exit at 15x EBITDA (£150m) highly plausible
- Infrastructure funds typically value on yield rather than multiple, and stabilised sites command premium pricing

### Path 2: Secondary Buyout (Year 4–6)

Infrastructure-focused private equity acquires a majority stake, recapitalises the business, and drives the scale-up. Founders and seed investors receive liquidity; management team stays on with new equity. Common in energy infrastructure.

### Path 3: IPO (Year 7–10)

At 50+ sites and £25m+ revenue, WindEdge would be an attractive AIM or Main Market listing. The green infrastructure narrative and growing data centre market provide strong investor appetite. Requires significant governance build-out and audit trail from early.

---

## 17. Appendices

### Appendix A: Scottish Wind Curtailment Data Sources

- National Grid ESO: Balancing Mechanism Reporting System (BMRS) — public dataset
- Ofgem: Constraint payments annual reports
- SSEN Transmission: Network Development Plans (NDPs)
- Scottish Government: Energy Statistics for Scotland

### Appendix B: Comparable Company Data

| Company | Country | Model | Revenue | Raised | Outcome |
|---------|---------|-------|---------|--------|---------|
| Hydro66 | Sweden | Hydro-adjacent DC | £18m | £35m | Active |
| GreenMountain | Norway | Fjord-cooled DC | €40m+ | PE-backed | Active |
| Borealis DC | Iceland | Geothermal DC | Private | Private | Active |
| Deep Green | UK | Waste heat DC | £5m | £30m | Active |
| Etix Everywhere | France | Modular edge DC | €60m | €80m | Active |

### Appendix C: Scottish Wind Farm Operator Contacts

*(For internal use — do not distribute)*

- **SSE Renewables**: Innovation and New Ventures team, Perth HQ
- **Vattenfall UK**: Business Development, Edinburgh office
- **RWE Renewables UK**: Development team, Swindon (Scotland portfolio managed centrally)
- **ScottishPower Renewables**: Innovation team, Glasgow
- **Fred Olsen Renewables**: Edinburgh HQ, known to pursue ancillary revenue streams

### Appendix D: Key Grant Funding Sources

| Fund | Value | Eligibility | Deadline |
|------|-------|-------------|----------|
| Scottish Enterprise SMART grant | Up to £100k | SME, innovation project | Rolling |
| Innovate UK Smart grants | Up to £500k | UK company, R&D element | Quarterly rounds |
| UKRI Net Zero Innovation Portfolio | £1m+ | Net zero technology | Annual |
| Scottish Government Just Transition Fund | Variable | Highlands and Islands | Rolling |
| REIF (Renewable Energy Investment Fund) | Loan finance | Renewable energy projects | Rolling |
| Highlands and Islands Enterprise (HIE) | Up to £500k | HIE area projects | Rolling |

### Appendix F: Sources & Assumptions — Complete Figure Reference

Every quantitative figure in this document is listed below with its source and confidence level.

**Confidence ratings:**
- ✅ Published source — verifiable from the cited reference
- ⚠️ Industry estimate — directionally supported but not from a single authoritative source
- 🔴 Author calculation or extrapolation — methodology described; treat as illustrative

---

#### Curtailment & Grid

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| Scotland curtails 900–910 GWh annually (2023) | ✅ | National Grid ESO Balancing Mechanism Reporting System (BMRS), bmrs.elexon.co.uk. Verify exact figure from published BM data. |
| Constraint payments £700–703m (2023) | ✅ | National Grid ESO annual constraint cost data; Ofgem State of the Energy Market report. 2023 elevated by high gas prices. Verify at nationalgrideso.com. |
| Curtailment table 2020–2023 (480, 612, 780, 910 GWh; £283m, £401m, £594m, £703m) | ✅ | BMRS data and Ofgem constraint payment reports. Figures consistent with published reporting but should be verified against primary sources before investor use. |
| 2024 estimated 1,050+ GWh / £800m+ | ⚠️ | Author extrapolation from 2020–2023 trend. Not a published figure. |
| 2,000+ GWh curtailment by 2028 | 🔴 | Author extrapolation. SSEN Transmission NDPs discuss curtailment growth but this specific figure is not taken from a published projection. Replace with SSEN NDP figure if available. |
| Scotland ~15 GW installed wind capacity | ⚠️ | Scottish Government Energy Statistics for Scotland (gov.scot/energy-statistics). **This figure should be verified — as of 2024, total installed wind (onshore + offshore) may be closer to 12–13 GW.** |
| ~30% of UK total wind capacity | 🔴 | Calculated from the 15 GW figure above. Subject to same uncertainty. |
| 30–60% curtailment rate at specific Highland sites | ⚠️ | Consistent with BMRS site-level data but no single published source for this range. Verify using site-specific BMRS constraint event data. |
| Grid upgrades complete 2030–2033 | ✅ | SSEN Transmission Strategic Wider Works programme; Ofgem RIIO-T2/T3 regulatory decisions. ssen-transmission.co.uk. |

---

#### Energy Prices

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| UK grid electricity £80–140/MWh for large commercial consumers | ✅ | Cornwall Insight commercial tariff tracker; Ofgem published data. Range reflects variation by contract, location, and year. |
| Hyperscaler effective PPA rate £40–75/MWh | ⚠️ | LevelTen Energy and Modo Energy PPA market reports; consistent with published hyperscaler sustainability reports. Not a specific disclosed contract rate. |
| Curtailed wind PPA rate £5–20/MWh | 🔴 | Author estimate. No published market price exists for bilateral behind-the-meter curtailment PPAs (they are private). Framed as an estimate throughout. |
| NUoS charges £15–25/MWh in Scotland | ✅ | Ofgem TNUoS tariff schedule, published annually. ofgem.gov.uk. |
| WindEdge effective all-in rate £15–35/MWh | 🔴 | Calculated from curtailed wind estimate + 10% grid backup hours. Not a market rate. |
| 85–90% energy cost advantage | 🔴 | Calculated: (grid midpoint − curtailed wind midpoint) ÷ grid midpoint. Illustrative. |
| Demand response revenue £50–150/MWh | ✅ | National Grid ESO Demand Flexibility Service published auction results and Firm Frequency Response market data. nationalgrideso.com. |
| Mining revenue £30–50/MWh | ⚠️ | Author estimate based on Bitcoin mining economics at prevailing network difficulty and BTC price. Highly variable; treated as secondary income. |

---

#### Data Centre Industry

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| Energy as 40–60% of data centre opex | ✅ | Uptime Institute Annual Global Data Centre Survey; Lawrence Berkeley National Laboratory "United States Data Center Energy Usage Report." |
| Industry average PUE 1.58 | ✅ | Uptime Institute Annual Global Data Centre Survey 2023. uptimeinstitute.com. Verify against most recent edition. |
| PUE 1.05–1.10 design target | ⚠️ | ASHRAE TC 9.9 cold-climate benchmarks; Schneider Electric and Vertiv vendor case studies for free-air-cooled containers in northern European climates. GreenMountain (Norway) publishes PUE of ~1.15 as a comparable. This is a design target, not a measured figure. |
| ~89% free cooling hours | 🔴 | Author calculation applying the ASHRAE free-cooling threshold (~18°C wet bulb) to Met Office Scottish Highland climate data. A formal site-specific psychrometric analysis is required before use in engineering documents. |
| Scotland average ambient temperature ~8°C | ✅ | Met Office UK Climate Averages for Scottish Highland stations. metoffice.gov.uk/research/climate/maps-and-data/uk-climate-averages. Verify for specific candidate sites. |
| Cooling energy saving £80–120k per MW per year | 🔴 | Author calculation comparing cooling energy at PUE 1.08 vs. PUE 1.5, at £120/MWh energy cost across 1 MW IT load. Illustrative. |
| 12–16 weeks container delivery | ⚠️ | Based on published lead times from Schneider Electric, Vertiv, and comparable containerised DC vendors. Formal quotes needed. |
| 18–36 months traditional DC build | ✅ | Widely cited in JLL, CBRE, and Cushman & Wakefield data centre market reports. |
| PUE 1.4+ for major colo operators | ✅ | Uptime Institute; individual operator sustainability reports (Equinix, Digital Realty publish PUE data annually). |

---

#### Market Size

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| UK data centre colocation market £5.3bn (2024) | ⚠️ | JLL UK Data Centre Report; CBRE Data Centre Market View. Verify against the most recent edition of either report. |
| 11–13% CAGR, £9.8bn by 2030 | ⚠️ | Same analyst sources. CAGR figures from commercial reports are indicative. |
| Green data centre market $140bn by 2030, 19% CAGR | ⚠️ | Grand View Research, Green Data Center Market Report. Commercial market research; treat as indicative. |
| SAM £1.2bn | 🔴 | Author estimate: ~23% of UK colo market defined as sustainability-motivated or HPC buyers. No external source. |
| AI compute demand tripling every 18 months | ⚠️ | Widely attributed to industry observers including IEA and Nvidia executives, but not a formally published statistic. Use with caution. |

---

#### Pricing & Revenue

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| Colocation price £150–200/kW/month | ⚠️ | Author estimate based on published rack rate data from UK colo providers (BroadGroup, DCD research). Market rates vary significantly. |
| Market rate £180–250/kW/month | ⚠️ | Same basis. |
| GPU pricing £3.50–6.00/GPU-hour | ⚠️ | Author estimate benchmarked against published cloud GPU pricing from Lambda Labs, CoreWeave, and Vast.ai as comparable managed GPU providers. |
| AWS p4d equivalent £8–12/hour | ⚠️ | AWS published on-demand pricing for p4d.24xlarge instances, converted to per-GPU equivalent at prevailing GBP/USD rate. Verify at aws.amazon.com/ec2/pricing. |
| Starlink Business £140/month | ✅ | Starlink published pricing at starlink.com. Subject to change. |
| Rural Scottish fibre £500–2,000/month (1GbE) | ⚠️ | Author estimate based on BT Openreach and wholesale fibre market data. Highly site-dependent. Formal quotes needed. |
| Microwave link capex £15,000–40,000 | ⚠️ | Author estimate based on licensed microwave equipment costs (Ericsson MINI-LINK, Cambium). Formal quotes needed. |

---

#### Financial Model

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| All unit economics figures (revenue, opex, EBITDA, margin) | 🔴 | Author financial model. Key assumptions: colocation £170/kW/month, 70% utilisation, curtailed wind £15/MWh, grid backup 10% hours at £100/MWh. Not validated against operational data. |
| 5-year P&L and cashflow projections | 🔴 | Author model. Site rollout schedule and revenue ramp assumptions are illustrative. |
| Capex per site (£400k container, £400k battery, etc.) | 🔴 | Author estimates based on vendor published pricing and comparable project data. Formal quotes required before committing capital. |
| 3.5–4.5 year site payback | 🔴 | Calculated from the unit economics model above. |
| Revenue per employee £207k (Year 5) | 🔴 | Calculated: £9.3m Year 5 revenue ÷ 45 headcount. Model output. |
| LTV:CAC 20:1–45:1 | 🔴 | Calculated from assumed deal sizes and estimated CAC. Highly uncertain at pre-revenue stage. |

---

#### Comparable Transactions

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| Etix Everywhere €80m raised (2022) | ⚠️ | Reported in trade press (DCD, Data Economy). Verify via Crunchbase or company announcements. |
| Hydro66 £35m Series B (2021) | ⚠️ | As above. |
| Datacenter One €50m (2023) | ⚠️ | As above. |
| Deep Green £30m Series A (2023) | ⚠️ | As above. |
| Iceotope £30m Series B (2022) | ⚠️ | As above. |
| Exit multiples 8–18x EBITDA | 🔴 | Author estimate based on reported infrastructure fund acquisition multiples. Actual multiples vary significantly by market conditions, asset quality, and buyer. Treat as directional. |

---

#### Regulatory & Tax

| Figure | Rating | Source / Methodology |
|--------|--------|---------------------|
| SEIS relief 50%, limit £250k per company | ✅ | HMRC published guidance. gov.uk/guidance/seed-enterprise-investment-scheme-background. |
| EIS relief 30%, limit £5m per year | ✅ | HMRC published guidance. gov.uk/guidance/enterprise-investment-scheme-background. |
| SSEN grid connection application fee ~£2,000–15,000 | ✅ | SSEN published connection offer fee schedule. ssen.co.uk/connections. |
| UK Data Centre Security and Resilience Act (2025) | ✅ | UK Parliament; DSIT guidance. Mandatory registration threshold of 1 MW IT load. |

---

### Appendix E: Recommended Advisers

**Legal:**
- Burness Paull (Edinburgh/Glasgow) — Scottish infrastructure specialist
- Pinsent Masons (Edinburgh) — energy and data centre expertise

**Accountancy / Audit:**
- Johnston Carmichael (Scottish-focused, SEIS/EIS experts)
- Deloitte Edinburgh (for Series A and beyond)

**Technical due diligence:**
- Mott MacDonald (electrical infrastructure)
- DCD Intelligence (data centre consultancy)

**Energy:**
- Baringa Partners (energy market advisory)
- Cornwall Insight (grid and energy market analysis)

---

*This document is confidential and intended solely for the use of the person to whom it is addressed. WindEdge Data Centres Ltd. All rights reserved.*

*Version 1.0 — May 2026*
