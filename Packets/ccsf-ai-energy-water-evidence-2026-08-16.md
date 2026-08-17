# Research Packet: AI Energy and Water — Current Evidence and CCSF Implications, August 2026

- **Template version:** 2026-08-05
- **Status:** CLEARED FOR PUBLIC DISCLOSURE
- **Direction:** work → personal
- **Clearance date:** 2026-08-16
- **Cleared by:** Jeremy Pollock
- **Research period covered:** through **August 11, 2026**, which the document states as its own evidence cutoff. Legislative and regulatory status after that date is explicitly out of scope and had already moved by the time this packet was cut.
- **Last verified:** the document's own claims carry its 2026-08-11 date. Three of them were independently re-checked against primary PDFs on 2026-08-16 and the results are recorded under "Independent verification" below — one of the document's page citations did not survive that check. Everything else in the body carries the document's own verification and nothing newer.
- **Originating private repository or repositories:** `jp-sfgov/sfgov-ccsf-compute` (private, work side)
- **Safe source paths:** `CCSF_ai_energy_water_evidence_2026-08-11.md`
- **Source commits:** `a98b8bb` — "Substitute the energy/water evidence base; re-source correction 6 to primary," 2026-08-16, SSH-signed, signature verified good. The file is unchanged at work-side `HEAD` (`18174daa549b3405702894a0c891e318df8d4803`); the three commits after `a98b8bb` touched other corpus files.
- **Intended destination repository or repositories:** `jspidersf/models-and-harnesses` (personal side), `CCSF-compute/` subdirectory
- **Destination canonical document roles:** the corpus's evidence base for AI energy and water — the document every other file in the corpus now cites when it needs an external number. Its Appendix A is a retraction ledger against the rest of the corpus and is the most operationally useful part of it for a receiving side.
- **Transfer form:** graduated document (full verbatim body)
- **Expected result identity:** SHA-256 `48e5dceb0cb31e9501428d7ed0e8269af89ecbd8b1dd41ed837f1d8f41a83760` — 318 lines, 50,381 bytes, verified byte-equal to the blob at `a98b8bb`. This is the digest of the embedded body below.
- **Baseline content identities — read this before integrating.** There is only one, and it is **a different document under the same filename**:

| State | Commit | Title | SHA-256 | Lines | Bytes |
|---|---|---|---|---|---|
| Superseded | `c686b1300097f41083c59072555233bc136de029` | "AI and Data Center Energy and Water — Evidence Refresh, August 2026" | `57bf887e072ebd0719fbbc5e98cb3d4b2774a43e227c1873d3f794735d61dbad` | 519 | 64,320 |
| Current | `a98b8bb` | "AI Energy and Water: Current Evidence and CCSF Implications" | `48e5dceb0cb31e9501428d7ed0e8269af89ecbd8b1dd41ed837f1d8f41a83760` | 318 | 50,381 |

**This was a substitution, not an edit.** The two documents share a filename, a subject, and a date in that filename, and nothing else structurally: different title, different authorship line, different section numbering, 201 fewer lines. A destination holding the superseded document will not produce a meaningful diff against the current one, and — the more dangerous failure — **section cross-references from elsewhere in the corpus will resolve to the wrong sections rather than to nothing.** Every other document in the corpus cites this file by section number, and all of those pointers were repaired on the work side after the substitution. Replace wholesale; do not merge.

### Provenance, and one thing about it that cannot be audited

The current document was produced in a separate session at Jeremy's direction, by a different tool and model than the rest of the corpus — its own metadata line reads *Codex · GPT-5 · 2026-08-11*. It was commissioned as an assume-false review of the superseded document: take each of that document's claims, attempt to falsify it against current primary sources, and rebuild.

That session reported correcting the California demand forecast, a Google publication date, AB 2619's status, a Rhodium comparison, water arithmetic, a Fairwater qualification, and the corpus appendix; that all other tested arithmetic passed; that no material issue remained unresolved; and that the analytical conclusion did not change. It reported its own confidence as high.

**The draft-to-final diff is unauditable.** The session worked in a scratch proposal directory, reported that the proposal's hash matched the replacement, and then removed the directory. No archive remains. So the *claim* that the delivered file equals the reviewed proposal cannot now be checked, and neither can the intermediate reasoning. What can be checked is the file itself, which is what this packet transfers, and its content against primary sources, which is what the "Independent verification" section below does for three claims and does not do for the rest. A receiving side should treat the document as a well-constructed research note whose internal review process is not reproducible, not as a verified artifact.

### Independent verification performed 2026-08-16, and its one negative result

Three of the document's claims were checked directly against primary PDFs on the work side, after the substitution and independently of the session that produced it:

1. **The retirement of the 4.5 GW figure holds, on a stronger basis than the document gives it.** The document's §3.2 and Appendix A retire a "4.5 GW of data-center demand" claim that had entered the corpus from a CAISO document. The cited CAISO report — "Demand response issues and performance 2024," created March 14, 2025, 26 pages — contains **no instance of the string "4.5" and no instance of "data cent" anywhere in its extracted text**. The claim had no support in its own source. Checked by text extraction from the PDF.
2. **The CEC utilization-factor citation holds.** The 67-percent factor, its derivation from Silicon Valley Power operating data, its application to *requested* capacity, its status as the upper end of observed utilization, and the worked example all appear in the CEC's April 15, 2026 data center methodology memo at printed pages 7 and 15. PG&E's filed objection that the factor is a high-end estimate that may not represent typical data centers appears in its comment filing.
3. **One page citation in the document is wrong.** Appendix A's "67% utilization factor" row cites the PG&E comments as **"pp. 4–5."** The filing is 8 PDF pages, **carries no printed pagination at all**, and the passage sits on a single page — PDF page 5. The citation is wrong on both counts. This is a locator error, not a substantive one: the quoted characterization is accurate and the URL in the row resolves to the filing. Recorded because a reader following the citation will not find what the row says is there, and because it is evidence about how closely to trust the document's other page locators.

**Not independently verified, and material:** the adopted-IEPR figures of about 5,800 MW and 8,400 MW for California 2040 and their "pp. 55–56" locator; the four operator water-use-efficiency disclosures; the IEA Figure 2.1 task values that carry the whole reasoning-and-agents section; the Rhodium ranges; the LBNL page and figure locators; the New Zealand, OpenAI, OECD, and Azure-trace datasets in §7.1; and the EU regulation thresholds in §6. That is most of the document. The three checks above were chosen because those claims were load-bearing for corrections already applied elsewhere in the corpus, not because they were the three likeliest to be wrong.

## Purpose and context

This packet transfers, in full, the document that is now the corpus's evidence base for every external number about AI energy and water use. It exists because the corpus had accumulated figures that could not be traced, that had drifted from their sources, or that were arithmetic which does not reproduce — and because a research corpus whose numbers cannot be checked is worse than one with fewer numbers.

Two things make it worth transferring as a whole rather than as findings:

- **Appendix A is a nineteen-row retraction ledger against the rest of the corpus.** For each topic it states what the corpus said, what the current treatment is, and a status: retained, superseded, retired, or unresolved. It is the most directly actionable part of the document for a receiving side that holds any of the same claims. All nineteen rows have since been worked through the work-side corpus; that pass is summarized under "Corrections and freshness triggers" below so the receiving side can see which rows became edits, which were already satisfied, and which were deliberately left as flags.
- **Its epistemic conventions are the point, not decoration.** §2 defines observed, estimated, projected, and scenario, and insists on system boundaries — information-technology electricity versus facility electricity, water withdrawal versus consumption, prompt versus task versus session versus worker-day. Several of the corpus's errors were boundary errors rather than factual ones. Stripping those conventions out would reproduce the failure the document exists to correct.

**Non-authorization.** Nothing in this document is evidence that CCSF has authorized a compute project, a site, a procurement, or a capital decision. Its own closing paragraph says the concept remains informal and unchartered and that nothing in it constitutes approval, assignment, scope, or resourcing. Its CCSF workload and facility figures are described in its own status line as planning scenarios, not forecasts or approved plans.

## Research scope and method

Carried verbatim in the body; the method as the document states and practices it:

- **Assume-false review.** Each claim inherited from the superseded document was treated as false until re-established against a current primary source. The results are visible in Appendix A's status labels rather than asserted in prose.
- **Declared source hierarchy** (§2): greatest weight to government and national-laboratory work, then peer-reviewed studies and open measurement; vendor disclosures retained only with their boundaries; preprints and practitioner cases used as emerging or illustrative evidence, not settled baselines. The document applies this visibly — it names Microsoft authorship on a peer-reviewed modeling paper, names a first-party estimate as first-party, and labels a practitioner case as illustrative.
- **Boundary discipline.** Nearly every figure is given with its boundary in the same cell or sentence. The operator water table (§5.2) is the clearest case: four figures, four different boundaries, and an explicit statement that they cannot be ranked.
- **Arithmetic shown rather than asserted.** §7.1 works the corpus's own stated workload inputs through to a peak throughput range and shows that the published figure is not the result. §7.2 does the same for the cooling-water figures. This is the document's strongest method: it falsifies corpus numbers using only the corpus's own inputs, so the findings do not depend on trusting an external source.
- **Named omissions.** Appendix B lists seven things the document does not estimate. It is not a disclaimer; it is the list of what a reader must not infer from the document's silence.

## Findings

Carried verbatim below. Orientation for the receiving agent, by section:

