# TRACE-AI Publication Checklist

Table 1. TRACE-AI publication checklist for Transparent Reporting for Agentic Catalysis Enabled by Artificial Intelligence. This is a living, versioned community standard maintained at https://github.com/trace-ai-community/trace-ai-checklist.

Version: 0.1.1  
Date: 2026-02-07  
Status values: `Y` = yes / satisfied, `N` = no / missing, `N-A` = not applicable (explain why).

Fill this table for every manuscript or dataset that claims TRACE-AI alignment. Link each item to the exact evidence (manuscript section, figure, SI file, repo path, or DOI).

| ID | Item (what must be findable/verifiable) | Status (Y/N/N-A) | Evidence (section/link) | Notes |
| --- | --- | --- | --- | --- |
| A1 | Describe semantic and numerical harmonization steps and unresolved issues, if using multi-source data and data types (e.g., raw data files, spreadsheets, published literature). |  |  |  |
| A2 | Provide processing code that regenerates the ML-ready dataset from source data, and clearly state how dataset equivalence is checked (record counts/IDs, etc). |  |  |  |
| A3 | Define all input features/descriptors and their generation pipeline. |  |  |  |
| A4 | Provide dataset identifiers, access details, and core metadata sufficient for reuse. |  |  |  |
| A5 | State policy on negative/failed/suboptimal experiments and include if informative. |  |  |  |
| B1 | Document full model specification (architecture, hyperparameters, objective, versions). |  |  |  |
| B2 | Describe data-split strategies implemented to prevent information leakage. |  |  |  |
| B3 | Clearly state metrics applied to assess model performance with confidence intervals to avoid best-only reporting. |  |  |  |
| B4 | Justify the choice of metrics and examine trade-offs explicitly for multi-objective tasks. |  |  |  |
| B5 | Describe the uncertainty quantification method, its calibration and utilization. |  |  |  |
| C1 | Specify the agent policy and objectives, constraints, acquisition or reward functions, and provide configuration details or pseudocode with versioning including sources of stochasticity and which parameters are fixed across runs. |  |  |  |
| C2 | Declare the level of autonomy and human oversight, and document any interventions or overrides during the campaign, including their frequency, rationale, and impact on subsequent agent behavior. |  |  |  |
| C3 | Define stopping criteria and anomaly or failure handling procedures, and report any aborted runs, exclusions, or post hoc corrections. |  |  |  |
| C4 | Describe safety bounds, interlocks, and shutdown mechanisms, and explain how the agent is prevented from executing unsafe experiments. |  |  |  |
| C5 | Maintain a traceable record of the campaign trajectory, with summaries or representative segments when full iteration-level detail is impractical, sufficient to support the statistical reproducibility of agent behavior. |  |  |  |
| D1 | Provide executable tutorials or notebooks illustrating key elements of data management, model development, and workflow integration. |  |  |  |
| D2 | Link each tutorial or notebook to the relevant manuscript sections and checklist items, and include versioning information where feasible. |  |  |  |
| D3 | Document the execution environment required to run the tutorials (e.g., container images, lockfiles, or environment specifications) to mitigate dependency and API drift. |  |  |  |

## How to use
1) Clone this repo; copy this file into your project or supplement.  
2) Fill the table; keep links stable (DOIs, commit hashes, archival buckets).  
3) Export to PDF for submission if needed (`pandoc checklist/trace-ai-checklist.md -o checklist.pdf`).  
4) Keep the filled checklist under version control alongside data, models, and agent configs.

## Minimum evidence expectations
- Evidence should resolve to a specific, open artifact (section number, SI page, notebook path, log file, or DOI).  
- For `N-A`, state the domain reason (e.g., “no physical experiments performed”).  
- For multi-lab or distributed autonomy (A5), include cross-site data exchange and governance details in C1–C5 notes.
