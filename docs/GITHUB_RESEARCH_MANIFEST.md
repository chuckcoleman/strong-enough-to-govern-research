# GitHub Research Storage Plan

**Date:** 2026-10-01

## 1. Standalone public/reproducible repository: `stv-ranking-cap-analysis`

This should remain separate from the book repository because it asks an independently reusable empirical/engineering question.

Store:
- `README.md`
- `LICENSE`
- `CITATION.cff`
- `requirements.txt`
- `stv_wigm.py`
- `scotland_stv_rank_cap_analysis.py`
- `portland_stv_rank_cap_analysis.py`
- `run_stv_rank_cap_analysis.py`
- `docs/methodology.md`
- `data/README.md`
- `data/source_manifest.csv`
- machine-generated CSV outputs
- tests for the WIGM implementation
- a pinned commit/hash for the Scottish source data
- Portland CVR acquisition instructions and checksum

Do not silently treat Portland ranks 7–8 as observed: Portland 2024 ballots are censored by the six-ranking limit.

Prefer retrieval scripts or source manifests over redistributing third-party raw files unless redistribution rights are clear.

## 2. General research/reproducibility repository: `strong-enough-to-govern-research`

Keep private during proposal development if desired; publication status can be decided later.

Recommended structure:

```text
strong-enough-to-govern-research/
├── README.md
├── LICENSE
├── CITATION.cff
├── schemas/
│   ├── canonical_options.csv
│   ├── accountability_functions.csv
│   ├── comparative_case_schema.md
│   └── durability_dependency_schema.md
├── data/
│   ├── comparative_case_coding.csv
│   ├── timing_episode_seed.csv
│   ├── canonical_option_dependency_crosswalk.csv
│   ├── structural_case_coding.csv
│   └── source_manifest.csv
├── docs/
│   ├── methodology.md
│   ├── coding_protocol.md
│   ├── provenance.md
│   └── research_decisions.md
└── scripts/
    └── (only when a table/figure is actually generated computationally)
```

### Why these belong on GitHub

Store material when at least one is true:
- it is machine-readable data used in a claim;
- it is a coding schema that constrains case selection or classification;
- it is code that generates a table, figure, or result;
- it records source provenance or version pinning needed to reproduce the result;
- it documents a methodological decision that otherwise could drift across revisions.

The following files prepared in this research pass belong there:
- `comparative_case_coding.csv`
- `timing_episode_seed.csv`
- `canonical_option_dependency_crosswalk.csv`
- `structural_case_coding.csv`
- `PREPROPOSAL_RESEARCH_COMPLETION.md` (or a shortened `docs/research_decisions.md`)
- this manifest

## 3. Do not put these in a public reproducibility repository by default

- copyrighted books/articles/PDFs;
- publisher proposal drafts or manuscript chapters unless publication is intentional;
- private correspondence, peer-review material, or acquisition-editor communications;
- raw third-party datasets whose licenses do not permit redistribution;
- notes containing unverified allegations about identifiable people;
- duplicated web/PDF sources when a URL, DOI, archival identifier, and checksum will reproduce provenance;
- transient scratch files.

## 4. Source-version control

The exact canonical OPT definitions retrieved during this pass are in `preventing_dictatorship_v0.94.tex`, while the current dossier names v0.95 as its research baseline. The research repository should therefore contain a `provenance.md` stating the exact source file/hash used for `schemas/canonical_options.csv`.

If v0.95 is recovered later:
1. compare its nine option definitions with v0.94;
2. update `canonical_options.csv` only if definitions differ;
3. record the change in `research_decisions.md`;
4. never overwrite provenance silently.

## 5. When a separate timing repository becomes worthwhile

Do **not** create one yet. Keep the timing data in the general research repository until it becomes an independently reusable dataset (for example, a systematically coded multi-episode dataset across administrations and oversight mechanisms). At that point it can be split without changing the book's source-of-truth schema.

## 6. Reproducibility convention

For each derived result, record:
- source URL / DOI / archival identifier;
- retrieval date;
- source version/date;
- transformation script;
- output filename;
- any manual coding decision;
- whether the source can legally be redistributed;
- checksum for downloaded public data when practical.

This is more important than storing every source file itself.