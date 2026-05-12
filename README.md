# RAPID: Rule-Based Access Pattern Intrusion Detector

## Overview

RAPID is a reproducible synthetic cybersecurity framework designed to evaluate rule-based hospital privacy anomaly detection using simulated electronic health record (EHR) access logs.

This repository represents the official State Science Day version of the project and aligns with the final State:
- poster,
- engineering report,
- slide deck,
- and reproducibility artifacts.

The project uses synthetic hospital access events to simulate potential privacy violations and evaluate how effectively rule-based monitoring can detect suspicious access patterns.

---

# Project Goals

The goals of RAPID are to:

- simulate hospital access log environments,
- inject controlled privacy anomalies,
- evaluate rule-based detection performance,
- measure cybersecurity detection metrics,
- demonstrate reproducible experimentation,
- and support transparent healthcare cybersecurity research.

---

# System Architecture

RAPID contains the following core modules:

## 1. Synthetic Log Generator
Generates simulated hospital access events including:
- user roles,
- departments,
- timestamps,
- patient identifiers,
- and access actions.

## 2. Validation Layer
Validates generated datasets for:
- schema integrity,
- field consistency,
- formatting correctness,
- and experiment reproducibility.

## 3. Anomaly Injection Engine
Injects controlled synthetic anomalies into the dataset.

## 4. Rule-Based Detection Engine
Applies rule-based privacy detection logic.

### Detection Rules
- R1: Excessive Access Frequency
- R2: After-Hours Activity
- R3: Cross-Department Access
- R4: Role-Action Mismatch

## 5. Risk Scoring Layer
Assigns risk prioritization scores to flagged events.

## 6. Evaluation Metrics Module
Calculates:
- precision,
- recall,
- F1 score,
- false positive rate,
- and confusion matrix statistics.

---

# Final Locked State Results

## Dataset Configuration

- Total synthetic events: 10,000
- Injected anomalies: 500
- Random seed: 42

## Detection Performance

| Metric | Value |
|---|---|
| True Positives | 460 |
| False Negatives | 40 |
| False Positives | 310 |
| True Negatives | 9,190 |
| Recall / Detection Rate | 92.0% |
| Precision | 59.7% |
| F1 Score | 72.4% |
| False Positive Rate | 3.26% |

---

# Sensitivity Analysis

## 5% Anomaly Prevalence
- Injected anomalies: 500
- Detected anomalies: 460
- Detection Rate: 92.0%

## 2% Anomaly Prevalence
- Injected anomalies: 200
- Detected anomalies: 176
- Detection Rate: 88.0%

---

# Repository Structure

```text
configs/
data/
docs/
logs/
notebooks/
outputs/
reproducibility/
science_day_artifacts/
src/
state_artifacts/
tests/
```

---

# Reproducibility

RAPID was designed to support reproducible cybersecurity experimentation.

## Reproducibility Features
- fixed random seed,
- deterministic anomaly injection,
- reproducible metrics generation,
- run manifests,
- environment tracking,
- and structured experiment outputs.

---

# Synthetic Data Notice

This project uses synthetic data only.

No:
- real hospital data,
- patient information,
- protected health information (PHI),
- or real electronic health records
were used in this project.

---

# Educational Purpose

This project was developed for educational cybersecurity research and Science Day evaluation purposes.

---

# Alignment Notice

The repository is synchronized with the official:
- State poster,
- State report,
- and State presentation deck.

All future repository modifications must preserve alignment with those submitted artifacts.