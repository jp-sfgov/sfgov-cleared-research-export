# Research Packet: SFPUC Power and Water Deep-Dive — Corrected Engineering Appendix, August 2026

- **Template version:** 2026-08-05
- **Status:** CLEARED FOR PUBLIC DISCLOSURE
- **Direction:** work → personal
- **Clearance date:** 2026-08-16
- **Cleared by:** Jeremy Pollock
- **Research period covered:** 2026-06 through 2026-08-11 (document body), with two waves of corrections applied 2026-08-16
- **Last verified:** 2026-08-16 for §10 q.7, whose figure and its utility challenge were checked against the primary CEC and PG&E filings that day, and for the cooling-water arithmetic in §7.1 and §7.3, which was recomputed rather than re-sourced. 2026-08-11 for the other corrected passages. Earlier sections carry their own in-text verification dates and several are explicitly marked unsourced.
- **Originating private repository or repositories:** `jp-sfgov/sfgov-ccsf-compute` (private, work side)
- **Safe source paths:** `CCSF_SFPUC_power_water_deep_dive.md`
- **Source commits:** `18174daa549b3405702894a0c891e318df8d4803` — "Work the Appendix A retraction ledger through the corpus," 2026-08-16, SSH-signed, signature verified good. The five preceding states are recorded under baseline content identities below, because an earlier draft of this packet named an intermediate state as current and a personal-side integration may have landed against it.
- **Intended destination repository or repositories:** `jspidersf/models-and-harnesses` (personal side), `CCSF-compute/` subdirectory
- **Destination canonical document roles:** the SFPUC engineering appendix — SFPUC system inventory, Raker Act analysis, cooling architecture, three siting scenarios, cost tables, and the SFPUC engagement plan. Companion to the strategic brief, not a substitute for it.
- **Transfer form:** graduated document (full verbatim body)
- **Baseline content identities:** seventeen of the eighteen changes are in-place line replacements. Only change 4 adds a line — it inserts a table row — so the file is 515 lines in the pre-correction state and 516 lines in every state after it, and line numbers are stable from `c686b13` forward.

| State | Commit | SHA-256 | Lines | Bytes |
|---|---|---|---|---|
| Pre-correction | `d87bfd11ea0df511a5fb1f5f564bf9f4c8ea9859` | `43d98e76c5c09aa7c10953e286ddf005822fc138c7e565352ae0a30566b771d0` | 515 | 56,518 |
| After the six corrections | `c686b1300097f41083c59072555233bc136de029` | `d5de2151c6d7fefdf1bada5bed5252355f92220b9b8790387497b90375286790` | 516 | 59,753 |
| After depersonalization and the re-sourcing of correction 6 | `455569d5f20fa67bd009115be4ec4e43d306aa57` | `48a5ec100301ba33a2e91be139953a67ef21b00cacd0c559ec63ed1eda4927d7` | 516 | 60,740 |
| After the evidence-base substitution | `a98b8bb` | `fd79b573543c00e88fdef8d77f9829bd8a5c642280b024d325513fa45efbb8f8` | 516 | 62,524 |
| After cross-reference reconciliation | `81a8a85` | `8979da7786a689ece535b6be25333095921f758d1a7d59bbb3decf5adb730f42` | 516 | 64,938 |

Line and byte counts are the file's actual size at each commit; the digests are what a receiving side should compare against.

- **Expected result identity:** SHA-256 `dd4dfb2ef3c2978a94d52788bba495d56a11e5d44c3b2082d9e25864496aea82` — 516 lines, 67,785 bytes, verified byte-equal to the blob at `18174da`. This is the digest of the embedded body below.

### What changed since the earlier draft of this packet, and why it was never published

An earlier draft of this packet was cut against `455569d` and named `48a5ec10…` as its expected result. It was never published; the disclosure gate was never reached. Three further work-side commits have since touched this document, so that draft is superseded rather than amended:

1. **The companion evidence base was replaced, not edited.** `CCSF_ai_energy_water_evidence_2026-08-11.md` — the document every one of this file's correction notes cites by filename and section — was substituted wholesale on 2026-08-16 with an independently produced replacement. Its section numbering changed, three of its blocks were dropped, and it now carries a nineteen-row retraction ledger in its Appendix A. Every cross-reference in this document had to be repointed, and four of them turned out to have misstated what the old source said. That work is stage three below.
2. **Ten further edits landed here.** Five repointed or corrected cross-references, one reworded correction 6's citation, and four are new flags raised by the replacement's retraction ledger.
3. **Two of this document's corrections now rest on citations the corpus no longer evaluates.** The replacement dropped the old document's assessment of *Power 2026* (the sole support for the resource-adequacy row) and its TeraWulf comparison (which corroborated the $271/MWh anchor). Both citations are now marked unassessed in place. This is a real regression in support and is recorded rather than smoothed over.

### Why this transfers the whole document rather than a delta

Jeremy directed on 2026-08-16 that this packet be cut as a full body, consistent with the 2026-08-11 standing instruction to transfer complete document bodies verbatim rather than summaries or excerpts.

Two consequences follow, both deliberate and accepted:

1. **The full body names City staff.** Line 18 of the embedded document names the City CIO and two Department of Technology staff members, in a note whose purpose is to establish that this work is *not* a chartered City project; line 390 refers to the same three by first name. Under the 2026-08-11 disclosure decision that content is eligible, and Jeremy reviewed this specific instance on 2026-08-16 and directed the full-body transfer anyway. It is flagged here rather than buried because publishing it to a public repository is not reversible in any practical sense.
2. **The whole document travels, including its weak parts.** Several cost figures are explicitly marked "illustrative estimate" with no published source; one water figure is marked "midpoint assumption, unsourced"; and two water bands are now marked unresolved. Those markings are the document's own and are preserved. A reader who lifts a number out of this document without its marking will misuse it.

A third consequence — that an earlier state of the body named an individual outside City government three times — was resolved at the work-side source on 2026-08-16 by corpus-wide depersonalization, before this packet was rebuilt. The embedded body is byte-exact against a work-side file, and that file no longer carries the name.

The corrections are documented in full in the "Corrections and freshness triggers" section below, with their exact anchors, so the receiving side can see precisely what changed at each step of the chain without having to diff the states itself.

## Purpose and context

This packet transfers the corrected SFPUC power and water engineering appendix in full. It is the technical companion to the CCSF public-compute strategic brief: where the brief argues a position, this document does the engineering and cost work underneath it — what SFPUC actually owns and generates, whether the Raker Act permits serving a municipal data center, how a coastal-SF AI hall should be cooled, what three candidate sites would cost, and what CCSF would need to ask SFPUC in order to find out.

It is transferred now because eighteen changes have landed in it since the state a personal-side counterpart is most likely to match, and several change conclusions rather than citations. The document previously argued cooling architecture hard and supply-side water almost not at all; §7.3 now says supply-mix water intensity is plausibly the *larger* water decision. Its §9.2 cost table previously omitted a recurring cost category that applies to any load of consequence. Its cooling-water figures, which had read as arithmetic, do not reconcile with the WUE range stated in the same paragraph and are now marked unresolved. A personal-side counterpart carrying the uncorrected text is not merely out of date on those points — it is reasoning from a framing the current literature has moved past, and citing numbers that cannot be reproduced as written.

Why it matters to the receiving side: the personal-side corpus shares this document's lineage and its stale figures. This is the current state of the engineering analysis.

**Non-authorization.** Nothing in this document is evidence that CCSF has authorized a compute project, a site, a utility arrangement, a procurement, or a capital decision. The work-side project is unchartered research, and the document says so in its own opening. Preliminary conversations do not constitute approval, assignment, scope, or resourcing. The scenarios, cost tables, and engagement questions are analysis of what *could* be asked and built, not a plan that anyone has adopted.

## Research scope and method

The document's own framing sections state its scope and its limits; both are carried verbatim. Summarizing the method here rather than restating it:

- **Public and inferred sources only.** The document was built without access to SFPUC internal capital plans, interconnection queues, rate models, or land-disposition records. That is why its §10 is a list of *questions for SFPUC* rather than answers — the engagement plan exists because the research hit the boundary of what public sources can establish.
- **Illustrative-estimate convention.** Cost figures the document could not source to a published tariff, bid, or filing are marked "(illustrative estimate)" inline. That marking appears throughout the cost tables and is load-bearing. Several energy-rate figures carry an explicit instruction to verify against the current SFPUC Power Rates schedule before external use.
- **Modeled-inference convention.** Climate and cooling figures reached by modeling rather than measurement are marked as such — the ~95-percent-of-hours economization figure, for instance, is labelled a modeled inference with no published SF source, and the ~15-25 wet-bulb-exceedance days carry an explicit "no NOAA/ASHRAE source cited."
- **Anchoring convention.** Every correction was applied at a quoted-string anchor verified unique with `grep -c -F` before editing, never at a line number. Where an anchor did not hold, the change was dropped rather than relocated.
- **Formatting constraint.** This document is ingested into NotebookLM, which flattens markdown. Corrections therefore had to sit as live, non-struck body text rather than as strikethroughs or revision marks. That is why each correction reads as an appended sentence or parenthetical in the running prose.
- **What was verified when.** The stage-one corrections carry the superseded evidence document's 2026-08-11 verification and nothing newer. Correction 6's replacement text was read out of the primary CEC memo and the primary PG&E comment filing on 2026-08-16. The stage-three arithmetic flags were computed on 2026-08-16 from figures already in the document, so they rest on internal consistency rather than on an external source. Everything else carries its original date.

## Findings

The complete findings are carried verbatim in the embedded document below. They are not summarized here, because summarizing was the loss this transfer exists to avoid.

Orientation for the receiving agent, by section:

| Where | What it establishes | Epistemic status |
|---|---|---|
| Opening | Scope, and the explicit statement that this is not a chartered project | Framing; **names City staff** |
| SFPUC system inventory | What SFPUC owns and generates — Hetch Hetchy, the Sunol and Peninsula watersheds, transmission, the Power Enterprise | Fact from public sources |
| §2.7 Southeast Treatment Plant | Plant capacity, NPDES order, and the in-plant reuse precedent; **flagged 2026-08-16** as long-horizon only — no eastside tertiary supply, no eastside distribution main, and SFPUC's funded recycling project serves the west side | Fact on the plant; the integration pathway is speculative and now says so |
| Raker Act analysis | Whether the Act permits serving a municipal data center load | Legal analysis, **explicitly requiring City Attorney opinion before any commitment** |
| §7 cooling architecture | Dry-cooler-first with wet-trim as the right design for coastal SF; reclaimed water as peak-day insurance, not base supply; **corrected twice** — reframed around peak-day watershed withdrawal, then had an unsupported ">30x" peaking figure removed | Modeled inference on the climate figures; the peaking factors are now stated as often six and sometimes above ten |
| §7.1 | Three-loop liquid cooling for modern AI racks; **both makeup-water bands flagged unresolved 2026-08-16** | Fact on the cooling stack; the water figures cannot be reproduced as written |
| §7.2 | What SE Plant would need to deliver Title 22 tertiary, and what the purple-pipe extension would cost | Illustrative estimates, marked |
| §7.3 water math | WUE-based consumption at 5 MW and 40 MW; **corrected four times** — operator-WUE re-anchor, then a Meta/Google correction to it; the direct-versus-indirect finding, then two named limits on it; and an unresolved-arithmetic flag covering the whole passage | The original math rests on a midpoint the document marks unsourced and does not reconcile with its own stated range; the corrections are better sourced than what they qualify |
| §8 | Three siting scenarios in detail, including 200 Paul (Digital Realty) | Analysis on illustrative cost bases |
| §8.3 | The batch-and-overnight workload pod; **flagged 2026-08-16** — the 70/30 split is unmeasured, and "overnight" is a scheduling label here rather than a carbon claim, because this pod runs on direct hydro | Working assumption, flagged, not reversed |
| §9.2 | Consortium-scale cost table; **corrected** with a resource-adequacy row recorded as "not sized," then **re-cited** when the corpus lost its assessment of that source | Illustrative estimates, one explicit gap disclosure, and one citation now marked unassessed |
| §9.3 | Energy cost comparison across HHP, CleanPowerSF tiers, and a dedicated PPA; **corrected** with the TeraWulf $271/MWh external ceiling anchor, then **re-cited** when the corroborating cross-reference disappeared | Rate figures illustrative and marked "verify before external use"; the anchor now rests on the primary company release alone |
| §9.5 | Humboldt offshore wind and subsea HVDC — **framed as climate-vision context, not an anchor-offtaker thesis** (a 2026-06-20 correction) | Corrected framing; read the in-section note |
| §10 | Twelve questions for SFPUC; **question 7 corrected, then re-sourced to two primary filings** | Open questions, not findings; q.7's note is the best-sourced passage in the document |

**Four things the receiving side should not lose in integration:**

- **The cooling-water figures do not reconcile, and the document now says so twice.** On a per-IT-kWh basis at 24/7 operation, the document's own 0.5-1.8 L/kWh range gives 17.8 to 63.9 AF/year at 5 MW and 142 to 511 AF/year at 40 MW. The same document states 60-105 AF/year at 5 MW and an 820 AF/year upper bound at 40 MW. Reaching either top figure takes about 2.9 L/kWh, roughly 60 percent above the top of its own stated range. A total-facility rather than IT electricity boundary would close part of the gap — 1.8 L/kWh at PUE 1.2 gives 76.7 AF/year at 5 MW — but no boundary, duty cycle, or PUE is stated alongside the 60-105 figure, so it cannot be reproduced. Separately, the hybrid 7-20 AF/year band overlaps the bottom of the all-evaporative range computed from the same rule of thumb, which means the stated method does not by itself distinguish the two cooling modes. **Do not cite any of these figures until they are rebuilt on one basis.** This was computed on 2026-08-16 from figures already in the document; it is an internal-consistency finding, not a new source.
- **§7.3's corrected conclusion.** The "less than 1 percent of plant output" reassurance describes *onsite cooling water only*. Indirect water runs far larger nationally, which makes the supply-mix choice in Scenario C plausibly the larger water decision. Two limits on that inference are now stated in place: the national indirect figure is derived from the regional generation mix and **excludes power-purchase agreements and behind-the-meter generation**, which is precisely the arrangement Scenario C contemplates; and hydro-specific water accounting was never researched, while Hetch Hetchy is hydro. Direction graded medium-high; magnitude for this supply mix not established. Do not use the claim externally before that accounting is done.
- **§9.5's framing is itself a correction.** Humboldt offshore wind is climate-vision context, not consortium-anchored supply. That reframing was made 2026-06-20 after an earlier draft overstated it. The in-section correction note is live text; preserve it.
- **The Raker Act question is not settled and is not the document's to settle.** It routes to the City Attorney explicitly. Treat the analysis as issue-framing for counsel, not as a legal conclusion.

