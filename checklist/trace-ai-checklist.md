# TRACE-AI Publication Checklist

Version: 0.1.0  
Date: 2026-01-29  
Status values: `Y` = yes / satisfied, `N` = no / missing, `N-A` = not applicable (explain why).

Fill this table for every manuscript or dataset that claims TRACE-AI alignment. Link each item to the exact evidence (manuscript section, figure, SI file, repo path, or DOI).

| ID | Item (what must be findable/verifiable) | Status (Y/N/N-A) | Evidence (section/link) | Notes |
| --- | --- | --- | --- | --- |
| A1 | Multi-source harmonization steps and remaining incompatibilities are described (semantic and numerical). |  |  |  |
| A2 | Processing code regenerates the modeling dataset from raw sources; dataset equivalence checks (counts/IDs) are stated. |  |  |  |
| A3 | All input features/descriptors are defined with their generation pipeline. |  |  |  |
| A4 | Dataset identifiers, access details, and core metadata for reuse are provided. |  |  |  |
| A5 | Policy on negative/failed/suboptimal experiments is stated; informative negatives are included when possible. |  |  |  |
| B1 | Full model specification (architecture, hyperparameters, objectives, versions/checkpoints) is documented. |  |  |  |
| B2 | Data-split strategy prevents information leakage; split rules + seeds are reported. |  |  |  |
| B3 | Performance metrics with confidence intervals are reported to avoid best-only results. |  |  |  |
| B4 | Metric choice and multi-objective trade-offs are justified (e.g., Pareto fronts or weighting). |  |  |  |
| B5 | Uncertainty quantification method, calibration, and how UQ is used in decisions are described. |  |  |  |
| C1 | Agent policy is specified (objectives, constraints, acquisition/reward functions, stochastic sources, fixed params) with config or pseudocode. |  |  |  |
| C2 | Level of autonomy and human oversight are declared; interventions/overrides logged with frequency and impact. |  |  |  |
| C3 | Stopping criteria plus anomaly/failure handling are defined; aborted runs/exclusions/post hoc corrections are reported. |  |  |  |
| C4 | Safety bounds, interlocks, shutdown mechanisms, and guardrails preventing unsafe experiments are described. |  |  |  |
| C5 | Traceable record of campaign trajectory is maintained (full log or representative segments supporting statistical reproducibility). |  |  |  |
| D1 | Executable tutorials/notebooks cover data management, model development, and workflow integration. |  |  |  |
| D2 | Tutorials/notebooks are linked to relevant manuscript sections and checklist items with version info. |  |  |  |
| D3 | Execution environment is documented (container image, lockfile, or environment spec) to mitigate dependency/API drift. |  |  |  |

## How to use
1) Clone this repo; copy this file into your project or supplement.  
2) Fill the table; keep links stable (DOIs, commit hashes, archival buckets).  
3) Export to PDF for submission if needed (`pandoc checklist/trace-ai-checklist.md -o checklist.pdf`).  
4) Keep the filled checklist under version control alongside data, models, and agent configs.

## Minimum evidence expectations
- Evidence should resolve to a specific, open artifact (section number, SI page, notebook path, log file, or DOI).  
- For `N-A`, state the domain reason (e.g., “no physical experiments performed”).  
- For multi-lab or distributed autonomy (A5), include cross-site data exchange and governance details in C1–C5 notes.

