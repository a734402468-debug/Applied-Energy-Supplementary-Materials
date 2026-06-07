# Supplementary Data S2: Conservative manual-interaction baseline

This supplementary file provides the supporting calculation for the manual-workload baselines reported in Section VI.

The values are not controlled human-subject measurements. They are conservative lower-bound estimates used to make the efficiency comparison transparent. The estimates assume an experienced engineer, uninterrupted operation, no input errors, no rework, and no debugging iterations.

The calculation file `S2_baseline.csv` contains two workflow-level estimates:
1. the 201-bus model-preparation workflow, corresponding to the 15.7 h manual lower-bound estimate;
2. the representative N-1 security-assessment workflow, corresponding to the 182 s manual lower-bound estimate.

The unit_time_s column represents the grouped per-operation latency used in the simplified model; it aggregates physical interaction, context switching, and engineering verification components according to the operation category.
