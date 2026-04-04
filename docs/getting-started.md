# Getting Started with TRACE-AI Checklist

Audience: authors, reviewers, and editors working with the TRACE-AI publication checklist.

## Quick workflow (authors)
1. Copy `checklist/trace-ai-checklist.md` into your project repository or SI.  
2. Fill columns `Status`, `Evidence`, and `Notes` after each major milestone (data curation, model freeze, campaign completion).  
3. Complete supporting templates as applicable:
   - `templates/agent-card-template.md` for every agent/policy used.
   - `templates/data-manifest-template.yaml` for each dataset snapshot.
   - `templates/autonomy-run-log-template.md` per closed-loop run or batch.
4. Archive immutable artifacts (data/model tarballs, notebooks, logs) with DOIs or commit hashes; cite them in the Evidence column.  
5. Export a PDF for submission if needed (`pandoc` example: `pandoc checklist/trace-ai-checklist.md -o trace-ai-checklist.pdf`).  

## Quick workflow (reviewers/editors)
- Confirm every `Y` links to auditable evidence (section number, SI page, repo path, or DOI).  
- Spot-check leakage controls (B2), autonomy claims (C2), and safety guardrails (C4) against logs/configs.  
- If items are `N` or `N-A`, check that rationale is documented and scientifically acceptable.  

## Evidence guidance by section
- **Data (A1–A5)**: include harmonization notes, processing scripts, manifests, and policy for negative/failed data.  
- **Model (B1–B5)**: cite model cards, split scripts/seeds, metrics with CIs, Pareto analyses, UQ calibration plots.  
- **Workflow (C1–C5)**: link agent cards, autonomy logs, safety bounds, stopping rules, and trajectory logs.  
- **Executables (D1–D3)**: provide runnable notebooks/tutorials plus env specs or container tags; pin commit hashes.  

## Suggested repo layout (one possible pattern)
```
project/
  data/              # raw + processed (with checksums)
  models/            # checkpoints with metadata
  agents/            # configs, prompts, policies
  notebooks/         # executable artifacts
  logs/              # autonomy run logs, safety events
  docs/trace-ai/     # filled checklist + manifests
```

## Common pitfalls to avoid
- Reporting only best runs without seeds or split rules (violates B2/B3).  
- Missing safety bounds for autonomous execution (violates C4).  
- Sharing notebooks without environment pins (violates D3).  
- Dropping anomalies without logging rationale (violates A1/A5/C3).  

## Versioning
- Current checklist version: **2.1.0 (2026-04-04)**.  
- Track changes in `CHANGELOG.md`; cite the version you used in manuscripts.  

## License and reuse
- Checklist text and templates: CC-BY-4.0 (see `LICENSE`).  
- Contributions are welcome via issues or pull requests; use the issue template in `.github/ISSUE_TEMPLATE/trace-ai-checklist.md`.  
