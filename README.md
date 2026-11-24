# SD-GFNN: Synaptic Divergence Growing Feedforward Neural Network

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Official implementation and reproducibility package for:

**SD-GFNN: A Synaptic Divergence-Based Growing Feedforward Neural Network for Adaptive Network Expansion**

Author:
Dias Nurmagambetov
Prairie View A&M University, Texas, USA

---

## Overview

SD-GFNN (Synaptic Divergence Growing Feedforward Neural Network) is a dynamically expandable neural network that automatically increases its hidden-layer capacity during training.

Unlike conventional fixed-width multilayer perceptrons (MLPs), SD-GFNN introduces a **Synaptic Divergence (SD)** criterion that monitors neuron activity and determines when additional representational capacity is required.

The proposed framework:

- Starts from a compact architecture
- Monitors synaptic divergence values
- Triggers adaptive network growth
- Preserves previously learned knowledge
- Reduces unnecessary neuron expansion
- Improves parameter efficiency

---

## Repository Structure

```
SD-GFNN/
│
├── Experiments/
│   ├── source_code/
│   ├── ablation_study/
│   └── baseline_models/
│
├── Results/
│   ├── raw_csv/
│   ├── summary_tables/
│   ├── statistical_tests/
│   └── figures/
│
├── Seeds/
│   └── random_seeds.csv
│
├── Docs/
│   ├── configs/
│   ├── CITATION.bib
│   └── CITATION.cff
│
├── Manuscript/
│   └── submission_version.pdf
│
├── README.md
├── REPRODUCIBILITY.md
├── requirements.txt
└── LICENSE
```

---

## Included Reproducibility Materials

This repository contains all materials required to reproduce the experiments reported in the manuscript.

### Experimental Assets

✅ Source code

✅ Configuration files

✅ Random seeds

✅ Raw experimental outputs

✅ Statistical analysis

✅ Ablation study results

✅ Summary tables

✅ Figures used in the manuscript

---

## Datasets

Experiments were conducted using several benchmark datasets:

| Dataset | Task |
|----------|----------|
| Iris | Classification |
| Wine | Classification |
| Breast Cancer Wisconsin | Classification |
| Digits | Handwritten Digit Recognition |
| Fashion-MNIST | Image Classification |

Datasets are obtained through:

- Scikit-Learn
- TensorFlow/Keras

and can be automatically downloaded by the provided scripts.

---

## Installation

Create a Python environment:

```bash
python -m venv sd_gfnn_env
```

Activate:

Windows

```bash
sd_gfnn_env\Scripts\activate
```

Linux/Mac

```bash
source sd_gfnn_env/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running Experiments

Example:

```bash
python Experiments/source_code/digits_experiment.py
```

or

```bash
python Experiments/source_code/fashion_mnist_experiment.py
```

Results will automatically be stored in:

```text
Results/raw_csv/
```

---

## Reproducing Published Results

The exact random seeds used in the publication are provided in:

```text
Seeds/random_seeds.csv
```

To reproduce reported averages:

1. Load the provided seed list
2. Run all experiments
3. Aggregate results
4. Compare generated summary tables with:

```text
Results/summary_tables/
```

---

## Statistical Evaluation

The repository includes scripts and outputs for:

- Mean Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- 95% Confidence Intervals
- Paired t-tests
- Wilcoxon Signed-Rank Tests
- Cohen's d Effect Sizes

---

## Ablation Study

The ablation analysis evaluates various growth strategies:

- Single-node growth
- Linear growth
- Fibonacci growth (proposed)
- Exponential growth

Results are available in:

```text
Experiments/ablation_study/
Results/statistical_tests/
```

---

## Reproducibility Statement

All reported results can be reproduced using:

- Source code included in this repository
- Published configuration files
- Fixed random seeds
- Open benchmark datasets

No proprietary software, private datasets, or inaccessible resources are required.

Additional details are provided in:

```text
REPRODUCIBILITY.md
```

---

## Citation

If you use this work, please cite:

```bibtex
@article{Nurmagambetov2026SDGFNN,
  author = {Nurmagambetov, Dias},
  title = {SD-GFNN: A Synaptic Divergence-Based Growing Feedforward Neural Network for Adaptive Network Expansion},
  journal = {Neural Processing Letters},
  year = {2026}
}
```

---

## License

This project is released under the MIT License.

See:

```text
LICENSE
```

for details.
