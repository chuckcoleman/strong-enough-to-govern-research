# Strong Enough to Govern — Pre-Proposal Research Completion Memo

**Date:** 2026-10-01  
**Scope:** Research needed to stabilize the book proposal architecture, not the complete manuscript research program.

## Bottom line

The pre-proposal research program is sufficiently complete to begin proposal preparation. The remaining work is primarily manuscript-scale evidence building, legal updating, and implementation detail rather than a missing foundation for the proposal.

Four findings materially affect the proposal architecture:

1. **Domestic coercive/military authority is an independent red-line candidate.** It is legally distinct from National Emergencies Act continuation and plausibly satisfies the book's four inclusion tests: accountability consequence, concentrated chokepoint, time-sensitive reversibility, and availability of capacity-compatible safeguards. This does not require the proposal to declare a final sixth red line; it does require the proposal to show the category explicitly rather than assume it is contained in the emergency-power chapter.
2. **The comparative chapter can use a predeclared case-selection rule.** The primary universe can be V-Dem's 2026 set of ongoing U-turn democratizers (data through 2025), selecting cases for outcome variation rather than narrative convenience. Brazil, Botswana, Poland, and Zambia provide a compact primary set; Hungary is useful as a supplemental 2026 restoration case outside the V-Dem 2025-data universe.
3. **The timing thesis has a concrete empirical core.** Watergate/Nixon, McGahn, and Fast and Furious show substantial variation in the interval between compulsory process and useful compliance. The unit of analysis should be the accountability episode, with the practical deadline recorded separately from the legal disposition.
4. **Chapters 10–12 should not be treated symmetrically.** Senate procedure has a defensible but relatively narrow connection through appointments, confirmations, renewal, and oversight capacity. Redistricting reform has direct causal evidence that institutional design can constrain partisan map-drawing discretion. The stronger claim that RCV/STV/Condorcet/proportional electoral rules themselves reduce democratic backsliding or executive capture remains unestablished; Chapter 12 should distinguish demonstrated mechanical/administrative effects from structural hypotheses.

## 1. Red-line stress test

### Domestic coercive/military authority

Current law separates domestic military law-enforcement authority from ordinary emergency declarations. The Posse Comitatus Act generally prohibits use of covered armed forces to execute domestic law absent constitutional or statutory authorization. The Insurrection Act supplies a distinct statutory authorization framework in 10 U.S.C. §§251–255.

The category passes the book's inclusion screen as a serious candidate:

- **Accountability consequence:** control over coercive implementation can affect implementation/compliance and replacement/restoration, and can interact with election administration and public-order functions.
- **Chokepoint quality:** presidential invocation and command create concentrated decision points.
- **Time-sensitive reversibility:** deployment can alter physical conditions before judicial or legislative correction becomes effective.
- **Capacity-compatible safeguard possibility:** a bipartisan group convened by the American Law Institute proposed clearer triggers, gubernatorial consultation, a report to Congress within 24 hours, and a 30-day limit absent renewed congressional authorization while preserving immediate availability of forces in extraordinary circumstances.

The main unresolved question is not causal relevance but **boundary placement**. The proposal should distinguish:
- election-period coercive interference (overlap with OPT-E2),
- emergency continuation/default rules (OPT-M1),
- prosecution and other executive coercive functions (OPT-A3), and
- domestic military deployment authority.

Do not assign a new stable OPT identifier until the architecture is formally revised.

Sources:
- 18 U.S.C. §1385: https://uscode.house.gov/view.xhtml?edition=prelim&f=treesort&jumpTo=true&num=0&req=%28title%3A18+section%3A1385+edition%3Aprelim%29+OR+%28granuleid%3AUSC-prelim-title18-section1385%29
- 10 U.S.C. ch. 13: https://uscode.house.gov/view.xhtml?edition=2023&req=granuleid%3AUSC-2023-title10-chapter13
- ALI-convened Principles: https://www.ali.org/news/articles/guidance-insurrection-act-reform-issued-bipartisan-group

## 2. Comparative case design

### Eligible universe

Use V-Dem's Democracy Report 2026 U-turn-democratizer classification (data through 2025) as the primary sampling frame. V-Dem identifies Brazil, Botswana, Guatemala, Lesotho, and Poland as cases in which autocratization was reversed before democratic breakdown, and Bolivia, Mauritius, and Zambia as cases in which democratic breakdown was followed by a bounce-back. Zambia is explicitly described as a fragile reversal with renewed deterioration.

### Proposal-scale core cases

- **Brazil:** resistance/reversal case; useful for institutional response and reversal.
- **Botswana:** turnover/limiting case; useful because prolonged dominant-party rule nevertheless ended in peaceful electoral transfer.
- **Poland:** restoration-after-turnover case; useful for the reversibility problem and the legal/quick/effective restoration trilemma.
- **Zambia:** fragile reversal/negative-deviant case; useful because turnover did not guarantee durable restoration.
- **Hungary (supplemental):** a 2026 restoration case occurring after the V-Dem report's 2025 data cutoff. Keep it analytically separate from the predeclared primary sampling frame.

