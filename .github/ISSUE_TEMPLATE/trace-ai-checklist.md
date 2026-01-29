name: TRACE-AI Checklist Submission
about: Attach a filled checklist and artifacts for a manuscript or dataset
title: "[TRACE-AI] <project/manuscript title>"
labels: [checklist]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for aligning with TRACE-AI. Please link immutable artifacts (commit hashes, DOIs).
  - type: input
    id: contact
    attributes:
      label: Corresponding author / contact
      placeholder: name, email
    validations:
      required: true
  - type: textarea
    id: summary
    attributes:
      label: Scope
      description: Briefly state the system, data, and autonomy level.
    validations:
      required: true
  - type: textarea
    id: filled_checklist
    attributes:
      label: Checklist
      description: Paste the filled markdown table or link to the file (commit hash/DOI).
    validations:
      required: true
  - type: textarea
    id: artifacts
    attributes:
      label: Key artifacts
      description: Links to data, models, agent cards, notebooks, environment specs.
    validations:
      required: true
  - type: textarea
    id: deviations
    attributes:
      label: Deviations / limitations
      description: Note any N/A or unmet items and rationale.