| Where | What it establishes | Epistemic status |
|---|---|---|
| §1 Executive summary | LBNL and IEA national and global totals; the water components; and the finding that the corpus's worker-to-load chain does not hold while its electricity arithmetic does | Estimates and projections from national-laboratory and intergovernmental sources, labeled as such |
| §1 "What changed since the Inflation Reduction Act" | Policy and supply context, including two Rhodium model runs and the explicit warning that they cannot be added or ranked against each other | Modeled scenarios; the non-additivity caution is the load-bearing part |
| §2 Reading the evidence correctly | The observed/estimated/projected/scenario distinction and the boundary rules | Convention, not finding — but it governs how everything else should be read |
| §3.1 | Top-level U.S., global, and California estimates | Estimates and projections; the national totals explicitly cover all data centers, **not AI alone** |
| §3.2 California grid context | CAISO increases versus CEC total levels, which cannot be substituted; the 67-percent utilization factor correctly attributed; 2024 curtailment | Fact and estimate, with an explicit statement that curtailed energy is not firm or deliverable |
| §4.1 | Per-query estimates from Google, a peer-reviewed model, and Mistral, each with its boundary and each stated as non-rankable | First-party estimate, peer-reviewed model, and vendor lifecycle figure — three different things, so labeled |
| §4.2 Reasoning and agents | The IEA task values, the Hugging Face benchmark range, the coding-agent token ratios, and the practitioner case — concluding that **no defensible general multiplier exists** for CCSF | Mixed; the conclusion is the finding, and it is a negative one |
| §5.1 | National direct and indirect water, the roughly twelve-to-one ratio, and the correction of the "500-millilitre bottle per query" claim | Estimates with boundaries; the hydropower accounting question is explicitly left unresolved |
| §5.2 | Operator water-use efficiency on four incompatible boundaries, with ranking explicitly prohibited | Self-reported vendor disclosures, labeled |
| §5.3 | Peak-water scenarios, the Fairwater closed-loop example, the water-versus-carbon tradeoff, the free-cooling qualification, and the Southeast Plant long-horizon finding | Scenarios and one operating first-party example; the free-cooling figure is named as a modeled inference |
| §6 California policy | Status of one FERC proceeding, two CPUC proceedings, and four bills, plus the enacted EU comparison | Status as of a stated date, **already partly stale** |
| §7.1 | The workload arithmetic that falsifies the corpus's peak figure; the enterprise-evidence table; the GPU-count conflict; the six-point method recommendation; and the adoption and GPU-load sensitivity tables | Arithmetic and analysis on the corpus's own inputs; the sensitivity tables are explicitly labeled planning sensitivities, not forecasts |
| §7.2 | The facility-scale mismatch and the cooling-water non-reconciliation | Arithmetic; both marked unresolved rather than replaced with new numbers |
| §7.3 | The pilot-measurement recommendation and the conclusion that the corpus does not support a decision-grade central estimate | Recommendation, and a negative conclusion |
| Appendix A | Nineteen-row retraction ledger against the corpus, with status labels | The operational core of the document |
| Appendix B | Seven named omissions | Scope statement |

**Five things the receiving side should not lose in integration:**

- **The negative findings are the findings.** "No defensible general multiplier" (§4.2) and "the corpus does not support a decision-grade central estimate" (§7.3) are the document's conclusions. A reader who mines it for numbers and skips these will use it to do exactly what it argues against.
- **Appendix A's status labels are not interchangeable.** *Retired* means do not reuse. *Unresolved* means the arithmetic or definition is insufficient and the figure must be rebuilt, not merely re-cited. *Superseded* means a later source replaces it. *Retained with qualification* means keep it and keep the qualification. Collapsing these into "corrected" loses the instruction.
- **§7.1's arithmetic does not depend on any external source.** It falsifies a corpus figure using only the corpus's own stated inputs. That makes it the most robust finding in the document and the hardest to argue with.
- **Boundary statements travel with figures or the figures become wrong.** The operator water table is the sharpest case: separating a figure from "withdrawn" or "consumptive" turns four incomparable disclosures into a false ranking, which is the specific error the table was built to stop.
- **§6 is dated and says so.** It is current only through August 11, 2026, and the document states that legislation may change after the cutoff. It had already moved by 2026-08-16.

## Technical detail

Carried verbatim. The material a receiving side would otherwise have to reconstruct:

- **National and global electricity estimates with their bases** — LBNL's 2024 estimate and 2030 reference case and range, the IEA's 2025 estimate and 2030 projection with the global-share and emissions context, and the explicit statement that these are bottom-up models rather than meter censuses and cover all data centers rather than AI alone.
- **California-specific figures** — CEC total maximum-demand levels within the CAISO balancing area for 2040 in two scenarios, the CAISO *increase* figures for 2030 and 2040 that must not be substituted for them, the 67-percent utilization assumption with its correct attribution and PG&E's objection, and 2024 curtailment with the caution that curtailed energy is neither firm nor deliverable.
- **Per-task and per-query energy** — Google's median Gemini prompt figures with their boundary; a peer-reviewed median standard-query and long-reasoning pair; Mistral's lifecycle figures without electricity; the IEA's four indicative task values including the moderate-agent and reasoning-agent cases; the Hugging Face benchmark average and matched-model range; the coding-agent token ratios and their within-task variance; and a practitioner case whose electricity was modeled rather than metered.
- **Water** — national direct and indirect consumption with the indirect figure's generation-mix basis and its exclusion of power-purchase agreements and behind-the-meter generation; the roughly twelve-to-one ratio and why it is not a facility rule; the hydropower accounting problem left explicitly open for Hetch Hetchy; the corrected "bottle per query" figure; LBNL's modeled national water-use-efficiency values; four operator disclosures on four boundaries; peak-water capacity scenarios with facility peaking factors; a closed-loop operating example; the water-versus-carbon tradeoff finding; the free-cooling qualification with its underlying suitable-hours evidence; and the Southeast Plant and Westside project finding that makes eastside recycled-water cooling long-horizon.
- **Regulatory status** — one FERC show-cause proceeding and an abeyance motion, two CPUC proceedings, four California bills with thresholds and exclusions, and the enacted EU reporting and waste-heat regimes with their capacity thresholds.
- **The workload arithmetic** — the corpus's stated inputs, the four-step derivation to a peak throughput range, the demonstration that the published figure is a near-low-end selection, the midpoint that the same inputs would produce, and the warning against re-applying the token multiplier to a range that already includes input, reasoning, tool calls, and output.
- **The enterprise-evidence table** — six current public datasets, each with what it adds and why it cannot set the CCSF load.
- **The equipment conflict** — the rack-level GPU count that already exceeds the corpus's stated total, and the minimum physical total once the listed additional nodes are included.
- **Adoption and load sensitivity tables** — four adoption scenarios with daily-active share, inactive share, tasks per active user-day, and total daily tasks; and the same four scenarios converted to mean GPU load under two task-intensity assumptions, with an explicit statement of everything those figures exclude.
- **The cooling-water arithmetic** — three worked values at 5 MW, the reason PUE is not applied, the corpus figures they fail to reproduce, and an illustrative peak-day prorating that the document itself declines to treat as a design estimate.

## Public sources

The document cites its sources inline with resolvable URLs, and every figure in the body carries its citation at the point of use. Rather than duplicate roughly fifty citations, this table records the sources the document leans on hardest, since those are where a receiving side's own verification effort is best spent.

| Source title | Publisher or author | Publication date | URL and useful locator | Claim or finding supported | Verified date |
|---|---|---|---|---|---|
| US Data Center Energy Usage Report: 2025 Update | Lawrence Berkeley National Laboratory | 2026-06 | https://escholarship.org/uc/item/33m6w3x0 | §1, §3.1 — U.S. data-center electricity in 2024 and the 2030 reference case and range | Document's own, 2026-08-11 |
| US Data Center Energy Usage Report (LBNL-2001637) | Lawrence Berkeley National Laboratory | 2024-12 | https://eta-publications.lbl.gov/sites/default/files/2024-12/us_data_center_energy_usage_report_lbnl-2001637_0.pdf — pp. 56–58; Figure 4.7 | §5.1, §5.2 — direct and indirect water; modeled national water-use efficiency | Document's own, 2026-08-11 |
| Key Questions on Energy and AI | International Energy Agency | 2026 | https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary and the report PDF, Figure 2.1 and notes | §1, §3.1, §4.2 — global totals and the four indicative task energy values | Document's own, 2026-08-11 |
| Adopted 2025 Integrated Energy Policy Report | California Energy Commission | 2026 | https://efiling.energy.ca.gov/GetDocument.aspx?DocumentContentId=108996&tn=271454 — pp. 55–56 | §3.1 — California 2040 maximum data-center demand, mid and high cases. **Not independently verified** | Document's own, 2026-08-11 |
| Data center methodology memo, Supporting Document for the 2025 IEPR Forecast | California Energy Commission | 2026-04-15 | https://www.energy.ca.gov/sites/default/files/2026-04/Data_Center_Methodology_Memo_ada.pdf — printed pp. 7 and 15 | §3.2 — the 67-percent utilization factor, its SVP derivation, its application to requested capacity, and the worked example | **Re-verified 2026-08-16** |
| PG&E comments on the 2025 IEPR data center methodology | Pacific Gas and Electric Company | 2026 | https://efiling.energy.ca.gov/GetDocument.aspx?DocumentContentId=104787&tn=267761 — the passage is on PDF page 5 of 8; the filing has no printed pagination | §3.2, Appendix A — PG&E's objection that the factor is high-end and may not represent typical data centers | **Re-verified 2026-08-16; the document's own "pp. 4–5" locator is wrong** |
| Measuring the environmental impact of delivering AI at Google scale | Google | 2025-08 (May 2025 data) | https://services.google.com/fh/files/misc/measuring_the_environmental_impact_of_delivering_ai_at_google_scale.pdf | §4.1 — median Gemini prompt energy, emissions, and water; §5.2 — the 1.15 L/kWh consumptive figure | Document's own, 2026-08-11 |
| Joule paper on frontier-scale query energy | Oviedo et al. (Microsoft-authored) | 2026 | https://www.sciencedirect.com/science/article/pii/S2542435126001145 — DOI 10.1016/j.joule.2026.102430 | §4.1 — median standard query and long-reasoning case | Document's own, 2026-08-11 |
| AI Energy Score v2 | Hugging Face | 2026 | https://huggingface.co/blog/sasha/ai-energy-score-v2 | §4.2 — reasoning-cohort average and matched-model range | Document's own, 2026-08-11 |
| Coding-agent token study | Bai et al. | 2026-04 | https://arxiv.org/abs/2604.22750 | §4.2, §7.1 — coding-agent token ratios and within-task variance | Document's own, 2026-08-11 |
| Small Bottle, Big Pipe | Han et al. | 2026-03 | https://arxiv.org/abs/2603.02705 | §5.3 — peak public-water capacity scenarios and facility peaking factors | Document's own, 2026-08-11 |
| Making AI Less "Thirsty" | Li et al., Communications of the ACM | 2025-06 | https://doi.org/10.1145/3724499 | §5.1 — the corrected per-response water figure | Document's own, 2026-08-11 |
| Nature Reviews Clean Technology review | Nature Reviews Clean Technology | 2026 | https://www.nature.com/articles/s44359-026-00195-w | §5.3 — lowering water use can raise emissions in some configurations | Document's own, 2026-08-11 |
| Benefits of AI Openness | OECD | 2026-05 | https://www.oecd.org/content/dam/oecd/en/publications/reports/2026/05/benefits-of-ai-openness_40eaff39/746e8c9a-en.pdf — Table 3.1 | §7.1 — the enterprise-scale token-to-hardware comparator | Document's own, 2026-08-11 |
| Delegated Regulation (EU) 2024/1364 | European Union | 2024 | https://eur-lex.europa.eu/eli/reg_del/2024/1364/oj?locale=eng | §6 — enacted reporting thresholds and required metrics | Document's own, 2026-08-11 |
| Demand response issues and performance 2024 | California Independent System Operator | 2025-03-14 | CAISO publication, 26 pages | **Negative result.** Checked because a "4.5 GW of data-center demand" claim had been attributed to it. The report contains no instance of "4.5" and no instance of "data cent" in its extracted text | **Checked 2026-08-16** |

