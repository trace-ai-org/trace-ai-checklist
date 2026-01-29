# TRACE-AI Agent Card (template)

Fill one card per agentic system used in the study. Keep it versioned with code and data.

- **Agent name / ID**:  
- **Version / commit / container tag**:  
- **Point of contact**:  
- **Objective(s)**: optimization targets or hypotheses.  
- **Level of autonomy (A0–A5)**:  
- **Observation space**: sensors, features, retrieved context, uncertainty, history length, normalization.  
- **Action space**: controllable variables (bounds/units), discrete choices, replicate/check actions, calibration steps.  
- **Constraints & forbidden regions**: safety, operational, resource, or ethical; enforcement mechanism.  
- **Policy/decision core**: algorithm (BO/RL/heuristic), surrogate/model type, acquisition/reward function, optimizer, batch size.  
- **Stochasticity controls**: random seeds, exploration schedule (e.g., ε-greedy, temperature), noise injection.  
- **Update rules**: when/how models are retrained; warm-start sources; cold-start strategy.  
- **Tool access**: databases, retrievers, code execution, instruments/robots; guardrails and fail-safe behavior.  
- **Human oversight**: approval points, escalation triggers, override protocol.  
- **Safety interlocks**: hardware/software limits, shutdown paths, watchdogs.  
- **Logging**: what is logged, format, retention, and log-location/URI; run IDs.  
- **Domain of applicability**: where predictions/actions are valid; known gaps or OOD indicators.  
- **Known failure modes & mitigations**: include detection signals.  
- **Evaluation & validation**: offline metrics, prospective tests, reference catalysts/benchmarks.  
- **Dependencies**: container image, env file, hardware (GPUs, instruments).  
- **Change history**: summarize material changes since the last version.
