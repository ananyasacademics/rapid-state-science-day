# RAPID Experimental Methodology

## Objective

The objective of RAPID is to evaluate the effectiveness of rule-based privacy anomaly detection using synthetic hospital access logs.

---

# Experiment Configuration

## Dataset Size
- Total synthetic events: 10,000

## Injected Anomalies
- Total injected anomalies: 500

## Random Seed
- Fixed random seed: 42

---

# Detection Rules

## R1 — Excessive Access Frequency
Detects unusually high access volume within short time intervals.

## R2 — After-Hours Activity
Detects suspicious activity outside expected operating hours.

## R3 — Cross-Department Access
Detects department-inconsistent access patterns.

## R4 — Role-Action Mismatch
Detects actions inconsistent with expected role permissions.

---

# Evaluation Metrics

The experiment calculates:
- precision,
- recall,
- F1 score,
- false positive rate,
- and confusion matrix statistics.

---

# Locked State Results

| Metric | Value |
|---|---|
| Recall | 92.0% |
| Precision | 59.7% |
| F1 Score | 72.4% |
| False Positive Rate | 3.26% |

---

# Sensitivity Analysis

## 5% Anomaly Prevalence
- Injected anomalies: 500
- Detected anomalies: 460
- Detection rate: 92.0%

## 2% Anomaly Prevalence
- Injected anomalies: 200
- Detected anomalies: 176
- Detection rate: 88.0%

---

# Reproducibility Controls

The experiment uses:
- fixed random seed configuration,
- deterministic synthetic generation,
- structured outputs,
- and reproducible execution artifacts.

---

# Ethical Constraints

This project uses synthetic data only.

No:
- real hospital records,
- patient data,
- or protected health information (PHI)
were used.