The remaining citations are in the body at the point of use and are not reproduced here.

## Alternatives and conflicting evidence

- **The document's central claim is a refusal, and refusals can be wrong.** It declines to supply a general agentic multiplier. The strongest case against that: a planning organization needs *some* number to size infrastructure, and "measure it first" is not available to anyone deciding a budget cycle now. The document's own answer is the six-point method in §7.1 plus the labeled sensitivity tables, which is a real alternative to a point estimate rather than a refusal to help — but a reader who needs one number will find the document unhelpful, and that is a genuine cost rather than a misreading.
- **The IEA task values carry more weight than their basis supports.** §4.2's structure depends on four indicative values from a single figure in one report — token-scaled, GPU-only scenarios using open-model benchmarks, which the document says plainly. The recommendation in §7.1 nonetheless proposes building a moderate-energy scenario from one of them. That is a thin foundation, and it is the same kind of thin foundation the document criticizes elsewhere. The mitigating difference is that it is labeled as a scenario input rather than an estimate.
- **The corpus arithmetic findings admit an innocent explanation, and the document says so unevenly.** For the cooling water it explicitly names the possibility of a different electricity boundary. For the 500,000–600,000 tokens-per-second figure it characterizes the published range as "a near-low-end case" selected "without saying so," which is a claim about how the number was chosen rather than about arithmetic. A defensible alternative reading: the original author applied an unstated adjustment and failed to document it, which is a documentation failure rather than a selection one. Either way the figure cannot be reproduced from its stated inputs, which is the operative point.
- **A single "typical worker" is not always the wrong model.** The document argues cohorts and daily-active share must be modeled separately, citing a 95th-percentile-to-median ratio of six. For reserved-capacity planning, a blended average with a peak factor is a conventional and defensible approach. The document's stronger version of this argument is not about statistics but about the eligible-versus-active distinction — applying any per-worker rate to all 5,000 workers assumes universal daily use, and that assumption is the one that fails.
- **Superseding a decision of record on a document's own authority is procedurally irregular.** §7.1 contains a blockquote stating that the review "supersedes" the session-state file's 20–30× sizing assumption for this note's method, while noting that the session-state file remains unchanged and conflicts. Under the governing precedence rule, dated decisions of record outrank documents. The document is right on the substance — the multiplier is unsupported — but the conflict is live on the work side and has not been resolved by amending the decision record. A receiving side should treat the multiplier as retired on the evidence and note that the corpus's own decision record still says otherwise.
- **Three blocks of the superseded document were dropped and not replaced.** See "Corrections and freshness triggers" below. Two of them were the only assessment the corpus had of sources it still cites.
- **The document is one tool and model's work, reviewed by nobody else.** It corrects a document produced by a different tool and model, which is a real form of independence, but no third pass has checked it. The one locator error found on spot-check was found by looking, not by process.

## Caveats and unresolved questions

- **§6 is stale by construction.** Current only through August 11, 2026, and it says so. Any bill status in it should be re-checked before use.
- **One page locator is wrong** — the PG&E comments citation. See "Independent verification" above. Substance unaffected; the locator is not.
- **Most of the document's citations were not independently re-verified.** The three that were are named above. Everything else carries the document's own 2026-08-11 verification.
- **The draft-to-final diff is unauditable** and the intermediate reasoning is gone. See "Provenance" above.
- **Appendix B's seven named omissions are load-bearing,** and three of them bear directly on CCSF decisions: Hetch Hetchy-specific water consumption under a defined allocation method, Digital Realty's current water-use efficiency at 200 Paul, and CCSF resource-adequacy, interconnection, power-supply, construction, and operating costs. The corpus has no other source for any of the three, and one of them — resource adequacy — is a cost line that a corpus cost table now carries as "not sized."
- **The hydropower water-accounting question is explicitly unresolved** for Hetch Hetchy Power, and it is the input a CCSF water conclusion most depends on.
- **The document supersedes a decision of record on its own authority** and leaves the conflict live. See above.
- **It marks itself "Internal research note."** That marking is superseded by the 2026-08-11 disclosure decision but travels verbatim in the body; it describes the document's original classification, not its current one.
- **It names a work-side internal file** — `claude_session_state.md` — in the §7.1 blockquote, and characterizes one assumption that file records. Flagged at the disclosure gate below rather than decided here.
- **Its relative links to sibling corpus files will not resolve** where the file sits alone. See integration guidance.
- **Not assessed:** whether a personal-side counterpart exists under this filename, and if so which of the two documents it is. Everything in the integration guidance is contingent on that.

## Corrections and freshness triggers

### What the substitution dropped

Three blocks of the superseded document were not carried into the replacement. Their absence has consequences that are already visible elsewhere in the corpus:

1. **A source evaluation of an MIT publication** (superseded §2, 42 lines). Nothing in the corpus now evaluates that source.
2. **An assessment of *Power 2026* (Somani), including a fact-check of it and the reasoning against a coal-and-diesel recommendation it contained** (superseded §7, 91 lines). This is the costliest loss. The corpus still cites that book as the sole support for treating resource adequacy as a recurring load-serving-entity obligation, and the replacement's Appendix B lists CCSF resource-adequacy cost as an explicit omission — so the citation now stands unassessed, and it is marked as such in the companion deep dive. The dropped reasoning against the coal-and-diesel recommendation is not recorded anywhere else in the corpus.
3. **A corpus-change list** (superseded §8, 23 lines), largely superseded in function by the replacement's Appendix A, which is more systematic. This loss is the least consequential; the replacement's version is better.

Whether to port any of the three back is an open work-side decision, recorded here because a receiving side integrating this document inherits the same gap.

The replacement also **removed a corroborating cross-reference for the TeraWulf $271/MWh figure**, which now rests on the primary company release alone in the companion deep dive.

### What Appendix A's nineteen rows produced in the corpus

The rows were worked as a scoped pass on the work side on 2026-08-16 and committed at `18174da`. The disposition is recorded here because a receiving side holding the same corpus documents faces the same nineteen decisions:

- **Eleven became edits** across five corpus documents: the misidentified 4.5 GW figure (retired on the primary check described above); California curtailment (an unverifiable April 2026 record retracted); the scope of national totals (marked all-data-center, not AI); water-use efficiency (four operator figures marked as sharing no boundary, with the consumptive figure shown to sit above the national modeled range rather than below it); the agentic multiplier and throughput (retired as a central estimate); worker adoption and use distribution; CCSF equipment and electricity (the GPU-count conflict); facility scale; CCSF cooling water; Southeast Plant recycled water; the California bills; and the sensitive-workload share.
- **Four needed no edit** because the corpus already satisfied them: the San Francisco free-cooling figure was already stated as a modeled inference; the CCSF planning population was already framed as a planning choice; the enterprise-scale comparator was new material with nothing to correct; and the superseded California demand figures existed only in the superseded document, not in the corpus.
- **Three were deliberately left as flags rather than reversals:** the workload-scheduling row, whose midday-versus-overnight recommendation would reverse standing CCSF guidance; a water-use-efficiency procurement target, recorded as suspended rather than carried forward; and the residual equipment and power arithmetic. Reversing a standing recommendation was left to Jeremy rather than executed.