Use the same coding fields for each case:
`attempted_control -> chokepoint -> accountability_function -> response -> immediate_outcome -> reversibility -> durability -> shared_dependencies -> evidence_against_mechanism`.

Sources:
- V-Dem Democracy Report 2026: https://www.v-dem.net/documents/75/V-Dem_Institute_Democracy_Report_2026_lowres.pdf
- Poland: https://www.journalofdemocracy.org/articles/democracy-after-illiberalism-a-warning-from-poland/
- Hungary: https://www.journalofdemocracy.org/articles/can-peter-magyar-restore-hungarys-democracy/
- Zambia 2026: https://freedomhouse.org/country/zambia/freedom-world/2026

## 3. Timing evidence

The proposal can state a testable timing proposition without claiming that every delay is obstruction:

> A legal remedy can be formally successful yet institutionally ineffective when information, compliance, or adjudication arrives after the accountability process can still use it.

Seed episodes:

- **Nixon/Watergate:** Special Prosecutor subpoena for 64 tapes on 1974-04-16; Supreme Court upheld subpoena on 1974-07-24; House Judiciary adopted impeachment articles 1974-07-27 through 1974-07-30; Nixon resigned 1974-08-09. This is a case in which adjudication and compliance occurred while the accountability process remained live.
- **McGahn:** House Judiciary subpoena issued 2019-04-22; testimony scheduled for 2019-05-21 did not occur; transcribed interview occurred 2021-06-04 after extended litigation/accommodation. This is a clean example of eventual compliance after the original political context had materially changed.
- **Fast and Furious:** a House committee subpoena was issued in 2011; a 2018 conditional settlement was described by DOJ as ending six years of litigation and requiring additional production. This illustrates very long oversight-enforcement latency, while also requiring care because accommodation and document production occurred during the dispute.

For the full book, code at least:
`request/subpoena date`, `return date`, `filing date`, `trial decision`, `appeal`, `compliance/accommodation`, `relevant political deadline`, `whether relief could still change the outcome`, and `legitimate-process explanation for delay`.

Sources:
- Watergate chronology: https://www.archives.gov/education/lessons/watergate-constitution/chronology.html
- McGahn transcript: https://democrats-judiciary.house.gov/sites/evo-subsites/democrats-judiciary.house.gov/files/migrated/UploadedFiles/McGahn_Interview_Transcript.pdf
- Fast and Furious settlement: https://www.justice.gov/archives/opa/pr/department-justice-enters-conditional-settlement-agreement-produce-fast-and-furious-documents

## 4. Structural chapters

### Chapter 10 — Senate

Retain the chapter as a conditional structural-reinforcement chapter, but keep the proposal claim narrow. The clearest mechanisms are:
- appointment and confirmation delay,
- staffing continuity,
- emergency renewal,
- oversight capacity,
- impeachment and legislation.

This evidence does not by itself establish that Senate malapportionment or supermajoritarian procedure generally causes executive entrenchment. Those broader propositions remain research questions.

### Chapter 11 — House, redistricting, and subnational entrenchment

The chapter has a stronger empirical bridge. A 2026 APSR study estimates that redistricting reforms reducing partisan actors' leeway reduce partisan bias and increase competition; it also finds that institutional details matter, with designs lacking later partisan veto points producing different effects from nominal commissions that retain them.

Three useful state dossiers:
- **North Carolina:** post-election restructuring of elections/ethics administration, followed by state constitutional litigation and statutory redesign.
- **Wisconsin:** 2018 lame-duck legislation restricting powers of incoming statewide officials, including litigation-intervention and settlement authority.
- **Michigan:** transfer of map-drawing authority from legislature to an independent citizens commission; useful both as reform evidence and as a caution because minority-representation and remedial-map controversies remained.

These cases should be used to trace mechanisms, not to equate representational unfairness with anti-entrenchment effects.

Sources:
- APSR redistricting study: https://www.cambridge.org/core/journals/american-political-science-review/article/redistricting-reforms-reduce-gerrymandering-by-constraining-partisan-actors/5D85E711B3C401F0D24A9B7BB8C50337
- North Carolina SL 2017-6: https://www.ncleg.gov/EnactedLegislation/SessionLaws/HTML/2017-2018/SL2017-6.html
- North Carolina Cooper v. Berger listing: https://www.nccourts.gov/documents/appellate-court-opinions
- Wisconsin summary: https://statedemocracy.law.wisc.edu/our-work/lame-duck-power-grabs-in-north-carolina-and-beyond
- Michigan mapping data: https://www.michigan.gov/micrc/mapping-process/mapping-data

### Chapter 12 — Electoral design

The empirical stopping rule is now clear. Separate three types of claims:

