# Mapping TRACE-AI Checklist to Manuscript Sections

Use this as a guide when citing evidence in the checklist. Adjust section numbers to your draft.

| Checklist ID | Likely manuscript location | Notes |
| --- | --- | --- |
| A1–A5 | Data Management section (§1.1–1.4); figures or SI showing harmonization, preprocessing, negative data policy. | Include processing scripts and manifest links. |
| B1–B5 | Model Development section (§2.1–2.4); tables of hyperparameters, split strategy, metrics with CIs, UQ calibration plots. | For domain-shift cases, cite validation against experimental benchmarks. |
| C1–C5 | Workflow Integration section (§3.1–3.5); describe autonomy level, agent policy, safety bounds, stopping rules, and trajectory logging. | Include agent card(s) and run logs. |
| D1–D3 | Executable artifacts section or SI; notebook/tutorial references and environment specs. | Provide container tag or lockfile. |

If your manuscript reorders content, mirror the checklist IDs in section headers or footnotes for easy verification.
