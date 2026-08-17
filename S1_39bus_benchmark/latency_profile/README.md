# Supplementary Data: Latency Profiling

This folder provides the latency profiling records used to characterize the computational overhead of the LLM-enabled workflow.

## Scope

The profiling evaluates three backbone models under the same workflow setting:

1. Qwen2.5-32B-Instruct
2. Qwen2.5-7B-Instruct
3. Meta-Llama-3.1-8B-Instruct

The latency records are reported independently from the reliability benchmark results. They are intended to quantify the time contribution of LLM inference, deterministic workflow processing, solver execution, and state-verification related procedures.

## Files
- `../aggregated_results/timing_profile_summary.csv`: aggregated latency statistics for all evaluated backbones.

The metrics include:

- `llm_latency_s`: local vLLM API round-trip latency, including request and response overhead; it should not be interpreted as hardware-kernel-only inference time;
- `deterministic_planning_s`: deterministic workflow processing time;
- `execution_s`: simulation execution time;
- `cleanup_s`: workspace cleanup time;
- `result_ready_s`: total time until verified result availability;
- `workflow_total_s`: complete workflow time.

The reported values are summarized using sample count, median, quartiles, mean, standard deviation, percentile, minimum, and maximum values.

## Notes

Raw execution logs and local environment information are not included. The provided aggregated statistics correspond to the latency analysis reported in the manuscript.