## Technical detail

Carried verbatim in the embedded body. The material the receiving side would otherwise have to reconstruct:

- **Cooling architecture and water math** — the dry-cooler-first with wet-trim design, the three-loop liquid cooling stack for GB200-class racks, and the WUE-based scaling to 40 MW. The makeup-water comparison between hybrid and all-evaporative operation is carried with its unresolved-arithmetic flag; read that flag before using the bands.
- **Title 22 delivery path** — side-stream polishing skid sizing and cost at SE Plant, the purple-pipe run to 200 Paul, the pretreatment train specification (filtration, softening, dual biocide program, scale and corrosion inhibitors), the ASHRAE 188 Legionella Water Management Plan requirement, and quarterly Legionella PCR. All of it now carries the §2.7 long-horizon scope flag.
- **Operator-achieved WUE, on incompatible boundaries** — AWS 0.12 L/kWh (2025) and Meta 0.19 (2024) are water *withdrawn* per IT kWh on a global first-party fleet basis; Microsoft 0.27 (FY25) counts cooling and humidification water at owned and controlled sites operating at least twelve months; Google 1.15 (2023-24 study basis) is *consumptive* WUE for data centers supporting large-language-model workloads, and sits **above** the LBNL national modeled range of 0.45-0.48 L/kWh rather than below it. **These figures cannot be ranked against one another or against the national average, and none of them is a defensible CCSF design target.** Digital Realty, the operator of 200 Paul, has published no fleet figure, which matters because that is Scenario A's site.
- **Direct-versus-indirect water** — the national ratio and the per-query indirect share, both carried with the PPA-exclusion and hydro-accounting limits stated above.
- **Peak-day mechanics** — facility peaking factors often reaching six and sometimes exceeding ten, which annual-total reporting misses entirely. An earlier "occasionally over 30x" figure is retracted in place as unsupported.
- **Cost tables** — consortium-scale capital and recurring figures for the SEP upgrade, purple-pipe trunk, solar-plus-BESS at Sunol Valley and Central Valley, and a Sierra batch site at Moccasin; plus the energy-cost comparison across four supply options.
- **IRA elective pay** — how a municipal owner can directly monetize the 30-percent ITC, with energy-community and domestic-content adders reaching 40-50 percent, and why that favors SFPUC ownership over a PPA where land and interconnection align.
- **The twelve SFPUC engagement questions** — Sunol Valley parcel disposition, Warnerville land acquisition, the Sunol 1 MW and University Mound 240 kW small-hydro projects, Moccasin and East-of-Moccasin hydro potential, MID/TID contract terms, dark fiber, Moccasin interconnect headroom, SE Plant effluent temperature and Title 22 roadmap, CleanPowerSF IRP inputs, HHP allocation rules, and the Hunters Point Parcel E transfer schedule.

## Public sources

The document cites its sources inline. The table below covers the sources behind the corrected passages, which are the newest and most load-bearing material in the document.

| Source title | Publisher or author | Publication date | URL and useful locator | Claim or finding supported | Verified date |
|---|---|---|---|---|---|
| Small Bottle, Big Pipe (arXiv:2603.02705) | Han, Li, Wierman, Ren | 2026-03 | https://arxiv.org/abs/2603.02705 | §7 — facility peaking factors often six, sometimes above ten. The author list here is carried from an earlier note and is **not independently confirmed**; the current evidence base cites the preprint by title without naming authors | 2026-08-11 |
| Amazon 2025 sustainability report (WUE disclosure) | Amazon Web Services | 2026 | Operator sustainability disclosure | §7.3 — AWS 0.12 L/kWh withdrawn, 2025 | 2026-08-11 |
| Meta sustainability disclosure (WUE) | Meta | 2025 | Operator sustainability disclosure | §7.3 — Meta 0.19 L/kWh withdrawn, **2024**. An earlier state of this document gave 0.18 for 2025; both the figure and the year were wrong | 2026-08-11 |
| Microsoft environmental data (WUE, FY25) | Microsoft | 2026 | Operator sustainability disclosure | §7.3 — Microsoft 0.27 L/kWh, FY25, cooling and humidification water at owned and controlled sites operating twelve months or more | 2026-08-11 |
| Google WUE, consumptive basis, LLM-serving data centers | Google | 2024-25 study basis | Operator disclosure as reported in the corpus evidence base §5.2 | §7.3 — Google 1.15 L/kWh consumptive, **above** the LBNL modeled national range. Omitted from an earlier state of this document, which made operator disclosures look uniformly better than the national average | 2026-08-11 |
| US Data Center Energy Usage Report: 2025 Update (LBNL-2001758, DOI 10.71468/P1RP4F) | Lawrence Berkeley National Laboratory; lead author Sarah Josephine Smith | June 2026 | https://escholarship.org/uc/item/33m6w3x0 | §7.3 — national modeled WUE range 0.45-0.48 L/kWh; direct and indirect water totals, the latter derived from the regional generation mix and excluding PPAs and behind-the-meter generation | 2026-08-11 |
| Making AI Less "Thirsty" | Li, Yang, Islam, Ren — Communications of the ACM | 2025-06 (arXiv 2023-04) | https://dl.acm.org/doi/10.1145/3724499 | §7.3 — the indirect share of a query's water footprint | 2026-08-11 |
| Power 2026: Electricity Pricing in the Age of AI, Ch. 8 | Neel Somani, self-published | 2026 | https://power2026.ai/ | §9.2 — resource adequacy as a recurring load-serving-entity obligation. **Now unassessed.** The corpus's evaluation of this source was dropped when the evidence base was replaced, and the replacement lists CCSF resource-adequacy cost as an explicit omission | Assessment withdrawn 2026-08-16 |
| TeraWulf release on the Anthropic agreement | TeraWulf | 2026-07-06 | Primary company release | §9.3 — ~$271/MWh implied for ~401 MW over 20 years, building and cooling included, GPUs excluded. **Now the sole support for this figure**; the corroborating corpus cross-reference disappeared with the evidence-base substitution | 2026-08-11 |
| Supporting Document for the 2025 IEPR Forecast (data center methodology memo) | California Energy Commission | 2026-04-15 | https://www.energy.ca.gov/sites/default/files/2026-04/Data_Center_Methodology_Memo_ada.pdf — printed pp. 7 and 15 | §10 q.7 — the 67-percent utilization factor applied to *requested service capacity*, derived from Silicon Valley Power operating data, representing the **upper end** of observed utilization; and the worked example 9,587 MW × 67% = 6,423 MW | 2026-08-16 |
| PG&E comments on the 2025 IEPR data center methodology | Pacific Gas and Electric Company | 2026 | CEC docket comment filing; the passage sits on PDF page 5 of 8, and the filing carries no printed pagination | §10 q.7 — PG&E's request that the factor be differentiated between scenarios, calling 67 percent "a high-end estimate" that "may not reflect typical operational characteristics." Establishes that the factor is contested by the incumbent utility rather than settled | 2026-08-16 |
| E3, Forecasting Large Loads in the Age of AI and Data Centers | E3 | 2025-12 | https://www.ethree.com/wp-content/uploads/2025/12/E3Whitepaper_DataCenterForecasting.pdf | **Superseded.** This was the secondary chain of custody through which the 67-percent figure first entered the corpus, misattributed to PG&E analysis and to a nameplate denominator. Retained in this table only so the receiving side can recognize and discard the earlier attribution | Superseded 2026-08-16 |

Sources for the uncorrected body are cited in place within it. The document's own cost and rate figures are largely *not* sourced to published documents and are marked "illustrative estimate" precisely for that reason — that is a stated limitation, not a gap in this table.

## Alternatives and conflicting evidence

- **§7.3's indirect-water magnitude is contested for this specific case,** and on two grounds now rather than one. The national ratio excludes PPAs and behind-the-meter generation, which is the arrangement Scenario C contemplates, so the figure does not describe the configuration the document is reasoning about. And hydro water accounting is methodologically contested, reservoir-evaporation attribution in particular. A defensible counter-position: for a hydro-served load behind a PPA the indirect multiplier could differ materially in either direction, and "arguably the larger one" is an unresolved claim rather than a finding.
- **The operator WUE figures are self-reported**, unaudited, fleet-wide averages over different reporting periods and — the point that the correction added — different measurement boundaries. Two are withdrawal, one is consumptive, and one counts humidification. Fleet averages also blend climates; a global fleet at 0.12 says little about one coastal-SF hall. The re-anchor recommendation still holds only in the weak sense that the rule of thumb it replaces was explicitly unsourced. **It does not support a procurement target,** and an earlier state of this document's companion brief proposed one; that target is recorded on the work side as suspended rather than carried forward.
- **The cooling-water non-reconciliation admits an innocent explanation.** A total-facility electricity boundary rather than an IT boundary would account for part of the gap. The reason the flag stands anyway is that no boundary is stated, so the figure cannot be reproduced either way — the objection is to the unreproducibility, not to the number's plausibility.
- **The resource-adequacy row versus adding no row.** Naming an unsized cost is the more honest instrument, but it does place a row in a cost table that a casual reader could mistake for a priced line item. "Not sized — no published CCSF-scale figure found" is worded to resist that reading. The stronger objection now is that the row's only citation is unassessed.
- **The TeraWulf figure is not a comparable rate.** It is a full-facility lease including building and cooling and excluding GPUs, set against municipal energy-only rates. The text says so. Kept because a table of entirely illustrative figures with no external bound is worse than one with a clearly-labelled non-comparable ceiling.
- **The §10 q.7 addition was once the most reasonable of the corrections to decline** — weak anchor, secondary chain of custody, applied on an execute-all instruction rather than on the merits. That assessment is now wrong. Re-sourcing it to the CEC memo and the PG&E filing made it the best-supported passage in the document, and it is the object lesson for the rest: the figure carried a wrong attribution and a wrong denominator for five days, and only retrieving the primary document caught it.
- **Siting scenarios are not ranked with confidence.** The document presents three and reasons about tradeoffs; it does not establish that any is feasible, because the feasibility inputs are exactly what §10 asks SFPUC for.
- **§9.5's earlier framing was stronger and was corrected downward.** An earlier draft treated Humboldt offshore wind as an anchor-offtaker thesis. That was corrected 2026-06-20 to climate-vision context. If the personal side carries the earlier framing anywhere, this document is the corrected one.

## Caveats and unresolved questions

- **Not a chartered project**, and the document's opening says so. Every scenario and cost table is analysis of what could be asked, not a plan anyone adopted.
- **The Raker Act analysis requires a City Attorney opinion before any commitment.** The document states this explicitly. Legal questions belong to counsel; this analysis frames the issue and does not resolve it.
- **The cooling-water figures do not reconcile** and are flagged unresolved in two places. See the finding above.
- **Most cost and rate figures are unsourced illustrative estimates**, marked as such inline. Several carry an explicit instruction to verify against the current SFPUC Power Rates schedule before external use. Do not lift a number out of this document without its marking.
- **Climate and cooling figures are modeled inferences**, not measurements — the ~95-percent economization figure has no published SF source, and the ~15-25 wet-bulb-exceedance days carry no NOAA or ASHRAE citation.
- **§7.3's hydro and PPA dependencies are open** and are the single thing most likely to force a correction to be rewritten rather than merely refreshed.
- **Digital Realty has published no fleet WUE**, so Scenario A's operator cannot be held to a disclosed figure.
- **California resource adequacy remains unsized at CCSF scale,** and the citation naming the obligation is now unassessed. No published figure was found; the search was not exhaustive.
- **The *Small Bottle, Big Pipe* author attribution is not independently confirmed.** It is carried from an earlier note; the current evidence base cites the preprint by title only.
- **§8.3's 70/30 firm-versus-shiftable split is an unmeasured working assumption,** and the scheduling question above it — whether shiftable municipal work should target overnight hours or solar-rich midday hours — is flagged in the document rather than resolved. Reversing a standing recommendation was left to Jeremy.
- **The stage-three arithmetic flags rest on internal consistency, not on a new source.** They establish that the figures cannot be reproduced as written, not what the right figures are.
- **Not assessed:** whether a personal-side counterpart of this document exists, and if so what state it is in. Everything in the integration guidance below is contingent on that.

## Corrections and freshness triggers

Eighteen changes in three stages. All but change 4 are in-place line replacements; change 4 inserts a table row, taking the file from 515 lines to 516. Line numbers are stable from that point on.

### Stage one: the six changes between `43d98e76…` and `d5de2151…`

Applied 2026-08-16, committed at `c686b13`. Each is given with the anchor it was attached to, verified unique in the source file before editing. The corrected text itself is in the embedded body; these are the locations and the reasons.

| # | Section | Anchor (verified unique) | What changed and why |
|---|---|---|---|
| 1 | §7 | "Much smaller engineering ask." | Appended the general peak-day reframe. The document already had the peak-day insight but scoped it narrowly to reclaimed-water sizing; the literature makes it the framing for *any* SFPUC water conversation. Changes what a CCSF representative would put in front of the Water Enterprise. Graded medium-high. |
| 2 | §7.3 | "At 40 MW scale: 280-820 AF/year depending on cooling mode." | Appended the operator-achieved WUE re-anchor and the Digital Realty gap. The section's math ran off a 0.5-1.8 L/kWh rule-of-thumb with a 1.0 midpoint the document itself marked unsourced. Fact on the figures, recommendation on the target. Two of its figures were wrong and were corrected at stage three. |
| 3 | §7.3 | "Even a 40 MW DC's peak cooling demand is less than 1 percent of plant output." | Appended the direct-versus-indirect water finding and the Scenario C implication. **The most consequential of the six** — the "less than 1 percent" line was doing reassurance work while describing onsite cooling only. Fact on the national ratio; analysis on the Scenario C implication; carries an explicit unresolved dependency on hydro-specific accounting. |
| 4 | §9.2 | "\| Sunol Valley solar+BESS (25-40 MW) \|" (last existing table row) | Inserted a new row for California resource adequacy, recorded as "Not sized — no published CCSF-scale figure found." Gap disclosure. The table had omitted a recurring obligation applying to any load of consequence; the row makes the omission visible where a reader would look for it rather than filling it with an invented number. |
| 5 | §9.3 | "verify against current SFPUC Power Rates schedule" | Appended the TeraWulf ~$271/MWh implied-rate ceiling anchor. The table ran $40-90/MWh, entirely illustrative, with no external bound. Cited deliberately to the primary company release rather than to the secondary primer that popularized the figure. |
| 6 | §10 q.7 | "at the Moccasin substation for new behind-the-meter load." | Appended the PG&E 67-percent-of-nameplate counterweight, flagged in place as a weak fit. The companion document proposed this for both the brief and this file; on checking, this file discusses neither demand-forecast inflation nor nameplate-versus-actual load anywhere. Applied at the nearest topically adjacent point on an explicit execute-all instruction. Both of its substantive claims turned out to be false and were replaced at stage two. |

