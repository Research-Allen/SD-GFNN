# Reproducibility Statement

This repository provides all artifacts required to reproduce the experimental results reported in the manuscript.

## Hardware

Experiments were conducted using:

- Python 3.11
- PyTorch 2.x
- NumPy
- Scikit-learn

GPU acceleration is optional.

## Datasets

Datasets used:

1. Breast Cancer Wisconsin
2. Iris
3. Wine
4. Digits

All datasets are available through Scikit-learn.

## Experimental Protocol

For each dataset:

- 30 independent runs
- Unique random seed per run
- Identical train/test split procedure
- Same stopping criteria across methods

Metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC (binary datasets)
- Training time
- Final hidden-neuron count

## Included Artifacts

### Raw Results

results/*_runs.csv

### Summary Statistics

results/summary_statistics.csv

### Ablation Study

results/ablation_results.csv

### Seeds

seeds/random_seeds.txt

### Configurations

configs/*.yaml

These materials enable full reproduction of Tables and Figures reported in the manuscript.
