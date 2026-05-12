# RAPID Official State Metrics

## Project
RAPID: Rule-Based Access Pattern Intrusion Detector

## Final Locked State Results

- Total synthetic events: 10,000
- Injected anomalies: 500
- Detected anomalies: 460

## Confusion Matrix

- True Positives (TP): 460
- False Negatives (FN): 40
- False Positives (FP): 310
- True Negatives (TN): 9,190

## Evaluation Metrics

- Recall / Detection Rate: 92.0%
- Precision: 59.7%
- F1 Score: 72.4%
- False Positive Rate: 3.26%

## Sensitivity Analysis

### 5% Anomaly Prevalence
- Injected anomalies: 500
- Detected anomalies: 460
- Detection Rate: 92.0%

### 2% Anomaly Prevalence
- Injected anomalies: 200
- Detected anomalies: 176
- Detection Rate: 88.0%

## Detection Rules

- R1: Excessive Access Frequency
- R2: After-Hours Activity
- R3: Cross-Department Access
- R4: Role-Action Mismatch

## Additional System Features

- Risk scoring enabled
- Random seed fixed to 42
- Synthetic data only
- No real hospital data used
- Reproducible experiment pipeline

## Alignment Requirement

This metrics file is the official source of truth for:
- State poster
- State report
- State slide deck
- GitHub repository documentation