Two corrections the companion document proposed for this file were **not made, because there was nothing to correct**: it claimed this document contained an LBNL energy-share citation (it contains none) and that it attributed AB 1577 and AB 2619 (it never mentions either bill). Recorded because it bears on how much to trust that document's location index — five of its fourteen proposed locations did not hold when checked.

### Stage two: the two changes between `d5de2151…` and `48a5ec10…`

Applied 2026-08-16, committed at `455569d`. Both were directed by Jeremy after reviewing the stage-one draft of this packet.

| # | Section | Anchor (verified unique) | What changed and why |
|---|---|---|---|
| 7 | §10 q.7 | "at the Moccasin substation for new behind-the-meter load." | **Correction 6 re-sourced to primary documents, which falsified two of its claims.** The 67-percent figure is not PG&E analysis and is not a ratio to nameplate. It is a utilization factor the California Energy Commission applies to *requested service capacity*, derived from Silicon Valley Power operating data, and it represents the **upper end of observed utilization** rather than an average. The replacement text carries the verbatim quotes, the memo title and date, printed pages 7 and 15, the worked example, and PG&E's own filed objection that the factor is a high-end estimate that may not reflect typical operations. This upgrades correction 6 from weak-fit-and-nearly-declined to the best-sourced passage in the document; the earlier grading was wrong. |
| 8 | §1, §9.5, §9.5.5 | "The GovAI Coalition Summit", "per the wind file's existing", and the §9.5 correction note | **Three references to a named individual outside City government were depersonalized** to organizational and role framing. Directed corpus-wide by Jeremy on 2026-08-16, following the boundary set by an earlier depersonalization decision of record: every substantive mention by name is replaced, while files that state the directive itself are left unchanged so the directive stays auditable. Phrasing was chosen to preserve the fact/judgment split — the mentions read as "GovAI Coalition engagement" or "GovAI Coalition leadership" rather than bare "GovAI Coalition," because a bare substitution would make the correction banners appear to condemn the organization's sourced factual record rather than the unevaluated outreach idea. No substantive claim changed. |

### Stage three: the ten changes between `48a5ec10…` and `dd4dfb2e…`

Applied 2026-08-16 across three commits. Every one of them exists because the companion evidence base was replaced rather than edited: five repoint or correct cross-references into the new document, one rewords a citation, and four are new flags raised by the replacement's nineteen-row retraction ledger (its Appendix A).

| # | Commit | Section | Anchor (verified unique) | What changed and why |
|---|---|---|---|---|
| 9 | `a98b8bb` | §10 q.7 | "at the Moccasin substation for new behind-the-meter load." | Reworded correction 7's citation to point at the substituted evidence base. No sourced substance changed; the CEC and PG&E citations are unaffected. |
| 10 | `81a8a85` | §7 | "Much smaller engineering ask." | **Retracted "occasionally over 30x."** The replacement evidence base supports only facility peaking factors often reaching six and sometimes exceeding ten. Also records that the "Ren et al." attribution for the preprint is carried from the earlier note and is not independently confirmed, because the new base cites the preprint by title without authors. |
| 11 | `81a8a85` | §7.3 | "At 40 MW scale: 280-820 AF/year depending on cooling mode." | **Three errors removed from correction 2.** Meta's figure was given as 0.18 for 2025; it is 0.19 for 2024. Google's 1.15 consumptive figure was omitted, which had made operator disclosures appear uniformly better than the national average when one of them is above it. And the four figures were presented as comparable when they use incompatible boundaries. The passage now prohibits ranking them and states that none is a CCSF design target. |
| 12 | `81a8a85` | §7.3 | "Even a 40 MW DC's peak cooling demand is less than 1 percent of plant output." | Repointed to §5.1 of the new base, and added two limits it makes explicit: the indirect figure is derived from the regional generation mix and **excludes PPAs and behind-the-meter generation** — the Scenario C arrangement — and hydro accounting was never researched. Also retired the earlier note's characterization of the onsite figure as "plausibly low by one to two orders of magnitude," which the new base does not support. |
| 13 | `81a8a85` | §9.2 | "\| California resource adequacy (capacity-market obligation) \|" | Re-cited the resource-adequacy row directly to Somani, *Power 2026*, Ch. 8, and **marked the citation unassessed**: the corpus's evaluation of that book was dropped with the substitution, and the replacement's Appendix B lists CCSF resource-adequacy cost as an explicit omission. Nothing in the corpus now evaluates this source. |
| 14 | `81a8a85` | §9.3 | "verify against current SFPUC Power Rates schedule" | Re-cited the TeraWulf anchor. The corroborating cross-reference disappeared with the substitution; the primary company release is now the sole support. |
| 15 | `18174da` | §2.7 | "a directly relevant precedent" | **Scope flag: SE Plant integration is long-horizon only,** not near-term or permit-ready. Beyond the treatment-level gap the section already stated, the plant provides no eastside tertiary supply, there is no eastside distribution main, and SFPUC's funded recycling project (Westside EWRP) serves the west side. The in-plant reuse precedent is a precedent for treatment feasibility, not for delivery to 200 Paul. Source: the replacement base's Appendix A, "Southeast Plant recycled water." |
| 16 | `18174da` | §7.1 | "versus 60-105 AF/year for all-evaporative." | **Both makeup-water bands flagged unresolved,** pointing to the full arithmetic at §7.3. Neither should be cited until they are rebuilt on one basis. |
| 17 | `18174da` | §7.3 | "At 40 MW scale: 280-820 AF/year depending on cooling mode." | **The unresolved-arithmetic finding,** computed here rather than taken from the base: the stated WUE range and duty cycle give 17.8-63.9 AF/year at 5 MW and 142-511 at 40 MW against the document's own 60-105 and 820; the top figures need about 2.9 L/kWh, roughly 60 percent above the stated range; a PUE 1.2 total-facility boundary reaches only 76.7 at 5 MW; and the hybrid band overlaps what the same method yields for all-evaporative, so the method does not distinguish the cooling modes. Directs that all of these be recalculated on one duty cycle, one electricity boundary, and one WUE definition before use. |
| 18 | `18174da` | §8.3 | "**Batch and overnight workload**" | **Flagged, not resolved.** The 70/30 split is unmeasured, and the replacement base holds that in California shiftable work should target solar-rich midday hours rather than assume overnight is cleaner. The narrower point recorded here: this pod runs on direct Hetch Hetchy hydro, where the grid-carbon argument for midday shifting does not apply, so "overnight" is a scheduling label rather than a carbon error. It still bears on the shared-consortium "shoulder hours" claim and on the strategic brief's off-peak recommendation. Reversing a standing recommendation was left to Jeremy. |

### Earlier correction history carried in the body

§9.5's framing of Humboldt offshore wind and subsea HVDC was corrected 2026-06-20 from an anchor-offtaker thesis to climate-vision context. The in-section note is live text and should be preserved. A prior correction cycle at `91d8715a104ed7b5167a09fb316865de1301e19f` (2026-08-05) also touched this file.

### Freshness triggers

Re-verify when: the cooling-water arithmetic is rebuilt on a single basis, which would retire flags 16 and 17 and is the likeliest of these to fire because the work is internal rather than dependent on anyone else's publication; LBNL publishes a WUE methodology refresh or new direct/indirect water figures, particularly any treatment of PPA and behind-the-meter generation; any of the four named operators publishes a new fleet WUE on a stated boundary, or Digital Realty publishes one for the first time; **hydro-specific water accounting becomes available for the Hetch Hetchy system** — the trigger that could force correction 3 to be rewritten rather than refreshed; a published resource-adequacy cost figure at CCSF scale appears, or anything in the corpus assesses *Power 2026*; the CEC publishes a data center methodology memo for a later IEPR cycle, which would supersede the April 15, 2026 utilization factor, or the CEC rules on PG&E's request to differentiate that factor between scenarios; the TeraWulf lease terms are restated; SFPUC publishes a new Power Rates schedule, which every rate figure in §9.3 depends on; the SSIP Nutrient Reduction Project scope or the Westside EWRP program changes the eastside tertiary picture in §2.7 and §7.2; the CleanPowerSF IRP filing cycle advances; or the Hunters Point Parcel E transfer schedule moves off its 2027 estimate.

## Integration guidance

**Destination role.** Land the embedded document as the SFPUC engineering appendix in the personal side's `CCSF-compute/` subdirectory. Suggested name, matching the work-side original: `CCSF_SFPUC_power_water_deep_dive.md`.

**If a personal-side counterpart already exists**, compare its digest against the six recorded above before doing anything:

- `dd4dfb2ef3c2978a94d52788bba495d56a11e5d44c3b2082d9e25864496aea82` — already current; no action.
- `8979da77…` (after cross-reference reconciliation) — has changes 1-14 but not 15-18. Replacing it wholesale with the embedded body is a clean, verifiable update; alternatively apply changes 15 through 18 alone.
- `fd79b573…` (after the evidence-base substitution) — has changes 1-9. Missing 10-18.
- `48a5ec10…` (after depersonalization) — has changes 1-8. **This is the state an earlier draft of this packet named as current.** If a personal-side integration landed against that draft, this is the expected state, and it is missing all ten stage-three changes.
- `d5de2151…` (after the six corrections) — has changes 1-6, and still carries the named individual three times and the false 67-percent attribution.
- `43d98e76…` — exactly the pre-correction state.

In every case, replacing wholesale with the embedded body is the clean path and the resulting digest must equal `dd4dfb2e…`.

- **Equal to none of the six** — the personal side has independent divergence. **Do not replace wholesale.** Apply the eighteen changes at the anchors in the correction tables instead, verifying anchor uniqueness in the destination file first, and record the destination's own pre- and post-application digests. Note the sequential chains: changes 6, 7, and 9 share an anchor and are successive states of the same passage, so apply 9's text and neither 6's nor 7's; changes 2 and 11 likewise, so apply 11's; changes 3 and 12, so apply 12's; changes 1 and 10, so apply 10's; changes 4 and 13, so apply 13's; changes 5 and 14, so apply 14's; and changes 2, 11, and 17 all attach to the same §7.3 anchor, where 17's flag is appended in front of 11's text rather than replacing it. The safest handling for a divergent destination is therefore to take the current text of each of the eight distinct anchored passages from the embedded body wholesale, rather than to replay eighteen changes in order.

**Mismatch behavior.** If an anchor is absent or non-unique in the destination, do not apply that change by approximation and do not relocate it to a close-enough spot. Report the anchor failure and stop on that item. This is the exact failure mode that occurred upstream, where five of fourteen proposed locations did not hold — approximate placement is how weak-fit corrections get laundered into apparently-sourced body text. Correction 6 is the object lesson three times over: applied to a topically thin location on an execute-all instruction, then found to carry a wrong attribution and a wrong denominator that stood for five days, and corrected only when someone retrieved the primary document.

**Expected transformations: none.** Transfer the body byte-exact. Do not summarize, condense, or strip the "illustrative estimate," "unsourced," "modeled inference," "unresolved," "unassessed," or correction-note markings. Those markings are what make the document safe to reuse; without them the numbers read as sourced when they are not.

**Sequencing.** Land the companion packet's document (`CCSF_ai_energy_water_evidence_2026-08-11.md`) first or simultaneously. Every correction note in this document cites it by filename and section, and the references dangle otherwise. **This matters more than it did for the earlier draft:** if the personal side holds the superseded version of that document under the same filename, the section numbers cited here will resolve to the wrong sections rather than to nothing, which is the worse failure. Confirm the companion's digest before treating any cross-reference in this document as resolvable.

**Approval sequence.** Disclosure gate (Jeremy reviews this exact public packet) → publish to `jp-sfgov/sfgov-cleared-research-export` → integration gate (Jeremy reviews the exact personal-side destination diff and the ledger entry) → personal-side commit → ledger update.

**Destination-specific framing that should remain distinct.** The document reasons from a CCSF institutional position about SFPUC's Water and Power Enterprises, the Southeast Treatment Plant, CleanPowerSF, Hetch Hetchy Power, the Raker Act as it binds the City, and three specific San Francisco sites. That is the work side's context and its set of obligations, not the personal side's position. The non-authorization framing above travels with the document. The staff-name note at line 18 exists to establish non-chartered status and should be read that way, not as a list of endorsers.

## Exclusions and disclosure boundary

**Excluded from this packet:** work-side repository history and commit graph beyond the commit IDs cited for provenance; the work-side session state and its internal decision record; the correction-implementation packet that specified the stage-one changes and the inbound-integration packet that is the reviewable artifact for the integration gate (both internal working records that name staff and quote internal directives, and that deliberately retain their own internal/no-share classification because the 2026-08-11 decision covers the research corpus, not working records); prior-session transcripts; raw intake; reader and essentials build artifacts and build scripts; credentials and secrets; any Level 3-5 City data; and the work-side operating context (local filesystem paths, git-metadata locations, remote configuration, device details).

**Verification performed on the transferred body.** Scanned against a named checklist. Clean on: credential and key patterns, local filesystem paths, cloud-storage and git-metadata paths, personal email addresses, personal-only audience markers, Level 3-5 classification markers, and any reference to a depersonalized utility staff individual or to the depersonalized external contact. The checklist enumerates the specific names and identifiers being screened for and is therefore not reproduced in this public packet — reproducing it would publish exactly what it screens out.

**One checklist category is present rather than absent, and a second was resolved at the source.** Both are consequences of the full-body form.

