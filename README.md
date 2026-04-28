# MLOps Pipeline with Drift Detection & Auto-Retraining
![CI/CD](https://github.com/vhanumankumar/mlops-drift-detection/actions/workflows/ci_cd.yml/badge.svg)
> Automated model monitoring, drift detection, and retraining for production ML.


## Problem Statement
Production ML models degrade silently. This pipeline implements 
automated drift detection, performance monitoring, and retraining 
triggers — maintaining model reliability without manual intervention.

## Tech Stack
Python · MLflow · Evidently AI · Docker · GitHub Actions · Azure ML · Grafana

## Pipeline
1. Model trained + versioned with MLflow
2. Evidently monitors data/prediction drift daily
3. Drift threshold breach → auto retraining triggered
4. CI/CD via GitHub Actions deploys new model version

## Results
- Drift detected within 1 hour of distribution shift
- Model release cycle reduced by ~40%
- PSI-threshold automated retraining
- Full CI/CD via GitHub Actions

## How to Run
```bash
git clone https://github.com/vhanumankumar/mlops-drift-detection
pip install -r requirements.txt
python train.py
python monitor.py
```

## Status
Portfolio demo | MLOps best practices for UK enterprise AI
