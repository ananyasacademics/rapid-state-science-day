# RAPID Run Manifest Documentation

## Purpose

Run manifests provide reproducibility tracking for RAPID experiment executions.

Each manifest records:
- run configuration,
- experiment parameters,
- random seed settings,
- dataset generation details,
- and output references.

---

# Locked State Configuration

| Parameter | Value |
|---|---|
| Random Seed | 42 |
| Total Events | 10,000 |
| Injected Anomalies | 500 |

---

# Manifest Goals

The manifest system supports:
- reproducibility,
- experiment traceability,
- output verification,
- and deterministic reruns.

---

# Stored Information

Run manifests may contain:
- execution timestamps,
- configuration references,
- generated output filenames,
- dataset metadata,
- and metric summaries.

---

# State Alignment Notice

The State Science Day repository uses locked experiment configurations aligned with the submitted:
- State report,
- State poster,
- and State presentation deck.