1. **City staff names — present by decision.** Line 18 of the embedded document names the City CIO and two Department of Technology staff members, in a note establishing that this work is not a chartered City project. Line 390 refers to the same three by first name. This is disclosure-eligible under the 2026-08-11 decision, which explicitly accepted that DT and external-advisor staff names need not be stripped. Jeremy reviewed this specific instance on 2026-08-16, was told the full-body form would publish those names, and directed the full-body transfer. Recorded here because the decision was deliberate and because it is the first concrete application of that tradeoff. The names are of public employees in their professional capacities, in a note whose effect is to *limit* rather than expand what the document claims on the City's behalf.

2. **An unevaluated external contact — resolved at the source, and no longer present.** An earlier state of the body named an individual outside City government three times, each time in the course of *retiring* a suggestion that CCSF approach that person and the coalition they are associated with. An earlier draft of this packet flagged the mentions as an open call for the disclosure gate: publish as-is, or depersonalize before publication. Jeremy resolved it on 2026-08-16 by taking neither option as framed. Rather than modify the packet — which would have broken byte-exactness and converted a verbatim transfer into a modified one — he directed depersonalization at the work-side source, corpus-wide, and it was committed at `455569d` before this packet was rebuilt. The embedded body is therefore still byte-exact against a work-side file, and that file no longer carries the name. Recorded rather than deleted because the sequence is the point: the correct fix for a firewall finding in a verbatim packet is upstream in the source, not downstream in the wrapper. Screened clean here.

**Structural exclusions that apply regardless of clearance scope**, per this export repository's charter: credentials, raw intake, session transcripts and records, repository history, and Level 3-5 data are never disclosure-eligible.

## Closeout

