# Supplementary Data for the Controlled 39-Bus Benchmark

The materials are intended to document the benchmark prompt suite, experimental configurations, aggregated results, plotting inputs, and failure-summary statistics used in the controlled New England 39-bus benchmark.

## Repository contents

```text
.
├── README.md
├── Supplementary_Material.pdf
└── aggregated_results/
    ├── table2.csv
    ├── table3.csv
    ├── fig4.csv
    ├── fig5.csv
    ├── fig6.csv
    └── failure_reason_summary.csv
```

## Supplementary material

`Supplementary_Material.pdf` contains:

* the 45 benchmark prompts used in the controlled 39-bus evaluation;
* the workflow-planning system prompt used in the full-workflow configuration;
* the evaluated experimental configurations;
* aggregated reliability, ablation, model-sensitivity, and failure-summary results;
* a representative boundary case illustrating the plan-to-execution gap.

## Aggregated results

The folder `aggregated_results/` contains the CSV files used to support the tables and figures reported in Section V of the manuscript.

| File                                    | Description                                                                                                 |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `table2.csv`  | Aggregated planning validity, task-correct execution rate, and plan-to-execution gap for the full workflow. |
| `table3.csv` | Aggregated ablation and model-sensitivity results.                                                          |
| `fig4.csv`         | Input matrix for the full-workflow heatmap across task complexity levels and instruction variants.          |
| `fig5.csv`        | Input matrix for the ablation and model-sensitivity comparison figure.                                      |
| `fig6.csv`        | Input matrix for the composite-task instruction-variant trend figure.                                       |
| `failure_reason_summary.csv`            | Aggregated failure-summary statistics used for the failure analysis.                                        |

## Benchmark scale

The controlled benchmark contains 45 prompts. Each prompt is repeated 30 times under each evaluated configuration, resulting in 1350 runs per configuration. Five configurations are evaluated:

1. Full workflow with Qwen2.5-32B-Instruct.
2. Schema guidance removed.
3. Control layer removed.
4. Qwen2.5-7B-Instruct.
5. Meta-Llama-3.1-8B-Instruct.

The full benchmark therefore contains 6750 evaluated runs in total.

## Notes

The repository provides the supplementary PDF and the aggregated CSV files used to support the reported tables and figures. Local machine paths, internal service addresses, and environment-specific identifiers are not included.
