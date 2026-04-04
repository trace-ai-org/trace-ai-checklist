# TRACE-AI Publication Checklist

Table 1. TRACE-AI publication checklist for Transparent Reporting for Agentic Catalysis Enabled by Artificial Intelligence. This is a living, versioned community standard maintained at https://github.com/trace-ai-community/trace-ai-checklist.

Version: 2.1.0
Date: 2026-04-04
Status values: `Y` = yes / satisfied, `N` = no / missing, `N-A` = not applicable (explain why).

Fill this table for every manuscript or dataset that claims TRACE-AI alignment. Link each item to the exact evidence (manuscript section, figure, SI file, repo path, or DOI) directly in the item cell and mark the status in the right column.

| Items to check (each should be verifiable in manuscript, SI, or linked artifacts) | Y/N/N-A |
| --- | --- |
| **A. Data Management** |  |
| A1. Describe semantic and numerical harmonization steps and any unresolved issues when using multi-source data and heterogeneous data types (e.g., raw files, spreadsheets, literature). |  |
| A2. Provide processing code that regenerates the ML-ready dataset from source data, and state how dataset equivalence is checked (e.g., record counts, IDs). |  |
| A3. Define all input features or descriptors and their generation pipeline. |  |
| A4. Provide dataset identifiers, access details, and core metadata sufficient for reuse. |  |
| A5. State the policy on negative, failed, or suboptimal experiments and include them when informative. |  |
| **B. Model Development** |  |
| B1. Document the full model specification (architecture, hyperparameters, objective, versions). |  |
| B2. Describe data-splitting strategies implemented to prevent information leakage. |  |
| B3. Report performance metrics with appropriate uncertainty (e.g., confidence intervals) to avoid best-only reporting. |  |
| B4. Justify the choice of metrics and explicitly examine trade-offs for multi-objective tasks. |  |
| B5. Describe the uncertainty quantification method, its calibration, and how it is used in analysis or decision-making. |  |
| **C. Workflow Integration** |  |
| C1. Specify the agent policy, constraints, and acquisition or reward functions, and provide configuration details or pseudocode with versioning, including sources of stochasticity and parameters fixed across runs. |  |
| C2. Declare the level of autonomy and human oversight, and document any interventions or overrides during the campaign, including their frequency, rationale, and impact. |  |
| C3. Define stopping criteria and anomaly or failure-handling procedures, and report any aborted runs, exclusions, or post hoc corrections. |  |
| C4. Describe safety bounds, interlocks, and shutdown mechanisms, and explain how unsafe actions are prevented. |  |
| C5. Maintain a traceable record of the campaign trajectory, with summaries or representative segments when full detail is impractical, sufficient to support statistical reproducibility of agent behavior. |  |
| **D. Tutorials, Notebooks, and Executable Artifacts** |  |
| D1. Provide executable tutorials or notebooks illustrating key elements of data management, model development, and workflow integration. |  |
| D2. Link each tutorial or notebook to the relevant manuscript sections and checklist items, including versioning information where feasible. |  |
| D3. Document the execution environment required to run the tutorials (e.g., container images, lockfiles, or environment specifications) to mitigate dependency and API drift. |  |

## How to use
1) Clone this repo; copy this file into your project or supplement.
2) Fill the table; keep links stable (DOIs, commit hashes, archival buckets).
3) Export to PDF for submission if needed (`pandoc checklist/trace-ai-checklist.md -o checklist.pdf`).
4) Keep the filled checklist under version control alongside data, models, and agent configs.

## Minimum evidence expectations
- Evidence should resolve to a specific, open artifact (section number, SI page, notebook path, log file, or DOI).
- For `N-A`, state the domain reason (e.g., "no physical experiments performed").
- For multi-lab or distributed autonomy (A5), include cross-site data exchange and governance details in C1–C5 notes.
