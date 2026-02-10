# Conformal Prediction-Based Multi-Sensor Classification

This repository contains the code for the paper:

**Conformal Prediction-Based Multi-Sensor Classification**  
Farbod Siahkali, Vijay Gupta (Purdue University)

---

## Abstract

We consider the problem of multi-view classification using multiple sensors. Many traditional Bayesian approaches as well as modern learning models for classification provide point predictions. For safety-critical applications, it may be desirable to have a set of potential predictions such that there is a high enough probability of one element of the set being the correct prediction. Conformal prediction offers a model-agnostic framework for such a prediction with associated uncertainty quantification. However, most current sensor fusion methods for conformal prediction-based estimates require the associated $p$-values of the predictions from each sensor to be independent. Due to shared noise or other environmental correlations, this assumption may not be valid. We propose and analyze a strategy for fusing the outputs of multiple sensors that learns to account for dependencies among conformal $p$-values without assuming independence. Numerical experiments on one synthetic and three real-world datasets demonstrate that our conformal late fusion (CLF) approach outperforms conventional methods across all four datasets, often offering tighter and more efficient conformal sets at the desired coverage level.

---

## Repository Structure

- `Synthetic Data Experiments/` – synthetic multi-view experiments with controllable cross-view correlation  
- `CIFAR-10 Experiments/` – CIFAR-10 patch-based multi-view experiments  
- `CIFAR-100 Experiments/` – CIFAR-100 patch-based multi-view experiments  
- `MELD Experiments/` – multimodal emotion recognition experiments (text/audio/visual)  

---

## Requirements

Experiments were run in Python (PyTorch). You will typically need:

- Python 3.9+
- numpy, scipy, pandas
- pytorch
- scikit-learn
- matplotlib

---

## Usage

Each experiment folder is self-contained and includes scripts or notebooks for running the corresponding experiments. Please refer to the individual directories for details.

---

## Citation

If you use this code in your research, please cite the following paper:

```bibtex
@unpublished{siahkali2026conformal,
  title   = {Conformal Prediction-Based Multi-Sensor Classification},
  author  = {Siahkali, Farbod and Gupta, Vijay},
  note    = {Under review at Neurocomputing},
  year    = {2026}
}