1. **Formal properties:** what a tabulation rule guarantees mathematically.
2. **Administrative/implementation properties:** ballot design, auditability, count reproducibility, voter use of rankings, district magnitude.
3. **Democratic-resilience/anti-capture effects:** downstream effects on party systems, coalition incentives, governing capacity, and control of accountability institutions.

Current evidence is sufficient for (1) and increasingly strong for (2), especially from Scotland and Portland. It is not sufficient to state (3) as an established effect.

Relevant causal evidence is limiting rather than confirmatory:
- A preregistered study of 273 U.S. cities finds RCV initially increases candidate entry, but the effect dissipates and is concentrated among low-support entrants; it detects no effect on female or nonwhite candidate shares.
- A cross-national identification study finds more party-system fragmentation increases government fractionalization but no average effect on 25 other democratic-quality outcomes, with possible moderation in very high-polarization contexts.

Sources:
- RCV candidate entry: https://onlinelibrary.wiley.com/doi/10.1111/ajps.12908
- Party fragmentation: https://www.cambridge.org/core/journals/british-journal-of-political-science/article/does-partysystem-fragmentation-affect-the-quality-of-democracy/202A72173869E4CAA583822FB6518672

## 5. Canonical-option durability crosswalk

The canonical inventory contains nine stable IDs: OPT-E1, OPT-E2, OPT-M1, OPT-A1, OPT-A2, OPT-A3, OPT-C1, OPT-P1, and OPT-S1. The accompanying CSV records dependencies and common-mode failure candidates without assigning a comparative score.

The principal cross-cutting finding is that nominally different safeguards often share:
- court timing/compliance,
- appropriations,
- executive-branch records and custodians,
- career personnel,
- confirmation/staffing,
- state cooperation,
- or the same coercive chain.

The proposal therefore has a defensible contribution in **dependency structure**, not merely in adding more safeguards.

## 6. Epilogue evidence

National service and civic-engagement material should remain separate from the institutional safeguard claims.

AmeriCorps' 2023 State of the Evidence report synthesized 116 agency-conducted or funded studies from 2017–2022. It reports a mixed participant evidence base and notes that only a subset of participant studies used quasi-experimental or randomized designs. Earlier systematic-review material likewise contains positive, null, and program-specific findings rather than a general result that service reliably creates democratic tolerance or resilience.

The proposal can therefore describe the Epilogue as a research-grounded exploration of civic reinforcement, but should not make national service carry the causal burden of the institutional argument.

Sources:
- AmeriCorps 2023 State of Evidence: https://www.americorps.gov/sites/default/files/document/2023%20SOE%20Report_090123_final_508_0.pdf
- National Service Systematic Review: https://www.americorps.gov/sites/default/files/document/2015_08_19_NationalServiceSynthesisFullReport_ORE.pdf

## 7. Market differentiation

Recent adjacent books show substantial overlap in topic but not in the project's full mechanism:

- Lessig & Seligman, *How to Steal a Presidential Election* (Yale, 2024): presidential election mechanisms.
- Rose-Ackerman, *Democracy and Executive Power* (Yale, 2021): executive policymaking and accountability.
- *Global Challenges to Democracy* (Cambridge, 2025): comparative backsliding and resilience.
- Gamboa, *Resisting Backsliding* (Cambridge, 2022): opposition strategies.

The proposal's descriptive point of differentiation is the combination of:
**lawful executive capacity + observable chokepoints + timing/reversibility + accountability functions + common-mode dependency + two-dimensional durability.**

Sources:
- https://yalebooks.yale.edu/book/9780300270792/how-to-steal-a-presidential-election/
- https://www.cambridge.org/core/books/global-challenges-to-democracy/C50D0AC769FF0AA2C62DA9337F2C03E6
- https://www.cambridge.org/core/books/resisting-backsliding/introduction/00E68D789282B2664970CE70A4B15594

## 8. Source-control issue to resolve before proposal circulation

The current dossiers describe `preventing_dictatorship_v0.95.tex` as the research baseline, but the retrievable file containing the exact canonical nine-option inventory is `preventing_dictatorship_v0.94.tex`. A search did not retrieve a separate v0.95 source file.

Before proposal circulation:
- recover and archive v0.95 if it exists, **or**
- change the provenance statement so the canonical option inventory is explicitly sourced to v0.94.

Do not allow the exact option definitions to depend on an unavailable version reference.

## 9. What can wait until after proposal preparation

These are still needed for the book but are not proposal blockers:

- exhaustive federal/state certification-law survey;
- complete emergency-declaration and renewal history;
- full episode dossiers for statistics, science, IGs, prosecution, clemency, and courts;
- complete timing dataset across all four Chapter 7 subfamilies;
- full option-by-option legal drafting and amendment text;
- complete national-service/civic-reinforcement literature review;
- repeated updating of current cases and doctrine immediately before manuscript use.

The proposal can now be prepared while these proceed.