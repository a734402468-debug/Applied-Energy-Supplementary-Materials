# Applied-Energy-Supplementary-Materials
# Supplementary Materials

This repository provides supplementary materials for the manuscript:

**A Trustworthy LLM-Enabled Workflow for Power-System Modeling and Security Assessment**

The materials support the controlled benchmark and practical scalability assessment reported in the manuscript. They are organized into four folders.

## Repository structure

```text
.
├── README.md
├── S1_39bus_benchmark/
├── S2_KLM_time_estimation/
├── S3_modeling_workflow/
└── S4_N1_security_assessment/
```

## Folder descriptions

### S1_39bus_benchmark

This folder supports Section V of the manuscript. It contains the supplementary PDF and aggregated benchmark data for the controlled New England 39-bus evaluation.

The materials include the benchmark prompt suite, workflow-planning prompt, experimental configurations, aggregated reliability statistics, ablation and model-sensitivity results, plotting inputs, and failure-summary statistics.

### S2_KLM_time_estimation

This folder supports the manual-workload estimation used in Section VI. It provides the calculation materials for the Keystroke-Level Model (KLM)-based time estimate used to construct the conservative manual baseline.

### S3_modeling_workflow

This folder supports the model-preparation case study in Section VI. It contains the desensitized modeling prompt and the corresponding generated workflow plan used for the 201-bus practical case.

### S4_N1_security_assessment

This folder supports the representative N-1 security-assessment case study in Section VI. It contains the desensitized N-1 assessment prompt and the corresponding generated workflow plan.

## Notes

The supplementary materials are provided to document the benchmark settings, aggregated results, timing-estimation procedure, and representative workflow records used in the manuscript. Sensitive local paths, internal service addresses, and project-specific identifiers have been removed or replaced with generic descriptions where necessary.

The numerical results reported in the manuscript should be interpreted together with the corresponding tables and records in these supplementary folders.