- **Public export commit:** `d02857f20318b779ced2d0bb43c92a6a9124e160` — "Publish two cleared outbound research packets (work -> personal)," 2026-08-16, SSH-signed, signature verified good. This packet and its companion were published in that single commit. *(Filled in 2026-08-16; the field previously read "pending disclosure gate," which was left stale at publication and is corrected here.)*
- **Destination content commit or commits:** (pending — personal side)
- **Ledger or manifest commit:** `9732b02` in the private work repository — the sending side's sync-ledger entry recording this packet, its body digest, and the post-commit round-trip verification. Not publicly readable; recorded for traceability.
- **Amendment, 2026-08-16 — the unassessed *Power 2026* citation named below has a second instance the sending side had not counted.** The resource-adequacy row in the §9.2 cost table is one live citation to that book; the other is in a separate corpus document, on the financing chain for a long-term offtake agreement (construction debt underwritten against contracted cash flow, with the counterparty's credit rating setting the borrowing spread), cited to the same book's Chapter 4. Both carry an explicit "treat the citation as unassessed" flag in their own text, so no claim is presented as evaluated when it is not. Recorded because the sending side's own summary of this problem said "one citation," and the count was wrong.
- **Unresolved differences:** Nothing now open can block this packet at the disclosure gate. Whether a personal-side counterpart exists, and which of the six recorded digests it matches, is unknown to the sending side; the integration guidance branches on that and cannot be resolved here. Open on the substance: the cooling-water arithmetic (flags 16 and 17), correction 3's hydro and PPA dependencies, the unassessed *Power 2026* citation behind the resource-adequacy row, the unconfirmed preprint author attribution, the scheduling question in §8.3, and the Raker Act question, which belongs to the City Attorney. Most cost and rate figures in the document remain unsourced illustrative estimates. Open on the work side and outside this packet's body: whether to edit a dated internal correction-implementation record that still carries the depersonalized name, the disposition of four generated reader artifacts and five PDFs that are now stale against these corrections, and whether to port three blocks that were dropped when the evidence base was replaced. All of those are excluded from disclosure by the paragraph above and cannot leak through this channel.

## Completion checklist

- [x] The receiving agent can understand, verify, and integrate the cleared research without access to the originating private files — the full body is embedded, and the correction tables give every anchor and reason for all eighteen changes.
- [x] All eligible substantive detail, links, context, reasoning, caveats, corrections, and provenance were preserved. Nothing was condensed; the document's own "illustrative estimate," "unsourced," "modeled inference," "unresolved," and "unassessed" markings are intact.
- [x] Facts, analysis, inference, and recommendations are distinguishable — the orientation table maps status by section, the correction tables type each change, and the document's inline markings survive verbatim.
- [x] Every decisive claim is traceable to a public source or explicitly identified reasoning; the superseded secondary chain of custody is named as superseded, the withdrawn assessment is named as withdrawn, the unconfirmed attribution is named as unconfirmed, and the unsourced figures are named as unsourced.
- [x] Raw intake and private, restricted, or otherwise ineligible context were excluded.
- [x] Safe source and destination commits are recorded — source commit `18174da`, verified byte-equal to the stated digest, with all five prior states recorded for comparison. Destination commit pending the integration gate.
- [x] Jeremy reviewed the exact public diff and affirmatively cleared it for public disclosure.

---

## Extracting the body

Everything below the delimiter line is the source document, byte-exact, including its own H1 and heading levels. To verify or extract:

```
awk 'f{print} /^<!-- BEGIN VERBATIM/{f=1}' <this-file> \
  | sed '$d' > CCSF_SFPUC_power_water_deep_dive.md
shasum -a 256 CCSF_SFPUC_power_water_deep_dive.md
# expect dd4dfb2ef3c2978a94d52788bba495d56a11e5d44c3b2082d9e25864496aea82
```

The document's own heading levels are preserved rather than demoted, so that quoted section anchors (§2.7, §7.3, §8.3, §9.2, §9.5) resolve exactly as they do in the original.

<!-- BEGIN VERBATIM DOCUMENT: CCSF_SFPUC_power_water_deep_dive.md · SHA-256 dd4dfb2ef3c2978a94d52788bba495d56a11e5d44c3b2082d9e25864496aea82 -->
# CCSF SFPUC Power and Water Integration — Deep Dive

**Date:** May 15, 2026
**Author context:** Prepared for Jeremy Pollock, CCSF DT, as the engineering-and-procurement appendix to `CCSF_public_compute_strategic_brief.md`.
**Document purpose:** Comprehensive reference on the engineering, regulatory, and procurement dimensions of integrating a CCSF public AI compute facility with SFPUC water, power, and wastewater infrastructure. Built as a queryable source for NotebookLM and as a hand-off document for any SFPUC Power Enterprise or third-party engineering engagement.

---

## 1. Purpose and scope

The main strategic brief carries the policy case, governance, and external positioning at a level appropriate for the CIO and Director of Emerging Technology. This document holds the technical and institutional detail at the level appropriate for SFPUC Power Enterprise staff, SFPUC engineering, and any retained feasibility consultant.

**In scope:** the Hetch Hetchy hydroelectric system, the Hetch Hetchy Power Enterprise as service provider, CleanPowerSF as a procurement vehicle, the Southeast Water Pollution Control Plant as a candidate cooling-water source, the SSIP capital trajectory, the Raker Act, the 2015 LAFCo/EnerNex local buildout vision and its actual disposition over the past decade, the August 10, 2026 CleanPowerSF Integrated Resource Plan filing as the planning window, and the three candidate siting configurations.

**Out of scope:** detailed CEQA analysis, geotechnical assessment, specific PPA contract negotiation, and the legal opinion the City Attorney will need to issue on JPA formation and Raker Act application.

> [!warning] Corrections from Jeremy, 2026-06-20 — read before relying on this deep-dive
> - **Not a chartered project.** This is Jeremy's own analysis, not CCSF/SFPUC work product. Preliminary conversations only, with CIO Mike Makstman, Jane Gong, and Tania — none of it chartered or tasked.
> - **SFPUC/CleanPowerSF IRP engagement (§2.3, §10, §11) is a long-term process and will not happen in time for the August 10, 2026 IRP filing.** SFPUC is institutionally conservative; that filing window is effectively closed for this project. Treat §10's "highest-leverage window" framing as superseded.
> - **The Humboldt anchor-offtaker framing (§9.5.5) is retired** — wildly out of scale for CCSF's compute load. See companion brief §7.6 for the corrected framing.
> - **The GovAI Coalition Summit outreach recommendation (§9.5.5, §11) is an AI-generated suggestion**, not evaluated or adopted by Jeremy.

---

## 2. SFPUC system overview

### 2.1 Hetch Hetchy hydroelectric system

Approximately 385 MW nameplate capacity across three powerhouses in Tuolumne County: Holm (169 MW), Kirkwood (124 MW), Moccasin (110 MW). Add ~4 MW Moccasin Low-Head, ~8 MW in-City solar PV at SFPUC facilities, and ~2 MW biomass cogeneration at the Southeast Water Pollution Control Plant. The system is highly correlated with Tuolumne snowpack: long-run average annual generation ~1,574 GWh (1970-2014), but California hydro fell ~48 percent in 2021 versus normal. Multi-year droughts in 2012-2016 and 2020-2022 cut output materially. SFPUC was net-short in dry years and purchased market power to cover obligations. The system is energy-limited and largely committed.

The Moccasin Powerhouse Generator Rehabilitation (2018-2025) extended rotor and stator life; it returned to service in November 2025 with no capacity expansion. The Moccasin Penstock replacement at approximately $285 million is the single largest item in the FY26-35 capital plan, providing a 75-100 year life extension. The capital plan is asset preservation, not capacity growth.

Hetch Hetchy large hydro is *not* RPS-eligible for California Renewable Portfolio Standard purposes (it exceeds the 30 MW threshold and the system was constructed before the eligibility window). The 4 MW Moccasin Low-Head plant *is* RPS-eligible.

### 2.2 Hetch Hetchy Power Enterprise (HHP)

HHP is the SFPUC enterprise that serves municipal load. Distinct from CleanPowerSF. Serves Muni, SFO, SF General Hospital, City College, libraries, museums, ~25,000 streetlights, SFUSD schools, Port, City buildings, plus expanding retail to Treasure Island, Hunters Point, and Mission Rock. Approximately 150 MW of retail load across ~6,300 accounts.

HHP rates are the lowest in the system — likely $40-60/MWh for municipal enterprise customers versus ~$70-80/MWh for CleanPowerSF Green (unsourced — no tariff/source cited; verify). **A new CCSF data center is structurally eligible for HHP service as a municipal load.** Constraint: HHP is energy-limited and largely committed to existing customers. A 4 MW DC (~35 GWh/year) is absorbable (no HHP planning document cited — indicative, not an HHP position). A 40 MW DC (~350 GWh/year, 20-25 percent of average HHP generation) would stress the portfolio in dry years and require new supply layered on top (no HHP planning document cited — indicative, not an HHP position).

The 2023 HHP Integrated Resource Plan explicitly forecasts **no significant additional renewable procurement until 2033**, when additional supply is forecasted as needed to meet load growth and reliability obligations.

### 2.3 CleanPowerSF (CPSF)

SF's Community Choice Aggregation program. Approximately 385,000 accounts, 500+ MW retail load. Reached 100 percent renewable to all customers two years ahead of schedule (target was 2030; achieved 2024). 490 MW of currently online/contracted solar/wind/geothermal plus ~290 MW battery storage. Green default tier is >90 percent clean; SuperGreen is 100 percent California-certified at a small premium (~$7/month for small businesses). No rate increase for 98 percent of customers in FY25-26.

CleanPowerSF files an Integrated Resource Plan with the CPUC every 2-3 years. The next IRP is due **August 10, 2026**. The 2025 "Powering Tomorrow, Together" outreach was the precursor and remains inputs-open as of this drafting. **Correction (2026-06-20): this window will not be used for this project.** SFPUC engagement is long-term and gated on the project maturing well past its current informal stage; SFPUC's process is conservative and cautious by design. The realistic planning horizon is a future IRP cycle.

### 2.4 Central Valley solar + storage portfolio (contracted)

Since 2015, CleanPowerSF has committed to more than 800 MW of new solar/wind/geothermal and over 300 MW of storage (cumulative commitments including projects still in development, per CleanPowerSF); the ~490 MW above is the currently online/contracted slice of that total. Virtually all of it is sited in the Central Valley or further south, contracted through long-term PPAs:

- **Paulsell Energy Center** (NextEra, Stanislaus County): 20 MW solar + 15 MW BESS, COD July 2024.
- **Crow Creek Energy Center** (NextEra, Stanislaus County): 20 MW solar / 60 MWh BESS to CPSF.
- **Blythe IV** (NextEra): 62 MW solar plus new BESS amendment, $220 million over 20 years.
- **Darden** (Fresno): 71 MW solar + 71 MW BESS.
- **IP Easley** (Riverside): 50 MW share of 400 MW project.
- **Corby** (Solano County): 300 MW standalone BESS.

The pattern is clear: contracts in the Central Valley, not owned generation on SFPUC land.

### 2.5 California Community Power (CC Power) JPA

CleanPowerSF is a member of California Community Power, an 8+ CCA Joint Powers Authority. CC Power conducts joint procurement on behalf of member CCAs at scale that no single CCA could achieve alone. Active joint solicitations include 200 MW firm clean, 500 MW long-duration energy storage, and a Geothermal Strategic Initiative RFI issued May 2025.

**This is the operational precedent for the multi-government compute JPA the strategic brief proposes.** Same structural pattern (multi-government joint procurement of capacity through a JPA), same legal vehicle type (California JPA under Gov Code §6500), same opt-in-per-procurement governance. SFPUC has lived inside this governance model since CleanPowerSF joined CC Power. Whoever at SFPUC negotiated the CC Power membership is a useful internal precedent contact for the CCSF compute consortium structuring conversation.

### 2.6 Aqueduct right-of-way

SFPUC owns substantial right-of-way from Early Intake through Moccasin to Oakdale, Tesla, Sunol, and Newark — hundreds of miles of corridor. California has approximately 13 GW of theoretical canal-solar capacity statewide (Project Nexus context) (unsourced — no source cited; verify).

**Important correction to prior analysis:** the Hetch Hetchy water system is mostly tunnels and buried pipe between Sierra Nevada and the Bay Area. The canopy-over-canal model that works on the Turlock Irrigation District canals (Project Nexus, with UC Merced) does not transfer cleanly to the Hetch Hetchy geometry. The aqueduct ROW solar opportunity for SFPUC is at substation/parcel scale (Sunol Valley, Warnerville-adjacent, Tesla Portal, Pulgas), not canopy-over-canal scale. Replace the Project Nexus analogy with parcel solar framing.

### 2.7 Southeast Water Pollution Control Plant (SEP)

Located at 750 Phelps Street, approximately 0.5 mile from the candidate Digital Realty / 200 Paul Ave data center site. Hydraulic peak capacity 250 MGD (new headworks placed in service summer 2024). Average dry-weather flow ~60 MGD. Handles approximately 80 percent of SF's combined sewer and wastewater. Currently produces **disinfected secondary effluent** via high-purity oxygen activated sludge plus chlorination/dechlorination — **not Title 22 disinfected tertiary** as required for evaporative cooling tower service under California Code of Regulations Title 22 §60306.

The plant discharges to central San Francisco Bay under NPDES Order R2-2024-0013. It already reuses filtered/UV-disinfected effluent for in-plant process water — a directly relevant precedent for what would be required to serve a data center cooling load. *(Scope flag added 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` Appendix A, "Southeast Plant recycled water." Treat SE Plant integration as long-horizon only, not near-term or permit-ready. Beyond the treatment-level gap stated above, the plant provides no eastside tertiary supply and there is no eastside distribution main; SFPUC's funded recycling project (Westside EWRP) serves the west side. The in-plant reuse precedent is real but is a precedent for treatment feasibility, not for delivery to 200 Paul.)*

### 2.8 Sewer System Improvement Program (SSIP) trajectory

Total program ~$5+ billion. Key components relevant to the data center cooling question:

- **New Headworks Facility** (250 MGD): substantially complete, in service summer 2024.
- **Biosolids Digester Facilities Project**: ~80 percent construction complete early 2026; substantial completion 2027.
- **Nutrient Reduction Project** (~$1.47 billion): adds biological nitrogen removal targeting ~80 percent N reduction. **Described as "tertiary-grade" for nutrients but not full Title 22 tertiary** unless coupled with filtration plus UV disinfection.
- **No existing eastside recycled water distribution main** near 200 Paul Ave today. The Westside Enhanced Water Recycling Project (Oceanside, MF/RO/UV, 2 MGD avg, 4 MGD peak) is the active SF recycled-water capital project but is ~9 miles from 200 Paul and serves Golden Gate Park.

---

## 3. The 2015 LAFCo Local Buildout vision

In January 2015 SF LAFCo released "Local Build-out of Energy Resources of the Community Choice Aggregation Program," prepared by EnerNex and Willdan. The report identified a portfolio of in-City and regional renewable sites on SFPUC or City-controlled land totaling approximately 47.7 MW local/regional plus 29.8 MW at the Warnerville Substation in Stanislaus County, for a combined 77.5 MW average buildout potential at ~$453 million average capital cost.

Eight specific solar sites were modeled with LCOE and capital cost ranges from three independent estimators (LPI, SFPUC, Black & Veatch):

| Site | Avg MW | Avg Cap ($M, 2015) | LCOE ($/MWh, 2015) | Notes |
|---|---|---|---|---|
| Sunol Valley | 17.5 | $85 | $80-169 | Lowest local LCOE; 100-acre City-owned site on aqueduct corridor; recommended for RFP |
| Warnerville Substation | 29.8 | $173 | $113-169 | Largest single site; co-located with Hetch Hetchy 230kV switchyard; "subject to land acquisition" |
| Hunters Point Parcel E | 6.5 | $40 | $156-234 | 0.5 mi from 200 Paul; subject to environmental approvals (former Naval Shipyard) |
| SFO Parking Lot | 10 | $60 | $141-197 | Subject to SFO approval |
| Tesla Portal | 2.8 | $17 | $85-169 | On aqueduct ROW |
| Pulgas Balancing Reservoir | 2.5 | $20 | $150 | On aqueduct |
| University Mound North Basin | 2.9 | $20 | $154-273 | Seismic upgrade required |
| Sutro Reservoir / Summit Pump | 2.4 | $18 | $168-273 | In-City |
| SF Port Pier 90-94 | 3.1 | $21 | n/a | Industrial waterfront |

Small hydro on the SFPUC water system was separately identified:
- Bay Area: ~5-10 MW total potential. Two projects reportedly under development at time of report: University Mound (240 kW) and Sunol (1 MW).
- San Joaquin/Upcountry: ~10 MW from efficiency improvements, potentially >50 MW total at Moccasin and "East of Moccasin" if full development opportunity pursued.
- RPS eligibility: small hydro under 30 MW *is* RPS-eligible; Hetch Hetchy large hydro is not.

Recommended financing pattern: **PPA with ownership transfer at year 7**, citing Black & Veatch analysis that this produced the lowest lifetime LCOE. A private developer would build and operate for the first 7 years (capturing tax credits, absorbing performance risk), then transfer the asset to the City.

The report assumed:
- Federal solar ITC expiring at end of 2016 (since extended and superseded by IRA elective pay through 2032+).
- 2007-2013 solar PV cost trajectory.
- CleanPowerSF initial program load of 20-30 MW (since grown to 500+ MW).
- "H bonds" as a financing instrument (since superseded by current SFPUC revenue bond practice).

---

## 4. What actually happened 2015-2026: contracts replaced ownership

A decade after the LAFCo report, **virtually none of the identified sites has been built**. SFPUC and CleanPowerSF substituted out-of-county third-party PPAs and California Community Power JPA joint procurement for owned renewable development on SFPUC land. The substitution was driven by:

1. **PPA prices declined faster than expected.** Solar PV LCOE dropped 60-70 percent from 2015-2025 (illustrative estimate). Central Valley utility-scale projects via PPA reach prices below what owned local development could match.
2. **CleanPowerSF reached 100 percent renewable two years ahead of schedule** without needing owned local generation.
3. **Hetch Hetchy Power's customer base grew** with Treasure Island, Hunters Point, and Mission Rock retail expansion, absorbing the existing renewable resource.
4. **Owned local development requires capital, permitting, and operational capacity** that PPAs externalize to private developers.
5. **The 2023 HHP IRP** forecasts no significant additional renewable procurement until 2033, freezing the local-development question for the better part of a decade.

Tactically rational. Strategically leaves the local-development thesis unanswered. The CCSF compute consortium proposal, by introducing a *new municipal customer with a 35-350 GWh/year demand profile and political incentive to anchor on SFPUC infrastructure*, restores the demand-side case for owned generation that PPAs alone could not justify.

---

## 5. Site-by-site current disposition (May 2026)

| Site | 2015 LAFCo concept | 2026 actual status |
|---|---|---|
| **Sunol Valley** | 17.5 MW solar, RFP recommended | Re-scoped 2020 in SFPUC Local Renewable Energy Report to ~40 MW solar+storage at the closed 280-acre Sunol Valley Golf Course. November 20, 2020 LAFCo packet described as "high-suitability" at $30-35/MWh below in-City. **Never advanced past evaluation since 2020.** No RFP issued. Surrounding land hosts Sunol AgPark, Sunol Water Temple, Sunol Yard (rebuilt 2019), Sunol Valley WTP, DeSilva Gates aggregate quarry lease (~325 acres to ~2030), Alameda Creek Watershed Center (late 2026 completion). Political constraint: Alameda Creek Alliance, Sunol Citizens Advisory Council, 2017 community letter opposing industrial conversion |
| **Warnerville Substation** | 29.8 MW solar, subject to land acquisition | Land acquisition never closed. Warnerville treated as transmission asset only; Phase 2 substation rehabilitation contract DB-127R active. **Paulsell Solar Energy Center** (20 MW solar + 15 MW BESS, NextEra, COD June 2024) was sited nearby in Stanislaus County instead — third-party PPA on non-SFPUC land. The Warnerville-corridor solar demand was effectively satisfied off-site by contract |
| **2024 Moccasin parcel acquisition** | n/a (post-report) | $525K, 41 acres on Switchback Road. Purpose is **operational**: maintenance access, fire egress, easement extinguishment. **Not a renewable energy parcel.** Earlier analysis suggesting renewable relevance is corrected here |
| **Tesla Portal** | 2.8 MW solar | No movement since 2015 |
| **Pulgas Balancing Reservoir** | 2.5 MW solar | No movement since 2015 |
| **Hunters Point Parcel E** | 6.5 MW solar | **Not transferred to City.** Navy radiological remediation projects complete end of 2027. Hazmat removal for shipyard demolition began March 2026. No solar development possible on the parcel until post-transfer. A 200 Paul co-located solar story is on a 2+ year delay minimum |
| **SFO Parking Lot** | 10 MW solar carport | Not built. SFO has ~4.5-4.6 MW rooftop only; ZNE plan targets 55 MW campus-wide through third-party PPA. The 10 MW LAFCo carport concept is inactive |
| **University Mound North Basin** | 2.9 MW solar | Seismic upgrade completed 2011. No solar PV built on it. The reservoir is among the City's largest treated-water storage; solar use unclear due to operational constraints |
| **Sutro Reservoir / Summit Pump** | 2.4 MW solar | Not built |
| **SF Port Pier 90-94** | 3.1 MW solar | Not built. Per Port's 2023 OSW concept plan, the piers were redirected to potential offshore wind floating-foundation fabrication |
| **University Mound small hydro (240 kW)** | "Under development" 2014-15 | **No public record of operation.** Either dropped, completed undocumented, or the 2015 report overstated. Confirm with Power Enterprise |
| **Sunol Valley 1 MW small hydro** | "Under development" 2014-15 | **No public record of operation.** Current "Sunol 1.1 MW" reference in some SFPUC documents is solar PV at the WTP, not hydro. Confirm with Power Enterprise |
| **Moccasin Low-Head ~4 MW small hydro** | Operational 1986 | Still operational, RPS-certified |
| **East of Moccasin / >50 MW potential** | Theoretical maximum if pursued | **No active studies, no capital projects.** 2023 HHP IRP modeled scenarios in which further Moccasin investment is uneconomic |
| **Moccasin Powerhouse Generator Rehab** | n/a | $1.6M contingency increase, 331-day delay. Returned to service November 2025. Asset preservation only, no capacity expansion |
| **Moccasin Penstock replacement** | n/a | $285M, largest single item in FY26-35 capital plan. 75-100 year life extension. Asset preservation only |

---

## 6. The Raker Act constraint

The Raker Act of 1913 authorized SF to construct Hetch Hetchy dam and aqueduct on federal land in exchange for specific public-purpose commitments. **Section 6** prohibits sale of Hetch Hetchy power "to any corporation or individual" except to municipalities and qualifying irrigation/water districts. Strictly enforced by *United States v. City and County of San Francisco* (1940). Subsequent litigation has periodically tested the boundary; the consistent ruling has favored strict municipal-only application.

**Implications for the CCSF compute consortium:**

A municipal AI compute facility serving CCSF departments is structurally Raker-compatible — the offtaker is a municipal entity. Leasing capacity to private tenants (the commercial GPU marketplace, anchor-tenant, or commercial AI lab options in the original brainstorm) is **not** Raker-compatible without congressional or legal restructuring.

A consortium of California municipal members under a JPA is **cleanly Raker-compatible** because every offtaker is a municipal entity. This is a stronger legal posture than a standalone CCSF facility with anchor-tenant capacity sharing. The Raker Act, often framed as a constraint, is actually structurally aligned with the JPA consortium model.

City Attorney opinion required before any commitment.

---

## 7. The climate-driven cooling architecture

Coastal SF allows near-chillerless airside economization roughly 95 percent of hours annually (modeled inference, not a published SF figure — see benchmark §1). The right architecture for a 4-40 MW AI hall is **dry-cooler-first with wet-trim** only on the ~15-25 days per year when wet-bulb temperature exceeds 75°F (no NOAA/ASHRAE source cited). That hybrid design uses 7-20 acre-feet per year of makeup water for a 5 MW load versus 60-105 AF/year for all-evaporative. *(Both figures unresolved, flagged 2026-08-16 — the 60-105 AF/year all-evaporative band cannot be reproduced from the WUE range and duty cycle given in §7.3, and the hybrid band overlaps what that method yields for all-evaporative. Full arithmetic in the note at §7.3; do not cite either figure until they are rebuilt on one basis.)*

**Reclaimed water becomes a peak-day insurance policy, not the base cooling source.** Reframes the SE Plant integration question: you don't need 0.5 MGD of tertiary effluent year-round; you need 20-50K gpd reliably on the hottest days. Much smaller engineering ask. The more general point holds beyond reclaimed water: peak-day cooling demand can spike well above the annual average — the underlying modeling puts facility peaking factors at often six and sometimes above ten, so any SFPUC conversation about this facility's water draw should be framed around peak-day watershed withdrawal capacity, not annual totals or a per-query figure — annual-total reporting misses the spike that actually strains a watershed. *(Added 2026-08-11; corrected and repointed 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` §5.3, citing the *Small Bottle, Big Pipe* preprint, March 2026. An earlier "occasionally over 30x" figure has been removed as unsupported; the current evidence base states only that peaking factors often reach six and sometimes exceed ten. That base cites the preprint by title without naming its authors, so the "Ren et al." attribution recorded here is from the earlier note and is not independently confirmed.)*

This is fundamentally different from data center cooling design in Texas, Arizona, or even Virginia — peers where heat is the primary constraint. SF's climate is a structural advantage.

### 7.1 Liquid cooling architecture

Modern AI racks (GB200 NVL72 and successors) require direct-to-chip liquid cooling. The cooling architecture has three loops:

1. **Primary loop (chip-side, FWS):** deionized water or 25-50 percent glycol per ASHRAE TC 9.9 W45/W55 (supply 35-45°C, return 45-55°C, pH 7.5-9.0). Annual inhibitor testing. **Reclaimed water never touches the chip.**
2. **Facility water loop (TCS):** treated potable water or RO-polished reclaimed, between the CDU heat exchanger and the heat-rejection equipment.
3. **Heat rejection (where reclaimed water lives):** dry coolers (no water) or evaporative cooling towers (this is where reclaimed water serves). Hybrid dry/wet uses dry coolers first, evaporative as wet-trim on peak days.

### 7.2 Title 22 compliance

California Code of Regulations Title 22 §60306 requires **disinfected tertiary** recycled water for any cooling tower, evaporative condenser, or misting system, with drift eliminators and continuous biocide. Disinfected secondary is not permitted for cooling tower service without an approved variance.

SE Plant currently produces disinfected secondary. To deliver Title 22 tertiary to 200 Paul, the path is:

- **Side-stream polishing skid at SE Plant:** MBR or UF + UV, $1.5-4M for a 50-200 kgpd capacity unit serving a 5 MW load (illustrative estimate). At 40 MW scale, a larger central polishing facility ($15-40M, potentially folded into the SSIP scope) would be more economic.
- **Purple-pipe extension** from SE Plant to 200 Paul (~0.5 mile in urban Bayview): $400-1,200/LF in urban SF including pavement restoration, $1.5-3M for the run (illustrative estimate).
- **Pretreatment train at the data center:** 5-10 µm self-cleaning filtration, softening if needed, dual biocide program (oxidizing plus rotated non-oxidizing), phosphonate/polymaleic scale inhibitor, azole corrosion inhibitor. ASHRAE 188 Legionella Water Management Plan. Quarterly Legionella PCR.

### 7.3 Water consumption math

Industry rule-of-thumb water use effectiveness (WUE) is ~0.5-1.8 L/kWh for full evaporative cooling. At 1.0 L/kWh (midpoint assumption, unsourced) and 5 MW IT load running 24/7: 120,000 L/day ≈ 31,700 gpd ≈ **35 AF/year**. Hybrid wet/dry in SF climate: 7-20 AF/year. At 40 MW scale: 280-820 AF/year depending on cooling mode. *(Unresolved, flagged 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` Appendix A, "CCSF cooling water," which finds that the annual, peak-day, and scaling arithmetic in this corpus does not reconcile. Worked from the numbers as stated on a per-IT-kWh basis at 24/7 operation, the 0.5-1.8 L/kWh range gives 17.8 to 63.9 AF/year at 5 MW and 142 to 511 AF/year at 40 MW. Section 7.1 and strategic brief §4 instead give all-evaporative cooling as 60-105 AF/year at 5 MW, and the 40 MW upper bound above is 820. Reaching either of those top figures takes about 2.9 L/kWh, roughly 60 percent above the top of the range stated in this same paragraph. Some of the gap could come from a total-facility rather than IT electricity boundary — 1.8 L/kWh at PUE 1.2 gives 76.7 AF/year at 5 MW — but no boundary, duty cycle, or PUE is stated with the 60-105 figure, so it cannot be reproduced as written. Separately, the hybrid 7-20 AF/year band overlaps the bottom of the all-evaporative range computed from the same WUE rule of thumb, which means the stated method does not by itself distinguish the two cooling modes. Recalculate all of these from one duty cycle, one electricity boundary, and one WUE definition before any of them is used in an SFPUC conversation or cited externally.)* Operators publish WUE on incompatible boundaries, so their figures cannot be ranked against each other or against the national average. AWS 0.12 L/kWh (2025) and Meta 0.19 (2024) are water *withdrawn* per IT kWh, global first-party fleet basis. Microsoft 0.27 (FY25) counts cooling and humidification water at owned and controlled sites operating at least twelve months. Google 1.15 (2023–24 study basis) is *consumptive* WUE for data centers supporting large-language-model workloads — above the LBNL national modeled range of 0.45–0.48 L/kWh, not below it. Digital Realty (the operator of 200 Paul) has not published a fleet WUE figure. *(Added 2026-08-11; corrected 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` §5.2, "Operator disclosures are not a ranking." Three errors are removed from the earlier version of this passage: Meta's figure was given as 0.18 for 2025 rather than 0.19 for 2024; Google's 1.15 was omitted, which had made operator disclosures appear uniformly better than the national average; and the assertion that the rule-of-thumb and national average are "two to four times looser than what leading hyperscalers actually deliver" is one the evidence base expressly rejects, since withdrawal and consumption are not comparable quantities. **Suspended, not carried forward:** this passage also recommended that any CCSF procurement WUE target anchor on operator-achieved figures. The evidence base's Appendix A directs that fleet values not be used as a CCSF design target, and separately records this corpus's own cooling-water arithmetic — 7–20 AF/year hybrid, 60–105 at 5 MW, 280–820 at 40 MW — as not reconciling. Whether and how to set a procurement WUE target is therefore an open question pending that recalculation, not a settled recommendation, and the decision has not been made here.)*

For context: SE Plant average dry-weather flow ~60 MGD ≈ 67,000 AF/year. Even a 40 MW DC's peak cooling demand is less than 1 percent of plant output. That comparison covers only onsite cooling water. Nationally the ratio between direct and indirect water is roughly 12x: LBNL's 2023 figures show ~17.4 bn gallons of direct data-center cooling consumption against ~211 bn gallons consumed indirectly to generate the electricity that powers them (UC Riverside's Shaolei Ren group finds the same pattern per-query — roughly 87% of a typical query's water footprint is indirect, from power generation, not onsite cooling). Because Scenario C routes inference to CleanPowerSF Green or Hetch Hetchy Power, supply-mix water intensity is a real water decision here — arguably the larger one — not just a carbon decision. *(Added 2026-08-11; repointed 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` §5.1. Two limits on the indirect figure, both material here: it is derived from the regional generation mix for 176 TWh and **excludes facility power-purchase agreements and behind-the-meter generation**, which is precisely the arrangement Scenario C contemplates; and hydro-specific water accounting was never researched. Do both before using this claim externally.)*

---

## 8. Three siting scenarios in detail

### 8.1 Scenario A: 200 Paul Ave / Digital Realty with hybrid cooling

Digital Realty operates a colocation facility at 200 Paul Ave. Permit-ready, grid-connected today via CleanPowerSF. Bayview industrial zoning. Half a mile from SE Plant. Adjacent to Hunters Point Naval Shipyard (parcel transfer expected 2027).

**Energy:** CleanPowerSF Green (>90 percent clean) as default; Hetch Hetchy Power service may be achievable at 4-10 MW depending on allocation. CPSF SuperGreen (100 percent California-certified) available at small premium.

**Cooling:** Hybrid dry-cooler-first with wet-trim using SE Plant Title 22 reclaimed effluent. New side-stream polishing skid at SE Plant. Dedicated purple-pipe extension to 200 Paul.

**Capex premium:** $3-7M one-time for 5 MW (polishing + purple pipe). Scales to $20-50M at 40 MW including potential SSIP-scope tertiary upgrade.

**Pros:** Fast to deploy. No CEQA for the data center itself (Digital Realty operates an existing permitted facility). Latency to CCSF municipal users near zero. Politically excellent narrative — SF cooling SF's compute with SF's recycled water.

**Cons:** No on-site renewable generation in Phase 1 (Hunters Point Parcel E unavailable until 2027+). Cooling capex premium without owned generation savings — economics are marginal at 5 MW, favorable at 20+ MW.

### 8.2 Scenario B: Sierra batch pod (Moccasin or aqueduct-foothills)

A compact GPU pod sited in Tuolumne County or in the aqueduct corridor between Moccasin and Tesla, served directly by Hetch Hetchy hydro for non-latency-sensitive batch workloads.

**Energy:** Direct Hetch Hetchy hydro at the municipal enterprise rate (~$40-60/MWh). Behind-the-meter delivery avoids wheeling.

**Cooling:** Dry cooling adequate in Sierra winter; significant cooling load in summer when temperatures exceed 100°F at Moccasin, exactly when AI demand peaks. No wastewater source nearby.

**Four hard limits, all still applying:**

1. **No carrier-grade fiber** to SF today. The SFPUC SCADA backbone is not built for tenant-grade bandwidth. A ~140-mile middle-mile build (distance not GPS-confirmed) via leveraging Tuolumne County's Connect 49 plans or CENIC corridors would run $30-80M to do carrier-grade right.
2. **Drought-year firmness.** Hetch Hetchy is largely run-of-river with reservoir shaping. A 24/7 AI load cannot be firmed by Hetch Hetchy alone in dry years.
3. **Summer cooling.** Moccasin summer highs > 100°F kill dry-cooler efficiency exactly when inference demand peaks.
4. **CEQA, tribal consultation under AB 52, Tuolumne County land-use approval, wildfire risk** (Rim Fire 2013 burned the Holm-area watershed).

**Capex:** $80-150M for 10 MW pod including fiber, buildout, interconnect (illustrative estimate).

**Pros:** Direct hydro economics. Raker-compatible municipal load. White-space opportunity to extend Hetch Hetchy's municipal-load story to compute.

**Cons:** Operational complexity. Geographic disadvantage. Constraint stack means realistic ceiling is 10-15 MW.

### 8.3 Scenario C (recommended): Workload-split hybrid with Sunol Valley solar+BESS

The strongest physical configuration that can be assembled from current SFPUC inputs.

**Inference workload** (interactive, latency-sensitive, ~70 percent of total tokens — working assumption pending the Track 0 pilot, not a measured figure — drafts, summaries, Q&A): sited at 200 Paul under CleanPowerSF Green or HHP, with hybrid wet-trim cooling using SE Plant reclaimed effluent.

**Batch and overnight workload** (records-request triage, document OCR, scheduled reports, model fine-tuning, ~30 percent of tokens with relaxed latency tolerance — working assumption pending the Track 0 pilot, not a measured figure): sited at a Sierra batch pod under direct Hetch Hetchy hydro and dry cooling. *(Flagged, not resolved, 2026-08-16 — see `CCSF_ai_energy_water_evidence_2026-08-11.md` Appendix A, "Workload scheduling." The 70/30 split remains unmeasured, and that base holds that in California shiftable work should target low-carbon, solar-rich midday hours rather than assume overnight is cleaner. The narrower point here: this pod runs on direct Hetch Hetchy hydro, where the grid-carbon argument for midday shifting does not apply, so "overnight" is a scheduling label rather than a carbon error. It does still bear on the shared-consortium "shoulder hours" claim below and on the strategic brief's off-peak recommendation (§3.5), flagged there for the same reason.)*

**Dedicated solar+BESS resource at Sunol Valley** (25-40 MW solar plus 4-hour BESS): supplies the Sierra pod behind-the-meter where geometry allows, feeds surplus to Newark interconnect for SF-bound delivery, and serves as the additionality story for the consortium's renewable demand. Sunol is the lowest-LCOE site in the 2015 LAFCo inventory, the parcel is City-owned (280-acre former golf course), and the site has been re-scoped to solar+storage in SFPUC's 2020 internal review but has not advanced to RFP.

**This is the configuration that most efficiently exploits the JPA structure.** Batch workloads can be shared across consortium members on shoulder hours when each city's interactive demand is low. Solar generation at Sunol can serve a regional consortium load profile that no single city could absorb. The Sunol parcel becomes the consortium's anchor demand justification.

**Pros:** Uses each SFPUC asset for what it does best. Raker-compatible (all consortium offtakers are municipal). Restores the demand-side case for owned generation at Sunol that PPAs alone could not justify. Political narrative is durable (Hetch Hetchy / Fiber to Housing / SE Plant / Sunol all in one story).

**Cons:** Requires Sunol Valley parcel disposition to move forward at SFPUC, which has been stalled in evaluation since 2020. Alameda Creek Alliance and Sunol community opposition to industrial conversion is a real political constraint. Multi-site operations complexity. Capital ask is larger than either scenario alone.

---

## 9. Cost analysis

### 9.1 Cost premiums for a 5 MW facility at 200 Paul

| Element | One-time capex premium | Annual opex impact |
|---|---|---|
| Title 22 tertiary side-stream polishing at SEP | $1.5-4M (illustrative estimate) | +$50-150K (chemicals, monitoring) |
| Purple-pipe extension SEP to 200 Paul (~0.5 mi urban) | $1.5-3M (illustrative estimate) | minimal |
| Hybrid wet/dry cooling system vs. dry-only | ~$0 (similar baseline at AI density) | -$100-200K vs. potable cooling |
| HHP municipal enterprise rate instead of CPSF Green | $0 | -$600-700K/yr (unsourced — derived from unverified rate figures; verify) |
| Dedicated CV solar+BESS PPA (additionality) | $0 (PPA structure) | comparable to CPSF Green, 20-yr lock |

**Net for 5 MW:** roughly $3-7M one-time premium plus $600-700K/year of energy savings if HHP serves the load (illustrative estimate — derived from unverified rate figures; verify). Payback on cooling capex 5-10 years depending on energy mix. Below 4 MW the wastewater premium isn't worth the complexity. Above 10 MW it pencils strongly.

### 9.2 Cost premiums for a 40 MW facility (CCSF + early consortium members)

| Element | One-time capex premium | Annual opex impact |
|---|---|---|
| Full Title 22 tertiary upgrade at SEP or large polishing facility | $15-40M (could fold into SSIP scope) (illustrative estimate) | +$500K-1.5M |
| Purple-pipe trunk through Bayview industrial corridor | $5-15M (illustrative estimate) | minimal |
| CV solar+BESS PPA layered in (HHP alone insufficient at scale) | $0 (PPA) or $300-600M if SFPUC-owned | ~$25-30M/yr generation, 20-yr lock |
| Sierra batch site at Moccasin (10 MW pod) | $80-150M (fiber + buildout + interconnect) (illustrative estimate) | -$3-5M/yr vs. all-SF |
| Sunol Valley solar+BESS (25-40 MW) | $50-90M (utility solar at $1.8-2.3M/MW + BESS) (illustrative estimate) | -$2-4M/yr vs. PPA |
| California resource adequacy (capacity-market obligation) | Not sized — no published CCSF-scale figure found | Recurring; load-serving entities must procure and pay generators to remain available for any load of consequence. *(Added 2026-08-11; re-cited 2026-08-16 — currently absent from this cost analysis. Now cited directly to Somani, Power 2026, Ch. 8. The evidence base's assessment of that book, including its fact-check, was dropped when that document was replaced, and its Appendix B lists CCSF resource-adequacy cost as an explicit omission — so nothing in this corpus currently evaluates this source. Treat the citation as unassessed.)* |

At consortium scale, the SE Plant upgrade economics align with SSIP's own trajectory. CCSF compute could be a credible anchor demand customer that justifies adding full Title 22 capability to the SSIP scope, which would in turn make eastside recycled water economically viable for other Bayview industrial customers — cross-system synergy that doesn't show up in single-purpose business cases.

### 9.3 Energy cost comparison

For a 5 MW DC running 50 percent capacity factor (~22 GWh/yr):

| Option | $/MWh | Annual generation cost |
|---|---|---|
| Hetch Hetchy Power municipal enterprise rate | ~$40-60 | $0.9-1.3M |
| CleanPowerSF Green (default, >90% renewable) | ~$70-80 | $1.5-1.8M |
| CleanPowerSF SuperGreen (100% RPS) | ~$80-90 | $1.8-2.0M |
| Dedicated CV solar + 4-hr BESS PPA | ~$70-85 | $1.5-1.9M |

*Rate figures are illustrative — no published tariff cited; verify against current SFPUC Power Rates schedule before using in any external document.* For external scale reference: Anthropic's TeraWulf lease implies roughly **$271/MWh** for 400 MW over 20 years (building and cooling included, GPUs excluded) — well above every municipal rate in the table above, useful as a ceiling anchor, not a comparable figure. (TeraWulf release, July 6, 2026; cited to the primary release, not to the secondary primer that popularized it.) *(Added 2026-08-11; re-cited 2026-08-16 — the evidence-base cross-reference formerly here was removed when that document was replaced; it no longer carries the TeraWulf comparison. The primary release is the sole support for this figure.)*

HHP direct service is materially cheaper where capacity exists. **IRA elective pay treatment** lets a municipal owner directly monetize the 30 percent ITC (40-50 percent with energy-community and domestic-content adders), favoring SFPUC ownership over PPA where land and interconnection align.

---

## 9.5 Humboldt offshore wind + subsea HVDC as consortium-scale supply

*Claude Code · claude-sonnet-4-6 · added 2026-06-20*

**Companion source:** `CCSF_humboldt_offshore_wind_transmission.md` (2026-06-20), with a fact-verification log at its §8. This section folds that file's engineering-relevant findings into the deep-dive; see the companion file for the full political-economy framing, risk list, and source bibliography.

This adds a fourth energy-supply path alongside HHP (Section 2.2), CleanPowerSF (Section 2.3), and the Sunol Valley / Sierra batch pod paths analyzed in Section 8.2–8.3. Unlike those three, this path is not SFPUC-controlled — it is a regional CAISO transmission asset at state/regional-grid scale, ~~that the consortium could anchor as an offtaker,~~ **[struck 2026-06-21 — far too large for the consortium to "anchor"; see §9.5.5]** not a resource SFPUC can develop or contract for unilaterally. The wind file's own §4.2 has the consolidated four-path stack table.

### 9.5.1 Lease areas

Two BOEM Humboldt Wind Energy Area leases resulted from the December 6, 2022 Pacific offshore wind auction:

| Lease | Holder | Acreage | Estimated capacity | Status |
|---|---|---|---|---|
| OCS-P 0561 | Canopy Offshore Wind, LLC (RWE subsidiary) | 63,338 | ~1.6 GW | RWE "Canopy" project; commercial operation "mid-2030s, contingent on permitting" |
| OCS-P 0562 | California North Floating, LLC (Copenhagen Infrastructure Partners; project developer Vineyard Offshore) | 69,031 | over 1 GW | Lease signed June 2023, $173.8M |

**Correction to the combined-capacity figure used elsewhere in this corpus:** the wind file's "~1.6 GW" framing for the Humboldt leases (its §2.1) describes OCS-P 0561 alone. OCS-P 0562 adds "over 1 GW" on top, per BOEM's lease page and the original December 2022 auction reporting. Combined nameplate potential across both Humboldt leases is closer to **~2.6+ GW**, not 1.6 GW. This matters because the HVDC line sized in 9.5.2 below is explicitly the 1.6 GW figure — sized to OCS-P 0561's output, not to both leases combined. If OCS-P 0562 reaches construction on a similar timeline, the transmission scope described below may not have headroom for its full output without a further upgrade. This gap is not flagged in the wind file or its verification log; worth a line in any future revision of that file.

### 9.5.2 CAISO-approved transmission

CAISO's 2023-2024 Transmission Plan (Board-approved May 23, 2024) includes two new lines serving the Humboldt Wind Energy Area, both terminating in the East Bay/Delta:

- **260-mile, 500 kV VSC-HVDC line** — new Humboldt 500 kV substation → Collinsville 500 kV substation (Sacramento–San Joaquin Delta, eastern Contra Costa County). Capacity ~1.6 GW, sized to OCS-P 0561's output (see correction above). VSC (Voltage-Source Converter) technology, suited to variable renewable input.
- **140-mile, 500 kV AC line** — Humboldt substation → Fern Road substation. Adds delivery redundancy and incremental capacity beyond the HVDC line alone. Not previously captured in the wind file's body text; added here per the wind file's own verification log (§8, claim 2), sourced to Downey Brand's April 3, 2024 client alert.

**In-service target: by June 1, 2034**, per the CAISO schedule (wind file §8, claim 2) — later than the "early 2030s" figure used elsewhere in the wind file's body (its §4.5). Treat June 2034 as the more recent, verified figure.

Collinsville sits adjacent to existing PG&E Bay Area transmission infrastructure. It is unrelated to the Trans Bay Cable (53-mile, 400 MW HVDC, SF–Pittsburg) — that is a separate, already-operating asset.

### 9.5.3 Federal headwinds

Two federal actions affect project pace, not the underlying lease or transmission assets:

- **August 29, 2025:** USDOT (Secretary Sean Duffy) withdrew a **$426.7 million INFRA grant** (Nationally Significant Multimodal Freight & Highway Projects program) awarded for the Humboldt Bay Heavy Lift Multipurpose Marine Terminal — staging infrastructure for floating-turbine assembly, not the leases or the transmission line. The Harbor District is seeking alternative funding; the marine-terminal track is delayed, independent of lease or transmission status.
- **December 22, 2025:** a federal pause on offshore wind leasing was applied to five large-scale East Coast projects. Scope is East Coast only — Humboldt's leases (OCS-P 0561, OCS-P 0562) were not directly affected. Litigation over the broader federal pause authority is unsettled as of this drafting; treat the litigation posture as in flux rather than resolved.

**Net assessment, carried over from the wind file (§3):** the CAISO transmission approval is a state-level action (CAISO/CPUC) and does not depend on federal funding or federal lease status. The lease contracts are BOEM instruments, not grant-dependent. The marine terminal is the one piece of Humboldt infrastructure directly exposed to the federal funding cut, and it is staging infrastructure — not a gating dependency for the transmission line or the leases themselves.

### 9.5.4 Raker Act §6 application

Same logic as the Raker Act analysis in Section 6 above, applied to imported (non-Hetch Hetchy) power. Raker Act §6 governs sale of Hetch Hetchy-sourced power specifically; it does not directly apply to CAISO-market power imported via the Humboldt HVDC line. The relevant compatibility question is procurement structure, not power source: CleanPowerSF already procures out-of-county power (Central Valley solar, Section 2.4) through a municipal offtake vehicle and is Raker-compatible on that basis. Humboldt wind power procured the same way — through CleanPowerSF, a CC Power JPA joint solicitation (Section 2.5), or the proposed CCSF compute consortium JPA — follows the same logic: every offtaker under those structures is a municipal entity.

**City Attorney opinion required before any commitment** — the same standing requirement as Section 6's closing line, not a new one.

### 9.5.5 Climate-vision context (anchor-offtaker framing retired)

> [!warning] Correction, 2026-06-20
> This subsection originally argued CCSF's compute consortium could serve as anchor offtaker for the Humboldt transmission line. Per Jeremy's direction: that's wildly out of scale — CCSF/consortium demand (3-40 MW at any modeled scale) against a 1.6-2.6+ GW wind-and-transmission project isn't an anchor relationship. The corrected framing: Humboldt offshore wind belongs here as context for California's broader clean-power and electrification buildout, not as a structural thesis for CCSF's own energy planning. The two "entry points" below (CalCompute, GovAI Summit) are retired along with it — the GovAI Coalition Summit outreach connection specifically is an AI-generated suggestion never evaluated or adopted by Jeremy.

The CAISO-approved transmission line has a defined supply (Humboldt wind) and a defined delivery point (Collinsville). Its scale — 1.6 GW and growing — puts it at state/regional-grid scale, not municipal-consortium scale. Whatever brings it to final investment decision will be CAISO/state-level demand, not a single municipal consortium's IT load. What's still useful for CCSF's own planning: Humboldt is one more signal that California's clean-power supply is expanding substantially this decade — a tailwind for future energy sourcing, not a dependency, and not something this project should position itself around.

~~Two entry points, both already on the consortium's near-term calendar per the wind file (§4.4–4.5):~~

~~- **CalCompute framework process** — established by **SB 53** (signed September 29, 2025), codified at Gov. Code §11546.8. The statute directs a consortium to deliver a framework report to the Legislature by **January 1, 2027**, including funding-source and governance recommendations. An anchor-offtaker thesis is a concrete municipal-demand input ahead of that deadline.~~
~~- **GovAI Coalition Summit, December 9–11, 2026** — a recruiting venue for founding consortium members, per the wind file's existing GovAI Coalition leadership engagement recommendation (wind file §5.1, point 3).~~

### 9.5.6 Cost premium vs. base case

**No cost figure exists yet in this corpus for Humboldt-delivered power, and none should be assumed here.** The energy-cost comparison in Section 9.3 covers HHP, CleanPowerSF Green/SuperGreen, and a generic Central Valley solar+BESS PPA — none of those figures represent offshore wind delivered via a 260-mile HVDC import, which carries its own transmission-access charges, CAISO market-participation costs, and PPA structuring that the wind file does not model either. The open question — **PPA-style procurement through CleanPowerSF versus consortium-direct procurement, and what premium either carries over the Section 9.3 baseline** — is unresolved. Flag for SFPUC/CleanPowerSF engagement (a natural addition to the open-questions list in Section 12) rather than estimate; the procurement vehicle itself isn't chosen yet, so a number now would be a guess dressed as an estimate.

### 9.5.7 Collinsville interconnect question

The Collinsville 500 kV substation is an active PG&E project, independent of the Humboldt line — confirmed via a CAISO Project Sponsor Selection Report, CPUC CEQAnet entry 2025010149, FERC-granted transmission incentives, and the WECC 2026 Annual Progress Report (which lists "Collinsville 500/230 kV Substation Project" under LSPGCA) (wind file §8, claim 8). It is the receiving substation for the new Humboldt HVDC line, built as a separate PG&E capital project.

**Open question, not resolved by current sources:** Collinsville also serves PG&E's existing East Bay load and the broader Bay Area grid. Local congestion at Collinsville could constrain how much of the Humboldt line's output actually reaches San Francisco versus being absorbed by closer East Bay load. PG&E's own Bay Area transmission planning has not been examined for this constraint. Flag for PG&E engagement — a natural addition alongside the SFPUC-focused list in Section 11.

---

## 10. The CleanPowerSF IRP window — why timing matters, when this project is ready

**Correction (2026-06-20): the August 10, 2026 filing is not in play for this project.** SFPUC engagement is a long-term process that won't start until the project is far more developed than its current informal-conversation stage, and SFPUC's own posture is conservative and process-cautious. The analysis below explains why IRP timing matters *in general* — useful for whenever engagement does eventually happen, against a future filing cycle — not as an active near-term plan.

CleanPowerSF files an Integrated Resource Plan with the CPUC every 2-3 years. The 2025 "Powering Tomorrow, Together" outreach was the inputs-open precursor to the August 10, 2026 filing, which this project will miss.

**Why IRP timing matters whenever engagement does happen:**

1. The IRP is the document that justifies new generation procurement to the CPUC.
2. Owned generation at Sunol Valley (or any SFPUC-controlled site) has historically failed the IRP cost-effectiveness test because PPAs in the Central Valley beat the LCOE.
3. A new municipal demand profile — the CCSF compute load — could change the cost-effectiveness math by providing a stable, multi-decade offtaker that PPA-only resource portfolios cannot anchor.
4. Each filing locks the planning cycle for another 2-3 years, so missing one means waiting for the next.

**Recommended action, corrected (2026-06-20):** No near-term SFPUC outreach. Once the project has matured well past informal conversations with Mike, Jane, and Tania, get the CCSF compute load profile into a future CleanPowerSF IRP planning conversation through GovOps, the Mayor's office, or directly through CleanPowerSF staff — paced to SFPUC's own conservative process, not to any filing deadline.

---

## 11. Engagement points

### 11.1 SFPUC (priority order)

1. **SFPUC Power Enterprise leadership** — direct conversation on HHP allocation for a new municipal load, current Sunol Valley parcel disposition, the 2026 IRP inputs window. Power Enterprise is the operational decision-maker for any CCSF compute electric service.
2. **CleanPowerSF Director / Manager of Power Resources** — IRP scope and timing, CC Power JPA membership conversation as governance precedent, peer-CCA receptivity to a compute consortium offtake structure.
3. **Hetch Hetchy Water and Power Director** — Moccasin and East-of-Moccasin small hydro disposition, Sierra siting possibilities, fiber options.
4. **SFPUC Engineering / Water Quality Division** — SE Plant tertiary upgrade scope, Title 22 reclaimed water service to industrial customers, NPDES considerations.
5. **SFPUC Real Estate Services** — Sunol Valley parcel disposition, Warnerville-area parcel status, aqueduct-corridor land availability.
6. **SFPUC General Manager Dennis Herrera** — once the staff-level conversations have surfaced the questions, the GM is the convener of cross-Enterprise decisions.

### 11.2 City Attorney

Required for the Raker Act application opinion to a multi-government compute consortium. The City Attorney's office has a long history of Raker-compatibility analysis (every Hetch Hetchy commercial sales agreement passes through this office).

### 11.3 SF LAFCo

LAFCo's CleanPowerSF oversight role gives it standing to commission follow-up analysis on the local renewable buildout question, and LAFCo packet materials are how SFPUC's CleanPowerSF planning becomes public. LAFCo is also the entity that commissioned the original 2015 EnerNex report and is the natural sponsor for a 2026 update if CCSF compute proceeds.

### 11.4 GovOps and Mayor's office

For the IRP-inclusion ask to land at CleanPowerSF, the political channel goes through GovOps and the Mayor's office. Department of Technology cannot unilaterally direct SFPUC.

---

## 12. Open technical questions for SFPUC engagement

> **Note (2026-08-05):** these requests are framed for a **future** CleanPowerSF IRP cycle. The
> August 10, 2026 filing is not in play for this project (correction of record 2026-06-20).

1. **Sunol Valley parcel disposition.** What's the current SFPUC posture on the 280-acre former golf course? Has the 2020 ~40 MW solar+storage concept advanced beyond evaluation? What are the gating issues — Alameda County permitting, Alameda Creek Alliance opposition, internal land-use planning, or capital availability?
2. **Warnerville Substation land acquisition.** Did SFPUC ever pursue the land acquisition the 2015 LAFCo report flagged? Why did Paulsell get sited adjacent rather than on SFPUC land?
3. **Sunol 1 MW small hydro and University Mound 240 kW small hydro.** Did either project ever come online? If yes, status. If no, why not.
4. **Moccasin and East-of-Moccasin small hydro potential.** Has SFPUC scoped any of the >50 MW potential identified in the 2015 report? Is it in the current Hetch Hetchy capital plan?
5. **Current MID/TID power sales contract terms.** Is there capacity to redirect surplus to a new municipal load?
6. **Dark fiber availability** between Moccasin and SF. What carrier-grade capacity exists today, and what would a build cost?
7. **Spare interconnect capacity** at the Moccasin substation for new behind-the-meter load. *(Related, flagged 2026-08-11; re-sourced 2026-08-16, which corrected the earlier note twice over. **The 67% figure is not PG&E analysis and is not a ratio to nameplate.** It is a utilization factor the California Energy Commission applies to **requested capacity**, derived from Silicon Valley Power operating data: "A 67 percent utilization factor is applied to requested capacity in both the Planning Forecast and the Local Reliability Scenario," and among SVP’s existing data centers "observed peak demand relative to requested service capacity has ranged below this level, with 67 percent representing the upper end of observed utilization" — a ceiling on observed behavior, not an average. The memo’s worked example applies it as 9,587 MW × 67% = 6,423 MW. Source: CEC, "Supporting Document for the 2025 IEPR Forecast" (data center methodology memo), April 15, 2026, pp. 7 and 15; `energy.ca.gov/sites/default/files/2026-04/Data_Center_Methodology_Memo_ada.pdf`. Second, and more useful in a policy conversation: **the factor is contested by the incumbent utility, not settled.** PG&E asked the CEC to differentiate it between the two scenarios, calling the 67% figure "a high-end estimate from data centers in Silicon Valley Power’s (SVP) service territory" that "may not reflect typical operational patterns for data centers, especially in the earlier years of the forecast horizon, when new data centers are ramping up," and pointing to Lawrence Berkeley National Laboratory research showing typical *server* utilization spanning "approximately 15% to 85%" by data center type — while noting in the same breath that "server utilization and capacity utilization are not directly comparable, they are closely related," so treat that range as directional, not as a substitute figure. Source: PG&E Comments RE IEPR Commissioner Workshop on Load Modifier Forecast Results, CEC docket 25-IEPR-03, TN 267761, filed November 26, 2025, under the heading "PG&E recommends the CEC differentiate data center capacity utilization assumptions between the Planning Forecast and Local Reliability scenario" (PDF p. 5 of 8; the letter carries no printed page numbers). **The CEC did not adopt the recommendation** — the April 2026 memo still applies 67% to both scenarios. On the apparent conflict with the 85–90% load factor: the same memo reports average hourly load factors of 85–90% of **observed annual maximum demand** (p. 10) and states plainly that "the interval meter analysis was not used to derive the 67 percent utilization factor" (p. 11), so the two rest on different data and different denominators and are complementary rather than contradictory. The memo also flags, on the same page as the factor itself, that facilities built primarily for AI workloads "may exhibit different operating characteristics" (p. 7). Net for SFPUC: worth asking whether the utilization ratio holds for its own interconnection queue, and worth knowing the ratio is under active dispute in an open CEC proceeding rather than being a settled planning input. See `CCSF_ai_energy_water_evidence_2026-08-11.md` §3.2 and the brief’s §6.3 treatment of this figure.)*
8. **SE Plant effluent temperature profile** seasonally — needed to size the cooling loop.
9. **SE Plant Title 22 tertiary upgrade roadmap.** Is full Title 22 (filtration + UV) part of the SSIP Nutrient Reduction Project scope, or would it be a separate capital project?
10. **CleanPowerSF Integrated Resource Plan** — portfolio inputs for a future IRP filing, headroom for a 40 MW DC load, and IRP timeline for owned generation at Sunol Valley.
11. **HHP allocation rules.** Under what conditions can a new municipal load take HHP service vs. CleanPowerSF default? What's the current spare allocation?
12. **Hunters Point Parcel E transfer schedule.** Confirm with Navy/Treasure Island Development Authority for current 2027 estimate.

---

## 13. Sources

### SFPUC system and Hetch Hetchy

- [SFPUC Hetch Hetchy Power System](https://www.sfpuc.gov/about-us/our-systems/hetch-hetchy-power-system)
- [SFPUC Power Rates 2025-26](https://www.sfpuc.gov/accounts-services/water-power-sewer-rates/power-rates-2025-26)
- [SFPUC IRP filing, CEC docket 18-IRP-01](https://efiling.energy.ca.gov/GetDocument.aspx?tn=256080&DocumentContentId=91857)
- [SFPUC Moccasin Powerhouse Rehabilitation](https://www.sfpuc.gov/about-us/news/raindrops-electrons-moccasin-powerhouse-rehabilitation-project-moves-forward)
- [SFPUC FY 2024-25 to FY 2033-34 10-Year Capital Plan (Attachment B)](https://www.sfpuc.gov/sites/default/files/about-us/policies-reports/FY25-34_Capital_Plan_Report_AttB.pdf)
- [SFPUC 2025 Resolution Log](https://www.sfpuc.gov/sites/default/files/about-us/commission/2025_Resolution_Log.pdf)
- [Raker Act overview](https://en.wikipedia.org/wiki/Raker_Act)

### CleanPowerSF

- [CleanPowerSF Key Documents](https://www.cleanpowersf.org/key-documents)
- [CleanPowerSF Integrated Resource Plan page](https://cleanpowersf.org/resourceplan)
- [CleanPowerSF 2022 IRP LAFCo Presentation](https://cleanpowersf-sfpuc-yem2.squarespace.com/s/July-2022-IRP-LAFCo-Presentation-FINAL.pdf)
- [SFPUC Paulsell Energy Center announcement](https://www.sfpuc.gov/about-us/news/cleanpowersf-announces-solar-and-battery-storage-contract-expanding-programs)
- [SFPUC Crow Creek announcement](https://www.sfpuc.gov/about-us/news/sfpuc-commits-new-solar-and-battery-energy-storage-project-northern-california)
- [SFPUC 100% renewable announcement](https://www.sfpuc.gov/about-us/news/cleanpowersf-provides-100-renewable-electricity-san-francisco-customers-two-years)
- [California Community Power JPA formation](https://cacommunitypower.org/eight-ccas-form-new-jpa/)

### SE Plant and SSIP

- [SFPUC Treating the Liquid Flows (SE Plant)](https://www.sfpuc.gov/about-us/our-systems/sewer-system/treating-liquid-flows)
- [SFPUC New Headworks Facility](https://www.sfpuc.gov/construction-contracts/construction-projects/new-headworks-facility)
- [SFPUC Biosolids Digesters Facilities](https://www.sfpuc.gov/construction-contracts/construction-projects/biosolids-digesters-facilities)
- [SFPUC Upgrading System to Reduce Nutrients](https://www.sfpuc.gov/about-us/our-systems/sewer-system/upgrading-our-system-reduce-nutrients)
- [SFPUC Westside Enhanced Water Recycling Project](https://www.sfpuc.gov/construction-contracts/construction-projects/westside-enhanced-water-recycling-project)
- [SFPUC Recycled Water Rules and Regulations Oct 2024](https://www.sfpuc.gov/sites/default/files/documents/SFPUC_Recycled_Water_Rules_and_Regs_October_2024.pdf)
- [SFPUC Alternative Water Supply Annual Progress Report 2023-24](https://www.sfpuc.gov/sites/default/files/programs/2023-24_AWS_Annual_Progress_Report.pdf)
- [RWQCB Order R2-2024-0013 (SE Plant NPDES)](https://www.waterboards.ca.gov/sanfranciscobay/board_decisions/adopted_orders/2024/R2-2024-0013.pdf)
- [22 CCR § 60306 Recycled Water for Cooling](https://www.law.cornell.edu/regulations/california/22-CCR-60306)
- [EPA California Water Reuse Guideline for Industry](https://www.epa.gov/waterreuse/summary-californias-water-reuse-guideline-or-regulation-industry)

### Reclaimed water cooling precedents

- [Google uses recycled water at Georgia data center (DCD)](https://www.datacenterdynamics.com/en/news/google-uses-recycled-water-at-georgia-data-center/)
- [AWS using reclaimed wastewater at 20 locations (DCD)](https://www.datacenterdynamics.com/en/news/aws-using-reclaimed-wastewater-for-data-center-cooling-at-20-locations/)
- [Water Reuse Case Study: Quincy WA (EPA)](https://www.epa.gov/waterreuse/water-reuse-case-study-quincy-washington)
- [Microsoft datacenters water](https://local.microsoft.com/blog/understanding-water-use-at-microsoft-datacenters/)
- [NVIDIA Blackwell water efficiency / liquid cooling](https://blogs.nvidia.com/blog/blackwell-platform-water-efficiency-liquid-cooling-data-centers-ai-factories/)
- [GB200 NVL72 cooling requirements (ToneCooling)](https://tonecooling.com/nvidia-gb200-nvl72-cooling-requirements/)
- [Energy Implications of Economizer Use in California Data Centers (LBNL)](https://www.osti.gov/servlets/purl/937579)
- [DOE FEMP Cooling Water Efficiency for Federal Data Centers](https://www.energy.gov/cmei/femp/cooling-water-efficiency-opportunities-federal-data-centers)

### 2015 LAFCo report and disposition

- [SF LAFCo / EnerNex Local Build-out Final Report (January 30, 2015)](https://lafco.archive.sf.gov/sites/default/files/FileCenter/Documents/50676-SF%20LAFCo%20CCA%20Local%20Buildout%20Revised%20Final%20Report.pdf)
- [LAFCo CleanPowerSF Job Study (May 5, 2016)](https://www.sfgov.org/lafco/sites/default/files/FileCenter/Documents/55829-FINAL%20-%20LAFCo%20CleanPowerSF%20Job%20Study%205-5-16.pdf)
- [LAFCo Packet, November 20, 2020, Item 5 (LRER review, Sunol 40 MW)](https://www.sfgov.org/lafco/sites/default/files/lfc112020_item5.pdf)
- [LAFCo Packet, July 16, 2021, Item 3](https://www.sfgov.org/lafco/sites/default/files/lfc071621_item3.pdf)
- [LAFCo CleanPowerSF Update presentation, July 17, 2024](https://www.sfgov.org/lafco/sites/default/files/lfc071924_item3_presentation.pdf)
- [LAFCo CleanPowerSF BESS Study, September 2024](https://www.sfgov.org/lafco/sites/default/files/LAFCo_CleanPowerSF_BESS_Study_20240916.pdf)
- [Sunol Community letter to SFPUC, July 2017 (Alameda County BoS agenda)](http://www.acgov.org/board/bos_calendar/documents/DocsAgendaReg_7_19_17/GENERAL%20ADMINISTRATION/Regular%20Calendar/To_the_SFPUC_board_of_directors.pdf)
- [Alameda Creek Alliance, Sunol Valley campaign page](https://www.alamedacreek.org/restoration-progress/sunol-valley.php)
- [Independent News — Sunol Valley Golf Course closure (December 2015)](https://www.independentnews.com/news/another-golf-course-may-replace-closing-sunol-links/article_a484face-a44a-11e5-a157-6b40b4945bf0.html)
- [SFPUC Alameda Creek Watershed Center construction](https://www.sfpuc.gov/construction-contracts/construction-projects/alameda-creek-watershed-center-in-Sunol)
- [SFPUC Sunol AgPark](https://www.sfpuc.gov/learning/for-educators/school-field-trips/sunol-agpark)

### Digital Realty / 200 Paul

- [Digital Realty SFO10 / 200 Paul Avenue](https://www.digitalrealty.com/data-centers/americas/silicon-valley/sfo10)

### Solar and BESS economics

- [LBNL Utility-Scale Solar 2025 Update](https://emp.lbl.gov/sites/default/files/2025-10/Utility%20Scale%20Solar%202025%20Edition%20Slides.pdf)
- [APPA Elective Pay Tax Credits](https://www.publicpower.org/policy/elective-pay-tax-credits)

### Humboldt offshore wind and HVDC transmission (Section 9.5)

- [California North Floating LLC (OCS-P 0562) — BOEM lease page](https://www.boem.gov/renewable-energy/state-activities/california-north-floating-llc-ocs-p-0562)
- [California Lease Sale Winners: RWE, Equinor, CIP, Ocean Winds, Invenergy (Offshorewind.biz, Dec 7, 2022)](https://www.offshorewind.biz/2022/12/07/california-lease-sale-winners-are-rwe-equinor-cip-ocean-winds-and-invenergy-floating-wind-farm-capacities-higher-than-initially-estimated/) — OCS-P 0562 "over 1 GW" capacity estimate
- [Department of Transportation Announces $426.7 Million Grant to Develop Deepwater Port and Marine Terminal in Humboldt Bay (Downey Brand)](https://www.downeybrand.com/legal-alerts/department-of-transportation-announces-426-7-million-grant-to-develop-deepwater-port-and-marine-terminal-in-humboldt-bay/) — original INFRA grant award
- [Trump Administration Pulls Funding for Humboldt Bay Offshore Wind Terminal (Lost Coast Outpost, Aug 29, 2025)](https://lostcoastoutpost.com/2025/aug/29/doomed-offshore-wind/) — grant withdrawal
- [SB 53 chaptered text (LegiScan)](https://legiscan.com/CA/text/SB53/id/3271094/California-2025-SB53-Chaptered.html) — CalCompute statutory basis, Gov Code §11546.8
- [Governor Newsom Signs SB 53 (Sept 29, 2025)](https://www.gov.ca.gov/2025/09/29/governor-newsom-signs-sb-53-advancing-californias-world-leading-artificial-intelligence-industry/)
- See also `CCSF_humboldt_offshore_wind_transmission.md` §7 for the full Humboldt/CAISO source list (lease areas, transmission plan, federal headwinds)
<!-- END VERBATIM DOCUMENT -->
