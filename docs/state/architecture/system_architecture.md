# RAPID System Architecture

## Overview

RAPID (Rule-Based Access Pattern Intrusion Detector) is a modular synthetic cybersecurity experimentation framework designed to evaluate rule-based hospital privacy anomaly detection.

The system processes synthetic hospital access logs through multiple reproducible pipeline stages.

---

# High-Level Pipeline

Synthetic Log Generation
→ Validation Layer
→ Anomaly Injection
→ Rule-Based Detection
→ Risk Scoring
→ Evaluation Metrics
→ Experiment Outputs

---

# Core Components

## 1. Synthetic Log Generator

The synthetic log generator creates simulated hospital access events.

### Generated Fields
- user identifiers,
- departments,
- staff roles,
- patient identifiers,
- timestamps,
- and access actions.

### Purpose
The generator creates reproducible synthetic datasets without using real hospital records.

---

## 2. Validation Layer

The validation layer verifies:
- schema integrity,
- required fields,
- timestamp consistency,
- and formatting correctness.

### Purpose
This stage ensures experiment reliability and reproducibility.

---

## 3. Anomaly Injection Engine

The anomaly injection engine inserts controlled synthetic privacy anomalies into the dataset.

### Injected Behaviors
- excessive record access,
- after-hours access,
- cross-department access,
- and role-action mismatches.

### Purpose
This stage creates labeled ground-truth anomalies for evaluation.

---

## 4. Rule-Based Detection Engine

The detection engine evaluates events using deterministic cybersecurity rules.

## Detection Rules

### R1 — Excessive Access Frequency
Flags users accessing unusually high numbers of records within short time intervals.

### R2 — After-Hours Activity
Flags suspicious access occurring outside expected operational hours.

### R3 — Cross-Department Access
Flags access patterns inconsistent with department assignments.

### R4 — Role-Action Mismatch
Flags actions inconsistent with expected permissions for staff roles.

---

## 5. Risk Scoring Layer

Flagged events receive risk prioritization scores.

### Purpose
Risk scoring helps prioritize suspicious events for review.

---

## 6. Evaluation Metrics Module

The metrics module calculates:
- true positives,
- false positives,
- true negatives,
- false negatives,
- precision,
- recall,
- F1 score,
- and false positive rate.

### Purpose
This stage measures rule-based detection effectiveness.

---

# Reproducibility Design

RAPID was designed for reproducible experimentation.

## Reproducibility Features
- fixed random seed,
- deterministic anomaly injection,
- structured output artifacts,
- run manifests,
- and reproducible metrics generation.

---

# Data Safety

RAPID uses synthetic data only.

No:
- real patient records,
- protected health information (PHI),
- or real hospital logs
are included in this repository.