Three items in Appendix A were **not** independently re-verified when they were acted on: the identification of the 4.5 GW figure as planned offshore wind (corroborated against the corpus's own offshore-wind capacity figure but not re-sourced), the demand-response values in the CAISO report that preceded the retired clause, and AB 2619's status.

### Freshness triggers

Re-verify when: any California bill in §6 moves — **this has the shortest fuse of anything in the document, and three of the four bills were on Appropriations suspense at the cutoff**; the CPUC rules in R.26-04-009 or completes the SB 57 assessment due January 1, 2027; FERC acts in EL26-71 or rules on CAISO's abeyance motion; the CEC adopts a later IEPR cycle or rules on PG&E's request to differentiate the utilization factor; LBNL publishes a further update, particularly any treatment of power-purchase agreements in indirect water; the IEA revises its task-energy figure, which would ripple through the whole reasoning-and-agents section; any of the four named operators publishes a new water figure on a stated boundary, or Digital Realty publishes one for the first time; the EU adopts the draft rating regulation that was still in feedback at the cutoff; a CCSF pilot produces measured workload data, which would retire most of §7.1; or hydropower water accounting becomes available for the Hetch Hetchy system.

## Integration guidance

**Destination role.** Land the embedded document as the corpus's energy and water evidence base in the personal side's `CCSF-compute/` subdirectory. Suggested name, matching the work-side original: `CCSF_ai_energy_water_evidence_2026-08-11.md`.

**If a personal-side counterpart already exists under this filename**, compare its digest first:

- `48e5dceb0cb31e9501428d7ed0e8269af89ecbd8b1dd41ed837f1d8f41a83760` — already current; no action.
- `57bf887e072ebd0719fbbc5e98cb3d4b2774a43e227c1873d3f794735d61dbad` — **the superseded document.** Replace it wholesale with the embedded body. Do not diff and merge: these are two different documents that happen to share a filename, and a merge would produce a document with two incompatible section-numbering schemes. Then check every cross-reference elsewhere in the destination corpus that cites this filename by section, because those pointers were written against the old numbering and will now resolve to the wrong sections.
- **Neither** — either the destination has independent divergence, or it holds an older evidence document under a different name. In either case do not merge. Land this document as new content and treat reconciliation of any prior evidence file as a separate decision.

**The cross-reference hazard is the main integration risk, and it is worse than a broken link.** The superseded document and the replacement use different section numbers for related material. A pointer written as "§4.1" against the old document will resolve to a real but wrong section in the new one. On the work side this required repairing twelve live analytical pointers across five documents, of which four turned out to have misstated what the old source said. If the destination corpus cites this file by section anywhere, budget for that pass rather than assuming the replacement is drop-in.

**Relative links.** The body contains relative links of the form `./CCSF_public_compute_strategic_brief.md` in Appendix A and its closing source list. They resolve only where the sibling corpus files are present in the same directory. They will not resolve in this export repository, and they will resolve in the destination only if the corpus is landed together. This is expected and is not a defect in the body; do not rewrite them.

**Expected transformations: none.** Transfer the body byte-exact. Do not condense Appendix A, do not collapse its status labels into a single "corrected," and do not separate any figure from the boundary stated alongside it. Preserve the document's own status line and Appendix B verbatim: the status line records that CCSF figures are planning scenarios rather than forecasts, and Appendix B is the list of what the document's silence does not imply.

**Sequencing.** Land this document **first or simultaneously with the companion SFPUC deep-dive packet.** Every correction note in that document cites this one by filename and section. If the destination holds the superseded document under this filename, those citations will resolve to wrong sections rather than to nothing.

**Approval sequence.** Disclosure gate (Jeremy reviews this exact public packet) → publish to `jp-sfgov/sfgov-cleared-research-export` → integration gate (Jeremy reviews the exact personal-side destination diff and the ledger entry) → personal-side commit → ledger update.

**Destination-specific framing that should remain distinct.** The document's §7 reasons from CCSF's specific institutional position — a 5,000-worker eligible cohort, a municipal facility scenario, SFPUC water and power, the Southeast Treatment Plant, and 200 Paul. That is the work side's context and its set of obligations. The general evidence in §§1–6 is portable; the CCSF application in §7 is not, and its figures are planning scenarios rather than forecasts or approved plans. The non-authorization framing travels with the document.

## Exclusions and disclosure boundary

**Excluded from this packet:** work-side repository history and commit graph beyond the commit IDs cited for provenance; the work-side session state and its internal decision record; the internal correction-implementation and inbound-integration working records, which name staff and quote internal directives and which deliberately retain their own internal/no-share classification because the 2026-08-11 decision covers the research corpus rather than working records; prior-session transcripts; raw intake; the deleted scratch proposal directory in which this document was drafted; reader and essentials build artifacts and build scripts; credentials and secrets; any Level 3–5 City data; and the work-side operating context (local filesystem paths, git-metadata locations, remote configuration, device details).

**Verification performed on the transferred body.** Scanned against a named checklist. Clean on: credential and key patterns, local filesystem paths, cloud-storage and git-metadata paths, personal email addresses, personal-only audience markers, Level 3–5 classification markers, City staff names, and any reference to the depersonalized external contact or to a depersonalized utility staff individual. The checklist enumerates the specific names and identifiers being screened for and is therefore not reproduced in this public packet — reproducing it would publish exactly what it screens out.

**Two checklist categories are present rather than absent. Both are judgment calls for the disclosure gate rather than findings, and neither is resolved here.**

1. **The body names a work-side internal file and characterizes its content.** The §7.1 blockquote names `claude_session_state.md` and states that it records the 20–30× multiplier as the load-bearing sizing assumption, that this review supersedes it for the note's method, and that the file remains unchanged and conflicting. Nothing from inside that file is quoted, and no decision text, staff name, or internal directive is reproduced — what travels is a filename and one characterized assumption, in the course of disclosing a conflict rather than concealing it. The tension: the export charter's never-disclosure-eligible list includes session records, and the session-state file is a session handoff record even though it is not a transcript. The narrow reading is that this is a corpus document's own text about a conflict, cleared by the 2026-08-11 decision, and that disclosing a conflict is better practice than hiding it. The cautious reading is that it points a public reader at the existence and content of an internal decision record. **Recorded for Jeremy's call at the disclosure gate.** If the call is to remove it, the fix belongs upstream in the work-side source, not in this wrapper — modifying the packet would break byte-exactness and convert a verbatim transfer into a modified one.
2. **The body marks itself "Internal research note."** That marking is superseded by the 2026-08-11 disclosure decision, which cleared the entire corpus for full unabridged disclosure through this channel. It travels verbatim because the transfer is byte-exact. A reader encountering it may reasonably wonder whether the document was cleared. It was — the marking records its original classification, not its current one. Recorded so that the apparent contradiction is explained here rather than left to inference.

**Structural exclusions that apply regardless of clearance scope**, per this export repository's charter: credentials, raw intake, session transcripts and records, repository history, and Level 3–5 data are never disclosure-eligible.

## Closeout

- **Public export commit:** `d02857f20318b779ced2d0bb43c92a6a9124e160` — "Publish two cleared outbound research packets (work -> personal)," 2026-08-16, SSH-signed, signature verified good. This packet and its companion were published in that single commit. *(Filled in 2026-08-16; the field previously read "pending disclosure gate," which was left stale at publication and is corrected here.)*
- **Destination content commit or commits:** (pending — personal side)
- **Ledger or manifest commit:** `9732b02` in the private work repository — the sending side's sync-ledger entry recording this packet, its body digest, and the post-commit round-trip verification. Not publicly readable; recorded for traceability.
- **Amendment, 2026-08-16 — one item under "Unresolved differences" below has since been resolved and its text is left standing rather than rewritten.** That paragraph states that the embedded document "supersedes a decision of record on its own authority, leaving that conflict live on the work side." Later the same day Jeremy retired the 20–30× agentic-token multiplier as a decision of record on the work side, so the conflict is closed by retirement rather than left live. The embedded body still describes it as live because the body is byte-exact and was not edited; §7.1's characterization of the work-side session-state file is therefore accurate as of the body's own source commit and stale as of this amendment. Nothing in the body's analysis depends on the conflict remaining open — §7.1 argues for replacing the point estimate with scenarios, which is the direction the retirement took.
- **Unresolved differences:** Two items are open for the disclosure gate itself and are named above — the internal-filename reference and the internal-note marking. Whether a personal-side counterpart exists, and which of the two documents it is, is unknown to the sending side; the integration guidance branches on that. Open on the substance: §6's bill statuses are stale by construction; one page locator is wrong; most citations were not independently re-verified; the draft-to-final diff is unauditable; the hydropower water-accounting question is unresolved; three of Appendix B's seven omissions bear directly on CCSF decisions and have no other source in the corpus; and the document supersedes a decision of record on its own authority, leaving that conflict live on the work side. Open on the work side and outside this packet's body: whether to port the three dropped blocks, the disposition of generated reader artifacts and PDFs now stale against these corrections, and two stale pointers in the work-side session state. All of those are excluded from disclosure by the paragraph above and cannot leak through this channel.

## Completion checklist

- [x] The receiving agent can understand, verify, and integrate the cleared research without access to the originating private files — the full body is embedded with its own inline citations, and the substitution, the dropped blocks, and the cross-reference hazard are documented.
- [x] All eligible substantive detail, links, context, reasoning, caveats, corrections, and provenance were preserved. Nothing was condensed; Appendix A's nineteen rows and their status labels, Appendix B's seven omissions, and the document's own status line are intact.
- [x] Facts, analysis, inference, and recommendations are distinguishable — the document's §2 conventions govern the body, the orientation table maps status by section, and this wrapper separates the document's own verification from the three claims re-checked independently.
- [x] Every decisive claim is traceable to a public source or explicitly identified reasoning; the unverified figures are named as unverified, the wrong locator is named as wrong, the unauditable provenance is named as unauditable, and the dropped assessments are named as dropped.
- [x] Raw intake and private, restricted, or otherwise ineligible context were excluded.
- [x] Safe source commit is recorded — `a98b8bb`, verified byte-equal to the stated digest, with the superseded document at `c686b13` recorded for comparison. Destination commit pending the integration gate.
- [x] Jeremy reviewed the exact public diff and affirmatively cleared it for public disclosure, including the two judgment calls named under "Exclusions and disclosure boundary."

---

## Extracting the body

Everything below the delimiter line is the source document, byte-exact, including its own H1 and heading levels. To verify or extract:

```
awk 'f{print} /^<!-- BEGIN VERBATIM/{f=1}' <this-file> \
  | sed '$d' > CCSF_ai_energy_water_evidence_2026-08-11.md
shasum -a 256 CCSF_ai_energy_water_evidence_2026-08-11.md
# expect 48e5dceb0cb31e9501428d7ed0e8269af89ecbd8b1dd41ed837f1d8f41a83760
```

The document's own heading levels are preserved rather than demoted, so that quoted section anchors (§3.2, §4.2, §5.2, §7.1, §7.2, Appendix A, Appendix B) resolve exactly as they do in the original.

<!-- BEGIN VERBATIM DOCUMENT: CCSF_ai_energy_water_evidence_2026-08-11.md · SHA-256 48e5dceb0cb31e9501428d7ed0e8269af89ecbd8b1dd41ed837f1d8f41a83760 -->
# AI Energy and Water: Current Evidence and CCSF Implications

```table-of-contents
```

*Codex · GPT-5 · 2026-08-11*

**Status:** Internal research note. Evidence is current through August 11, 2026. The external claims below have been checked against current primary sources and subjected to an assume-false review. CCSF workload and facility figures remain planning scenarios, not forecasts or approved plans.

---

## 1. Executive summary

AI is adding a large new source of electricity demand, but the scale depends on what is being counted. National and global totals generally cover all data centers, not AI alone. Per-query estimates cover particular models and tasks and cannot be multiplied into a citywide forecast without measuring how people actually use the systems.

Lawrence Berkeley National Laboratory (LBNL) estimates that U.S. data centers used **192 terawatt-hours (TWh), or 4.7% of U.S. electricity, in 2024**. Its 2030 reference case is **649 TWh, or 11.8%**, with a modeled range of **521–843 TWh, or 9.5%–15.3%**. These are bottom-up estimates based on equipment, facilities, and operating assumptions—not a census of utility meters and not an AI-only total. [LBNL 2025 Update](https://escholarship.org/uc/item/33m6w3x0)

Globally, the International Energy Agency (IEA) estimates data-center electricity use at about **485 TWh in 2025** and projects about **950 TWh in 2030**, when data centers would use roughly **3% of global electricity**. AI-focused data-center use is projected to triple. Data centers would still account for less than 1% of global carbon dioxide emissions in the IEA base case, but their loads are concentrated in particular regions and can be large enough to change local generation, transmission, and ratepayer costs. [IEA 2026 executive summary](https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary), [IEA energy-supply analysis](https://www.iea.org/reports/energy-and-ai/energy-supply-for-ai)

Ordinary text inference can use a few tenths of a watt-hour per query in the best public evidence. Longer reasoning and agentic work can use far more because it processes many more tokens and makes repeated model calls. Published energy comparisons range from a few-fold to hundreds-fold, depending on the model, task, settings, hardware, caching, and measurement boundary. The evidence reviewed does not establish a universal multiplier for municipal office work. CCSF must measure its own workloads before using a multiplier to size infrastructure.

Water has two main components. LBNL estimates that U.S. data centers consumed about **66 billion liters (17.4 billion gallons) onsite in 2023**, primarily for cooling, and nearly **800 billion liters (about 211 billion gallons) indirectly through electricity generation**. The national modeled ratio is about twelve to one, but it varies with location, cooling design, and power supply. Local planning must also address peak-day demand: a modest annual total can still require large pipes and treatment capacity during hot periods. [LBNL 2024 report, pp. 56–58](https://eta-publications.lbl.gov/sites/default/files/2024-12/us_data_center_energy_usage_report_lbnl-2001637_0.pdf)

The existing City and County of San Francisco (CCSF) scenario effectively treats all 5,000 eligible workers as active at 24–64 agent tasks per worker-day, then states **400–600 kilowatts (kW) of information-technology load** and **4.2–6.3 gigawatt-hours (GWh) per year** at a power usage effectiveness (PUE) of 1.2, meaning 20% facility overhead beyond the information-technology load. The electricity arithmetic is sound only after the 400–600 kW input is accepted. The worker-to-load chain is not: the listed workload inputs imply a **375,000–6.67 million tokens-per-second** peak, and the equipment list conflicts with its stated graphics-processing-unit (GPU) count. The public enterprise datasets reviewed show rapid growth and highly uneven use, but do not provide a representative absolute load per worker. Retain 5,000 workers as the eligible planning cohort; model the daily-active share and user cohorts separately before procurement.

### What changed since the Inflation Reduction Act

The Inflation Reduction Act became law on **August 16, 2022**, before ChatGPT's public release on **November 30, 2022**. It arrived near the end of roughly fifteen years of nearly flat U.S. electricity demand; the pre-Act outlook expected annual growth below 1% for much of the period through 2050. Federal modeling later estimated that the Act and the 2021 infrastructure law could produce **72%–81% clean electricity in 2030** and reduce net U.S. greenhouse-gas emissions to **35%–41% below 2005 levels**. Those were conditional scenarios, not guarantees. [Congress.gov](https://www.congress.gov/bill/117th-congress/house-bill/5376/titles), [OpenAI](https://openai.com/index/chatgpt/), [EIA 2022](https://www.eia.gov/outlooks/aeo/narrative/pdf/AEO2022_Narrative.pdf), [DOE modeling](https://www.energy.gov/policy/articles/investing-american-energy-significant-impacts-inflation-reduction-act-and)

Since then, AI-driven demand has expanded, while the Trump administration and Public Law 119-21, the 2025 budget reconciliation law, have reduced federal support for new clean supply. These developments affect emissions through different channels and at different scales. LBNL estimates that electricity used by all U.S. data centers—not AI alone—rises from **192 TWh in 2024 to 649 TWh in 2030**, increasing their national share from 4.7% to 11.8%. In one stress test, Rhodium Group's high data-center-demand case raised 2035 power-sector emissions **6%–13%** and total grid-system costs **13%–15%** above its baseline demand case. In a separate Rhodium run, the reconciliation law produced more than half fewer new clean-power capacity additions through 2035, **315–574 million metric tons more economy-wide greenhouse-gas emissions in 2035**, and power-sector emissions **19%–79% higher** than its no-law case. That no-law case already assumed major federal regulatory rollbacks, so the estimates isolate the reconciliation law rather than the Trump administration's total policy effect. [LBNL 2025 Update](https://escholarship.org/uc/item/33m6w3x0), [Rhodium data-center analysis](https://rhg.com/research/data-centers-electricity-demand/), [Rhodium final-law analysis](https://rhg.com/research/assessing-the-impacts-of-the-final-one-big-beautiful-bill/)

These are separate model runs with different baselines, scopes, and outputs. They cannot be added or used to rank the magnitude of AI demand against the reconciliation law. Together they show two distinct pressures: added electricity demand and reduced federal support for clean supply. Concentrated data-center projects can still dominate a local grid. AI adds load, while policy helps determine whether new demand is met by clean power or by running and building more fossil generation. Some rollbacks lower electricity demand by slowing vehicle electrification, but they shift energy use back to gasoline and raise total emissions rather than providing a clean offset. The Trump administration also repealed federal vehicle greenhouse-gas standards in February 2026; repeal of the 2024 power-plant carbon standards remained proposed at this note's cutoff. [U.S. Environmental Protection Agency vehicle action](https://www.epa.gov/regulations-emissions-vehicles-and-engines/final-rule-rescission-greenhouse-gas-endangerment), [U.S. Environmental Protection Agency power-plant rule status](https://www.epa.gov/stationary-sources-air-pollution/greenhouse-gas-standards-and-guidelines-fossil-fuel-fired-power)

Clean-energy construction continues: wind and solar, including small-scale solar, supplied **19% of U.S. electricity in 2025**, and developers planned a record **86 GW** of new utility-scale capacity for 2026, mostly solar, batteries, and wind. But major wind and solar tax credits now expire sooner, and the U.S. withdrawal from the Paris Agreement took effect in January 2026. Globally, current policies point to about **2.8°C of warming**, not a Paris-aligned carbon-neutral trajectory. AI did not create that gap, but it makes the infrastructure task harder. California remains on a separate statutory path to **100% renewable and zero-carbon retail electricity by 2045** and reported 67% clean retail electricity in 2024. [EIA 2025 generation](https://www.eia.gov/TODAYINENERGY/detail.php?id=67367), [EIA 2026 capacity additions](https://www.eia.gov/todayinEnergy/detail.php?id=67205), [Congressional Research Service](https://www.congress.gov/crs-product/R48611), [UNFCCC](https://unfccc.int/node/61231), [UNEP 2025](https://www.unep.org/resources/emissions-gap-report-2025), [California Energy Commission](https://www.energy.ca.gov/data-reports/clean-energy-serving-california)

---

## 2. Reading the evidence correctly

Four categories should not be blended:

| Term | Meaning in this note |
|---|---|
| **Observed** | Metered or reported operating data for a defined facility, fleet, or grid. |
| **Estimated** | A model of current or past use where complete measurement is unavailable. |
| **Projected** | A model of future use under stated assumptions. |
| **Scenario** | An internally selected planning case used to test consequences; it is not a prediction. |

The system boundary matters just as much as the number. Information-technology electricity excludes cooling and power conversion unless facility overhead is added. Water withdrawal includes water returned to the source; consumption is the portion not returned, usually because it evaporates. An AI prompt, an agentic task, a user session, and a worker-day are different units.

This note gives greatest weight to government and national-laboratory work, then peer-reviewed studies and open measurement. Vendor disclosures are retained only with their boundaries. Preprints and practitioner cases are used as emerging or illustrative evidence, not as settled baselines.

---

## 3. Energy scale and trajectory

### 3.1 Current top-level estimates

| Geography and metric | Current estimate | What it covers |
|---|---:|---|
| United States, 2024 | **192 TWh; 4.7%** | LBNL estimate for all data centers. |
| United States, 2030 reference | **649 TWh; 11.8%** | LBNL projection for all data centers. |
| United States, 2030 range | **521–843 TWh; 9.5%–15.3%** | LBNL compounded-uncertainty range. |
| Global, 2025 | **About 485 TWh** | IEA estimate for all data centers. |
| Global, 2030 | **About 950 TWh; about 3%** | IEA projection; AI-focused use triples. |
| California, 2040 mid/planning case | **About 5,800 MW** | California Energy Commission (CEC) maximum data-center demand within the CAISO balancing area, including existing load. |
| California, 2040 high/local-reliability case | **About 8,400 MW** | CEC high scenario within the CAISO balancing area, including existing load; not the planning case. |

Sources: [LBNL 2025 Update](https://escholarship.org/uc/item/33m6w3x0), [IEA 2026](https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary), [adopted 2025 Integrated Energy Policy Report, pp. 55–56](https://efiling.energy.ca.gov/GetDocument.aspx?DocumentContentId=108996&tn=271454).

The national totals do not isolate AI. They include conventional computing, storage, networking, cloud services, and cryptocurrency activity where it falls within the report's data-center definition. The future range is wide because equipment shipments, server power, utilization, efficiency, construction, and interconnection timing are uncertain.

### 3.2 California grid context

The California Independent System Operator (CAISO) reports that the CEC forecast used for its planning adds **1.8 GW of data-center load by 2030 and 4.9 GW by 2040** within the CAISO balancing area. These are increases, while the CEC figures above are total maximum-demand levels in the same area and include existing load. They cannot be substituted for one another. The **4.5 GW** figure previously attributed to data centers in the corpus actually refers to planned offshore wind and should not be reused. [CAISO July 2026 informational report](https://www.caiso.com/documents/jul-20-2026-informational-report-large-loads-and-co-located-loads-el26-71.pdf), [CAISO transmission plan](https://www.caiso.com/documents/board-approved-2025-2026-transmission-plan.pdf)

The CEC converts requested interconnection capacity into expected maximum operating demand using a **67% utilization assumption derived from Silicon Valley Power operating data**. It is not a PG&E average. PG&E told the CEC that the factor is high-end and may not represent typical data centers. Requested capacity is therefore not the same as forecast demand. [CEC methodology memo](https://www.energy.ca.gov/sites/default/files/2026-04/Data_Center_Methodology_Memo_ada.pdf), [PG&E comments](https://efiling.energy.ca.gov/GetDocument.aspx?DocumentContentId=104787&tn=267761)

CAISO curtailed **3.4 million megawatt-hours (MWh)** of wind and solar in 2024, 29% more than in 2023; solar accounted for 93%. This establishes that substantial renewable generation is sometimes unavailable to the market. It does not establish that the energy is firm, deliverable to a particular data center, or available when an interactive workload needs it. Hourly and locational analysis would be required. [EIA using CAISO data](https://www.eia.gov/todayinenergy/detail.php?id=65364)

---

## 4. From a prompt to an agentic workflow

### 4.1 What ordinary-query estimates show

Google estimates that a median Gemini Apps text prompt used **0.24 watt-hours (Wh)**, emitted **0.03 grams of carbon-dioxide equivalent**, and consumed **0.26 milliliters of onsite water** in May 2025; the paper was released in August 2025. Its electricity boundary includes accelerators, host processors and memory, idle capacity, and facility overhead. It remains a first-party estimate using an undisclosed production workload. [Google technical paper](https://services.google.com/fh/files/misc/measuring_the_environmental_impact_of_delivering_ai_at_google_scale.pdf)

Oviedo and coauthors model a median **0.31 Wh per standard query** for a defined frontier-scale serving configuration and **3.91 Wh** for a long, roughly 5,000-output-token reasoning case—about 13 times the standard case. The study is peer reviewed and openly documented, but it is Microsoft-authored modeling rather than an independent measurement of closed production systems. [Joule, DOI 10.1016/j.joule.2026.102430](https://www.sciencedirect.com/science/article/pii/S2542435126001145)

Mistral reports **1.14 grams of carbon-dioxide equivalent and 45 milliliters of water** for one 400-token Le Chat response. It does not report electricity. Its lifecycle boundary is broader than Google's onsite operating boundary, so the figures should not be ranked against each other. [Mistral lifecycle assessment](https://mistral.ai/news/our-contribution-to-a-global-environmental-standard-for-ai/)

These examples establish that some ordinary text queries use electricity measured in tenths of a watt-hour. They do not establish a universal per-query value or a basis for CCSF sizing.

### 4.2 Reasoning and agents

The IEA's 2026 indicative model puts GPU electricity at **0.31 Wh** for large-model text generation, **1.14 Wh** for reasoning, **7.6 Wh** for a moderate agentic task with four to six sequential calls, and **50 Wh** for an agentic task with reasoning. The 7.6 Wh case is about 25 times the figure's large-model text case, but it is not a matched-model multiplier and does not validate CCSF's 20–30× *token* assumption. The IEA values are token-scaled, GPU-only scenarios using open-model benchmarks, not measurements of enterprise workers or optimized production systems. [IEA, Figure 2.1 and notes](https://iea.blob.core.windows.net/assets/3179f7f8-01f6-4dd6-bffa-c9f7b73f1dc9/KeyQuestionsonEnergyandAI.pdf)

Hugging Face's open AI Energy Score v2 benchmark reports an average **30×** increase across its tested reasoning cohort, with matched-model results from **154× to 697×** in selected cases. The benchmark measures GPU energy for open models under controlled prompts, not full-facility production energy. It demonstrates variability, not a universal “reasoning multiplier.” [Hugging Face AI Energy Score v2](https://huggingface.co/blog/sasha/ai-energy-score-v2)

Bai and coauthors report that coding agents used about **1,200× more tokens than multi-round code chat and 3,500× more than single-round code reasoning** on SWE-bench Verified. Individual runs on the same task varied by as much as 30×. These are comparisons among different coding-task constructs, not a general agent multiplier. The April 2026 preprint measures tokens, not electricity. Input dominates its million-token trajectories; in the paper's Claude Sonnet 4.5 example, cache reads dominate. Those tokens cannot be divided by an output-tokens-per-second benchmark to size GPUs. [Bai et al. preprint](https://arxiv.org/abs/2604.22750)

In an illustrative practitioner case, Zeke Hausfather logged 1,138 typed prompts, more than 14,000 model calls, 3.2 billion tokens, and 96% cache-read tokens over eight weeks of heavy coding-agent use. He then **modeled**, rather than metered, electricity at 70–330 kWh, with a 170 kWh central estimate. The case is useful for understanding workload shape but is not a population estimate. [The Climate Brink](https://www.theclimatebrink.com/p/the-real-energy-use-of-agentic-ai)

Watershed and coauthors propose a useful corporate accounting method based on spend, token activity, or provider data. Their task ranges and hypothetical-company example are illustrative rather than observed enterprise workloads. The paper itself says provider data remain incomplete and that non-production benchmarks can overstate optimized production energy by 4–20 times. [Watershed white paper](https://cdn.sanity.io/files/3ogo9b9g/production/a5c1f64ca5864e61b47e6384ee4d0ed31bc861f4.pdf), [open preprint](https://arxiv.org/abs/2608.06733)

**Conclusion:** reasoning and agentic workflows can use substantially more computation than ordinary chat, but the reviewed evidence does not provide a defensible general multiplier for CCSF. Measurement should separate workload class, model, uncached input, cache writes, cache reads, output and reasoning tokens, tool calls, latency, concurrency, and time of day.

---

## 5. Water and cooling

### 5.1 National scale

| 2023 U.S. data-center water estimate | Amount | Boundary |
|---|---:|---|
| Direct onsite consumption | **66 billion liters / 17.4 billion gallons** | Primarily evaporative cooling. |
| Indirect electricity-related consumption | **Nearly 800 billion liters / about 211 billion gallons** | Regional generation mix for 176 TWh; excludes facility power-purchase agreements and behind-the-meter generation. |

Source: [LBNL 2024 report, pp. 56–58](https://eta-publications.lbl.gov/sites/default/files/2024-12/us_data_center_energy_usage_report_lbnl-2001637_0.pdf).

The indirect estimate is about twelve times the direct estimate nationally, but the ratio is not a universal facility rule. It changes with the electricity supply, climate, and cooling system. Hydropower water accounting is especially sensitive to whether reservoir evaporation is allocated to power, water supply, flood control, or other uses; this note does not resolve that question for Hetch Hetchy Power.

The widely repeated “500-milliliter bottle per query” claim is wrong. The peer-reviewed GPT-3-era model estimated about 500 milliliters for roughly **10–50 medium-length responses**, depending on where and when the model ran. It is useful as a warning about system boundaries, not as a current per-query estimate. [Communications of the ACM](https://doi.org/10.1145/3724499)

### 5.2 Operator disclosures are not a ranking

LBNL's national model put average direct water-use efficiency just above **0.36 L/kWh through 2023** and projected roughly **0.45–0.48 L/kWh** afterward as liquid cooling expanded. It is a modeled national average for all data centers, not a performance standard for a new facility. [LBNL 2024 report, Figure 4.7](https://eta-publications.lbl.gov/sites/default/files/2024-12/us_data_center_energy_usage_report_lbnl-2001637_0.pdf)

| Operator | Reported water-use efficiency | Boundary |
|---|---:|---|
| AWS | **0.12 L/kWh, 2025** | Water withdrawn per IT kWh; global first-party fleet figure. |
| Meta | **0.19 L/kWh, 2024** | Water withdrawn per IT kWh; global first-party fleet figure. |
| Microsoft | **0.27 L/kWh, FY2025** | Cooling and humidification water at owned and controlled sites operating for at least 12 months. |
| Google | **1.15 L/kWh, 2023–2024 study basis** | Consumptive WUE for data centers supporting large-language-model workloads; not identified as a fleet-wide figure. |

Sources: [AWS](https://aws.amazon.com/sustainability/), [Meta environmental data index](https://sustainability.atmeta.com/wp-content/uploads/2025/10/Meta_2025-Environmental-Data-Index.pdf), [Microsoft](https://datacenters.microsoft.com/sustainability/efficiency/), [Google technical paper](https://services.google.com/fh/files/misc/measuring_the_environmental_impact_of_delivering_ai_at_google_scale.pdf).

These values use different years, climates, portfolios, and definitions. Some measure withdrawal and others consumption. They cannot support a claim that one operator is two to four times “better,” and they should not be converted directly into a CCSF procurement threshold.

### 5.3 Peak demand and cooling choices

The *Small Bottle, Big Pipe* preprint models **697–1,451 million gallons per day** of new U.S. peak public-water capacity through 2030 if 2024 water intensity persists. An optimistic scenario with 10% annual efficiency improvement lowers the modeled range to **227–604 million gallons per day**. The paper says facility peaking factors often reach six and sometimes exceed ten. These are scenarios for direct public-water withdrawal, not a forecast of observed future use. [Han et al. preprint](https://arxiv.org/abs/2603.02705)

Microsoft's Fairwater facility in Mount Pleasant, Wisconsin, became fully operational on June 23, 2026. Microsoft says its facility-wide closed loop continuously reuses cooling liquid without evaporation; the liquid is replaced only if water chemistry indicates a need, and the system is designed for six or more years between fills. This is an operating first-party example, but it does not eliminate water associated with electricity generation. [Microsoft operating announcement](https://news.microsoft.com/source/2026/06/23/microsoft-completes-construction-on-first-datacenter-facility-in-mount-pleasant-wisconsin/), [design description](https://blogs.microsoft.com/blog/2025/11/12/infinite-scale-the-architecture-behind-the-azure-ai-superfactory/)

Cooling decisions can trade water for electricity and carbon. A 2026 peer-reviewed review finds that lowering water use can increase emissions in some configurations. The correct objective is therefore not “zero water” in isolation, but the lowest combined effect under local climate, grid, and water conditions. [Nature Reviews Clean Technology](https://www.nature.com/articles/s44359-026-00195-w)

San Francisco's cool climate is favorable for airside or dry cooling, but the corpus's **about 95% free-cooling** figure is a modeled inference, not a measurement from an operating San Francisco facility. The underlying sources indicate more than 8,500 potentially suitable hours under the wider American Society of Heating, Refrigerating and Air-Conditioning Engineers (ASHRAE) allowable envelope and nearly year-round airside contribution, subject to humidity and equipment limits. [Green Grid WP#46](https://datacenters.lbl.gov/sites/default/files/WP46UpdatedAirsideFreeCoolingMapsTheImpactofASHRAE2011AllowableRanges.pdf), [LBNL economizer study](https://www.osti.gov/servlets/purl/937579)

The U.S. Environmental Protection Agency's (EPA's) Water Reuse Action Plan 2.0 calls for work with states and regulated parties on permitting best practices for recycled water in industrial and data-center cooling. It is not a permit, mandate, funding award, or finding that an eastside San Francisco project is feasible. The Southeast Treatment Plant currently produces disinfected secondary effluent, not a distributable tertiary supply for data-center cooling, and the funded Westside Enhanced Water Recycling Project serves the west side. Recycled-water cooling near the Southeast Plant should therefore remain a long-horizon option. [EPA WRAP 2.0](https://www.epa.gov/waterreuse/water-reuse-action-plan-20), [SFPUC liquid treatment](https://www.sfpuc.gov/about-us/our-systems/sewer-system/treating-liquid-flows), [SFPUC Westside project](https://www.sfpuc.gov/construction-contracts/construction-projects/westside-enhanced-water-recycling-project)

---

## 6. California policy and ratepayer context

The following status is current only through **August 11, 2026**:

| Matter | Current status | Relevance |
|---|---|---|
| FERC EL26-71 | The Federal Energy Regulatory Commission opened a Federal Power Act §206 show-cause proceeding in June 2026. CAISO filed a motion to hold it in abeyance through November 16 while tariff options are developed. | Open proceeding, not a final tariff-reform order. |
| California Public Utilities Commission (CPUC) Rule 30, A.24-11-007 | Interim framework for defined 50–230 kV retail customers. Customers initially fund facilities; refund and cost-allocation questions remain open. | Relevant to large-load interconnection, but not final. |
| CPUC R.26-04-009 | Open rate-design proceeding whose scope includes data centers and other large loads. | The proceeding asks whether new tariffs are needed. |
| SB 57 | Enacted in 2025. CPUC may assess data-center cost shifts; if completed, the assessment is due January 1, 2027. | Does not clearly require completion of a study. |
| SB 886 | Assembly Appropriations suspense. Would create separate tariffs by July 1, 2027, using a threshold no greater than 25 MW and a ten-year prefunded procurement commitment. Publicly owned facilities are excluded. | Pending bill, not a current CCSF requirement. |
| AB 1577 | Senate Appropriations suspense. Current text applies at 10 MW or more of installed IT-equipment electrical capacity and covers energy, power usage effectiveness, load, waste heat, onsite fuel, and demand flexibility. | Current text contains no water or WUE reporting and excludes publicly owned facilities. |
| AB 2619 | Senate Appropriations suspense as of August 10. Would require projected water information before and with an initial city or county business-license, equivalent-instrument, or permit application, and direct annual water reporting at renewal. | Pending bill. |

Sources: [FERC EL26-71](https://www.ferc.gov/media/e-10-el26-71-000), [CAISO July report and August motion](https://www.caiso.com/documents/aug-3-2026-caiso-s-motion-for-abeyance-regarding-lard-loads-el26-71.pdf), [CPUC Rule 30 interim decision](https://docs.cpuc.ca.gov/PublishedDocs/Published/G000/M574/K875/574875643.PDF), [CPUC R.26-04-009](https://docs.cpuc.ca.gov/PublishedDocs/Published/G000/M601/K776/601776967.PDF), [SB 57](https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=202520260SB57), [SB 886](https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=202520260SB886), [AB 1577](https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=202520260AB1577), [AB 2619](https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=202520260AB2619).

Across the reviewed proceedings and bills, the recurring policy questions are who funds attributable grid upgrades, what operating characteristics must be disclosed, and how to limit cost shifting to other customers. For CCSF, ownership and public-facility exclusions must be checked before assuming a large-load rule applies.

The European Union provides a useful enacted comparison. Delegated Regulation (EU) 2024/1364 requires annual reporting from data centers with at least **500 kW of installed IT demand**, including total and potable water input, water-use efficiency, waste heat reused, and energy-reuse performance. The Energy Efficiency Directive separately requires member states to ensure that data centers above **1 MW of total rated energy input** use waste heat or another recovery application unless a technical and economic assessment finds it infeasible. A further label-based rating regulation remained a draft at the cutoff. The European Commission published it for feedback on March 26, 2026, with adoption planned for the third quarter; the October 2025 study was preparatory, not law. [Delegated Regulation 2024/1364](https://eur-lex.europa.eu/eli/reg_del/2024/1364/oj?locale=eng), [Directive 2023/1791](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32023L1791), [draft rating regulation](https://eur-lex.europa.eu/legal-content/EN/PIN/?uri=PI_COM%3AAres%282026%293247482), [European Commission status](https://energy.ec.europa.eu/topics/energy-efficiency/energy-efficiency-targets-directive-and-rules/energy-efficiency-directive/energy-performance-data-centres_en)

---

## 7. What the evidence means for CCSF

### 7.1 Replace the point estimate with scenarios

The corpus's **5,000-worker** population is a planning choice, not an observed deployment. Its other workload inputs are also assumptions: three to eight agentic tasks per worker-hour, 30,000–150,000 tokens per task, eight active hours per day, 250 workdays per year, a three-to-four-times peak factor, a 20–30× token multiplier, and a 70% interactive/30% shiftable split.

The inputs do not produce the published **500,000–600,000 tokens-per-second** peak:

| Arithmetic from the stated inputs | Result |
|---|---:|
| Agent tasks per worker-day | **24–64** |
| Total tokens per year | **0.9–12.0 trillion** |
| Mean rate during the 2,000 stated work hours | **125,000–1.67 million tokens/second** |
| Three-to-four-times peak | **375,000–6.67 million tokens/second** |

The published range therefore selects a near-low-end case without saying so. A simple midpoint of the task and token assumptions would produce a **2.06–2.75 million tokens-per-second** peak, not 500,000–600,000. This midpoint is arithmetic, not a recommended forecast. The 20–30× multiplier must not be applied again: the 30,000–150,000 token range already claims to include input, reasoning, tool calls, and output.

Current enterprise evidence is newer and more relevant than the material used to create the scenario, but it still does not supply a CCSF central estimate:

| Evidence | What it adds | Why it cannot set the CCSF load |
|---|---|---|
| New Zealand Public Service Commission, October–December 2025 | 19,224 Microsoft Copilot prompts from 209 engaged users; 92 prompts per engaged user over the quarter. | Early use at one small public agency; no tokens, agent calls, concurrency, or energy. |
| OpenAI enterprise telemetry, 2025 | Weekly enterprise messages grew about 8×; average worker messages grew 30%; 95th-percentile workers sent 6× the median. | Reports growth and relative distributions, not absolute messages or tokens per worker-day. |
| OECD enterprise-sizing scenarios, 2026 | Illustrative cases assign one H100 to 1 billion tokens/month, two to three H100s to 10 billion, and eight H100s to 50 billion. | A modeled cost comparison using about 80% assumed GPU token capacity, not observed enterprise use; model, latency, and optimization choices can change capacity substantially. |
| Bai et al., 2026 | Coding-agent trajectories can reach millions of raw tokens and vary sharply across models and runs. | Coding benchmark, not office work; tokens are dominated by repeated and cached input; no electricity measurement. |
| Hausfather, 2026 | One heavy user's 1,138 typed prompts triggered more than 14,000 calls and 3.2 billion tokens, 96% cache reads. | One unusually intensive coding/research user; electricity was modeled, not metered. |
| Microsoft Azure production trace, 2026 | Agentic requests are bursty and alternate between model inference and tool execution; tool time matched or exceeded inference time for more than 27% of requests. | A 24-hour infrastructure trace with no users, tokens per worker-day, or municipal task mix. |

Sources: [New Zealand Public Service Commission](https://www.publicservice.govt.nz/assets/DirectoryFile/OIA-2025-0205-Information-request-regarding-AI-systems.pdf), [OpenAI enterprise report](https://openai.com/business/guides-and-resources/the-state-of-enterprise-ai-2025-report/), [OECD, Table 3.1](https://www.oecd.org/content/dam/oecd/en/publications/reports/2026/05/benefits-of-ai-openness_40eaff39/746e8c9a-en.pdf), [Bai et al.](https://arxiv.org/abs/2604.22750), [Hausfather](https://www.theclimatebrink.com/p/the-real-energy-use-of-agentic-ai), [Microsoft Azure production study](https://arxiv.org/abs/2608.04458).

The OECD table provides one current public enterprise-scale hardware comparator, but it is still illustrative. The CCSF inputs imply **75 billion–1 trillion tokens per average calendar month**, or 1.5–20 times the OECD's “very large” 50-billion-token case. That comparison does not prove a particular GPU count because the CCSF corpus mixes models and hardware generations while the OECD table assumes H100 capacity. It does show that the CCSF workload, hardware, and power figures were never reconciled through one declared serving model.

The reviewed public enterprise and government datasets do not jointly report seats, active users, tasks per user-day, calls per task, input/output/cache tokens, time-resolved concurrency, retries, success, and measured facility energy. The public evidence also shows that use is highly uneven: OpenAI's 95th-percentile workers sent six times as many messages as its median workers. A single “typical worker” hides lower-use workers and a heavy-use tail; when applied to the full eligible workforce, it also erases workers who are not active on a typical day.

> **Decision-record conflict:** `claude_session_state.md` still records 20–30× as the load-bearing sizing assumption. This review does not find support for using it as a universal central multiplier and therefore supersedes it for this note's sizing method. The session-state file remains unchanged and conflicts with this treatment. The IEA's roughly 25× GPU-energy sensitivity is not evidence for the prior token multiplier.

The most defensible update is therefore:

1. **Retain 5,000 workers only as the eligible planning cohort.** Do not treat every eligible worker as a daily active user.
2. **Retire 500,000–600,000 tokens per second as the central result.** Preserve it only as a labeled legacy scenario.
3. **Retire 20–30× as a universal token multiplier.** If useful, define a separate moderate-energy scenario from the IEA: 7.6 Wh for a four-to-six-call agentic task, about 25× the figure's 0.31 Wh large-text case. This is not a matched-model comparison. Add the IEA's 50 Wh reasoning-agent case as a high sensitivity. Neither is enterprise telemetry.
4. **Model adoption and intensity separately.** Use daily-active share, delegated tasks per active user, and workload type as independent variables. The existing 24–64 tasks per worker-day should be a legacy stress range, not the default.
5. **Represent workers as cohorts, not one average user.** Report non-users or occasional users, regular users, and the heavy-use tail separately; do not apply the heavy-user rate to all 5,000 workers.
6. **Size hardware only after a pilot and model-specific benchmark.** Input prefill, cache reads, output decoding, tool compute, latency, concurrency, and key-value-cache occupancy are different resource demands and cannot be collapsed into one token rate.

The following adoption ranges are transparent planning sensitivities, not forecasts. “Daily active” means a worker who delegates at least one AI task on a typical workday.

| Adoption scenario | Daily-active share of 5,000 | Not active on a typical day | Tasks per active user-day | Total tasks per workday |
|---|---:|---:|---:|---:|
| **Low use** | 20%–40% | 60%–80% | 1–2 | 1,000–4,000 |
| **Mixed use** | 40%–70% | 30%–60% | 3–5 | 6,000–17,500 |
| **High use** | 70%–100% | 0%–30% | 6–10 | 21,000–50,000 |
| **Legacy stress** | 100% | 0% | 24–64 | 120,000–320,000 |

Applying the IEA's GPU-only task values shows the additional uncertainty introduced by task type:

| Adoption scenario | Mean GPU load if every task is a moderate four-to-six-call agent, 7.6 Wh/task | Mean GPU load if every task is a reasoning agent, 50 Wh/task |
|---|---:|---:|
| **Low use** | 1.0–3.8 kW | 6.3–25 kW |
| **Mixed use** | 5.7–16.6 kW | 37.5–109 kW |
| **High use** | 20–47.5 kW | 131–313 kW |
| **Legacy stress** | 114–304 kW | 0.75–2.0 MW |

These are average GPU loads across an eight-hour workday, not facility estimates. They assume every task in a row has the same intensity and exclude or incompletely cover host processors, memory, storage, networking, tool execution, idle and reserved capacity, redundancy, cooling, and peaks. Actual use will be a mixture. The table shows why adoption, user distribution, task mix, and system boundary matter more than a single multiplier.

The corpus's **30–55 Blackwell-class GPU** count also conflicts with its equipment list. One GB200 NVL72 rack already contains 72 Blackwell GPUs, exceeding that count. Adding at least two of the listed 8-GPU H200 nodes brings the minimum physical total to 88 GPUs across two generations before the small-model tier. The count should be replaced by an actual bill of materials or expressed as a defined equivalent-capacity measure. [NVIDIA GB200 NVL72](https://www.nvidia.com/en-us/data-center/gb200-nvl72/)

The stated **400–600 kW of IT load** may remain as a reserved-capacity scenario, but it is not derived from the workload evidence. If treated as a continuous average load at PUE 1.2, the electricity arithmetic is correct:

> 0.4–0.6 MW × 8,760 hours × 1.2 = **4.2–6.3 GWh per year**.

### 7.2 Scale and water inconsistencies

The energy and water engineering narrative often uses a **5 MW facility** as “CCSF scale.” Five megawatts is **8.3–12.5 times** the 400–600 kW scenario and aligns more closely with the corpus's 50,000-worker case. A continuously operating 5 MW IT load would use **52.6 GWh per year of facility electricity at PUE 1.2**. The roughly 22 GWh annual case elsewhere in the deep dive is IT electricity at a 50% capacity factor. The two values use different duty cycles and electricity boundaries and are not directly comparable.

The cooling-water estimates also do not reconcile. For arithmetic only, treating the corpus's unsourced 0.5–1.8 L/kWh range as onsite water consumption per IT kWh, a continuous 5 MW IT load gives:

- 0.5 L/kWh gives about **17.8 acre-feet per year**.
- 1.0 L/kWh gives about **35.5 acre-feet per year**.
- 1.8 L/kWh gives about **63.9 acre-feet per year**.

PUE is not added to this calculation because the WUE denominator is already IT electricity. The corpus instead gives 60–105 acre-feet at 5 MW and 280–820 acre-feet at 40 MW. Those figures should be marked unresolved until they are recalculated using one declared electricity boundary, duty cycle, and WUE definition. The hybrid peak-day range also cannot be reconstructed from the stated inputs. Naively prorating full-load WUE over the stated 15–25 wet-trim days gives about **0.7–4.4 acre-feet per year**, but that is illustrative only and is not a valid design estimate without hourly wet-trim cooling load and wet-mode WUE.

### 7.3 No-regrets next step

A representative workload pilot is more valuable than another literature-derived multiplier. It should measure:

- Users and active hours by workload class.
- Model, input tokens, output tokens, cache reads and writes, tool calls, and retries.
- Latency and service-quality requirements.
- Average, peak, and coincident throughput.
- Accelerator and host energy, utilization, and batching.
- Facility PUE and direct water use under the intended cooling design.
- The portion of work that can move to midday clean-energy hours without delaying resident or staff services.

Until representative measurements are collected, the defensible conclusion is a range: CCSF may have a sub-megawatt inference requirement, but the current corpus does not support a decision-grade central estimate.

---

## Appendix A. How the project's top-level data and estimates changed

Status labels: **retained** means the definition and source remain suitable; **superseded** means a later source or finding replaces it; **retired** means the claim should not be reused; **unresolved** means the evidence, definition, or arithmetic is insufficient.

| Topic | Existing corpus | Current treatment | Status |
|---|---|---|---|
| U.S. data-center electricity | 176 TWh/4.4% in 2023; 325–580 TWh/6.7%–12% in 2028. An earlier 9.5%–15.3% by 2030 figure was retired as unsourced. ([benchmark §§2, 5](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md); [scratchpad “LBNL” entry](./CCSF_compute_research_scratchpad.md)) | Retain the historical values. Use LBNL's 192 TWh/4.7% estimate for 2024 and 521–843 TWh/9.5%–15.3% for 2030. The matching 2030 range comes from a new source and does not validate the earlier unsourced claim. | **Superseded** |
| Scope of national totals | National data-center totals were used as context for AI growth. ([benchmark §2](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md); [scratchpad “LBNL” entry](./CCSF_compute_research_scratchpad.md)) | State explicitly that LBNL and IEA totals cover all data centers, not AI alone. | **Retained limitation** |
| California data-center demand | The prior draft used 4,280 MW mid and 6,510 MW high for 2040 from January planning slides. ([CEC slides, pp. 7–8](https://www.energy.ca.gov/sites/default/files/2026-01/2026-01-05_DAWG_Mtg_Slides-Combined_ada.pdf)) | Use the adopted forecast: about 5,800 MW mid/planning and 8,400 MW high/local reliability within the CAISO balancing area, including existing load. | **Superseded** |
| Misidentified 4.5 GW figure | The benchmark called 4.5 GW a data-center-demand figure. ([benchmark §2](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md)) | Retire it. The cited 4.5 GW referred to planned offshore wind, not data-center demand. | **Retired** |
| 67% utilization factor | The prior draft called this PG&E's analysis. | Attribute it to a CEC assumption derived from Silicon Valley Power operating data. PG&E criticized it as high-end and potentially unrepresentative. ([CEC methodology memo, pp. 7, 11, 15](https://www.energy.ca.gov/sites/default/files/2026-04/Data_Center_Methodology_Memo_ada.pdf); [PG&E comments, pp. 4–5](https://efiling.energy.ca.gov/GetDocument.aspx?DocumentContentId=104787&tn=267761)) | **Corrected attribution** |
| California curtailment | 3.4 million MWh in 2024. The prior draft added a more precise April 2026 claim that did not survive verification. ([benchmark §2](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md)) | Retain the primary-supported 2024 value. Curtailment is not firm energy available to CCSF. | **Retained / narrowed** |
| CCSF planning population | 5,000 knowledge workers using agentic systems. ([strategic brief §3.4](./CCSF_public_compute_strategic_brief.md); [initial brainstorm “Workload assumptions”](./CCSF_compute_initial_brainstorm.md)) | Keep only as the project's selected planning population, not an observed deployment. | **Retained context** |
| Worker adoption and use distribution | All 5,000 workers implicitly receive the same 24–64 agent-tasks/day rate. ([strategic brief §§2.1, 3.4](./CCSF_public_compute_strategic_brief.md); [initial brainstorm “Workload assumptions”](./CCSF_compute_initial_brainstorm.md)) | Separate eligible headcount from daily-active share and from light, regular, and heavy-use cohorts. Add low, mixed, high, and legacy-stress sensitivities. | **Superseded method** |
| Agentic multiplier and throughput | 20–30× tokens; 500,000–600,000 tokens/second peak. ([initial brainstorm “Agentic token multiplier”](./CCSF_compute_initial_brainstorm.md); [pilot design “Why this is the keystone” and “How to read the result”](./CCSF_workload_pilot_design_2026-06-27.md)) | Retire as a central estimate. Full arithmetic gives 375,000–6.67 million tokens/second; the IEA's roughly 25× moderate-agent *energy* scenario is not a validation of the token multiplier. | **Retired central estimate** |
| CCSF equipment and electricity | 30–55 GPUs; four to six racks; 400–600 kW IT; 4.2–6.3 GWh/year. ([strategic brief §§3.4–3.6](./CCSF_public_compute_strategic_brief.md); [initial brainstorm “Cluster Architecture” and “Energy Usage”](./CCSF_compute_initial_brainstorm.md)) | The GPU count conflicts with the listed one-to-two 72-GPU NVL72 racks plus H200 nodes. The power figure is not derived from the workload or bill of materials. The annual-energy arithmetic is correct only if 400–600 kW is continuous average IT load at PUE 1.2. | **Unresolved scenario** |
| Enterprise-scale comparator | The reviewed corpus did not include a transparent external comparator. | OECD's illustrative table maps 1, 10, and 50 billion tokens/month to one, two-to-three, and eight H100s. CCSF's assumptions imply 75 billion–1 trillion tokens/month, but differing model, hardware, and latency assumptions prevent a direct conversion. | **New, illustrative only** |
| Facility scale | The 0.4–0.6 MW worker model and a 4–40 MW engineering envelope are both described as CCSF scale. ([strategic brief §3.6](./CCSF_public_compute_strategic_brief.md); [SFPUC deep dive §§7.3, 9.3](./CCSF_SFPUC_power_water_deep_dive.md)) | Separate them. A 5 MW facility is 8.3–12.5× the 5,000-worker estimate and resembles the 50,000-worker case. | **Unresolved mismatch** |
| Workload scheduling | 70% interactive/30% batch; shift batch “overnight.” ([strategic brief §3.5](./CCSF_public_compute_strategic_brief.md); [SFPUC deep dive §8.3](./CCSF_SFPUC_power_water_deep_dive.md)) | Split remains unmeasured. In California, shiftable work should target low-carbon, solar-rich midday hours rather than assume overnight is cleaner. | **Partly superseded** |
| Sensitive-workload share | 40%–60% of work described inconsistently as eligible and ineligible. ([initial brainstorm “Organizational Context” and “Four Strategic Models”](./CCSF_compute_initial_brainstorm.md)) | The reviewed corpus did not identify supporting evidence; do not reuse. | **Retired** |
| San Francisco free cooling | About 95% of annual hours. ([benchmark §1](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md)) | Retain only as a modeled inference under ASHRAE allowable conditions, not an operating measurement. | **Retained with qualification** |
| Water-use efficiency | LBNL national values, evaporative-system values, and operator portfolio figures presented together. ([scratchpad “WUE benchmarks”](./CCSF_compute_research_scratchpad.md); [benchmark §1](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md)) | Keep definitions and boundaries in the same cells. Do not rank withdrawal and consumption figures or use fleet values as a CCSF design target. | **Unresolved comparison** |
| CCSF cooling water | 7–20 acre-feet/year hybrid and 60–105 at 5 MW; 280–820 at 40 MW. ([SFPUC deep dive §§7.3, 9.3](./CCSF_SFPUC_power_water_deep_dive.md)) | The annual, peak-day, and scaling arithmetic does not reconcile. Recalculate from one duty cycle, electricity boundary, and WUE definition. | **Unresolved** |
| Southeast Plant recycled water | Earlier text implied near-term or permit-ready integration. ([strategic brief §4](./CCSF_public_compute_strategic_brief.md); [SFPUC deep dive §2.7](./CCSF_SFPUC_power_water_deep_dive.md); [benchmark §6](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md)) | The plant does not provide an eastside tertiary supply or distribution main. Treat the concept as long-horizon only. | **Superseded** |
| California bills | June snapshots described SB 886, AB 1577, and AB 2619 provisions and status. ([scratchpad “California regulatory landscape” and “legislative pipeline”](./CCSF_compute_research_scratchpad.md)) | Replace with operative text and status through August 11, 2026. AB 1577 no longer includes water and excludes public facilities; SB 886 uses ten years and excludes public facilities; AB 2619 was on Senate Appropriations suspense as of August 10. | **Superseded** |

Principal local sources: [strategic brief](./CCSF_public_compute_strategic_brief.md), [SFPUC deep dive](./CCSF_SFPUC_power_water_deep_dive.md), [regenerative-data-center benchmark](./CCSF_regenerative_datacenter_benchmark_2026-06-24.md), [initial brainstorm](./CCSF_compute_initial_brainstorm.md), [workload pilot design](./CCSF_workload_pilot_design_2026-06-27.md), and [research scratchpad](./CCSF_compute_research_scratchpad.md).

---

## Appendix B. Limits and omissions

This note does not estimate:

- Embodied energy, carbon, or water from manufacturing accelerators, servers, and buildings.
- A complete AI-only share of national or global data-center electricity.
- Hourly or locational California emissions and deliverable curtailed energy.
- Hetch Hetchy-specific water consumption under a defined allocation method.
- Current water-use efficiency for Digital Realty's 200 Paul facility.
- CCSF resource-adequacy, interconnection, power-supply, construction, or operating costs.
- A decision-grade CCSF workload, because this review did not identify representative local measurements.

Closed-vendor production data remain sparse and use incompatible boundaries. Current California legislation may change after the August 11 cutoff. The CCSF compute concept remains informal and unchartered; nothing in this note constitutes project approval, assignment, scope, or resourcing.
<!-- END VERBATIM DOCUMENT -->
