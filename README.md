# MEF-Net
Open-Set Domain Generalization Classification of Hyperspectral Images Based on Evidence Fusion
## Overview

we propose MEF‑Net (Multi‑Evidence Fusion Network), which combines evidential deep learning, energy‑based modeling, and Dirichlet entropy to achieve both high accuracy on known classes and robust identification of unknown classes.

## Main Contributions

### 1. Multi‑Evidence Generator

- Global branch: captures macroscopic spectral profiles and spatial context
- Local branch: divides the spectrum into overlapping band groups to focus on local discriminative features
- Both branches output Dirichlet distribution parameters with explicit epistemic uncertainty

### 2. Uncertainty‑Aware Evidence Fusion Module

- Models evidence conflict as attention similarity
- Uses the epistemic uncertainty of each evidence source as a modulating factor (bias and weight) to enhance robust fusion

### 3. Energy–Dirichlet Entropy Joint Decision Mechanism

- Energy score measures how well a sample matches the known classes
- Dirichlet entropy quantifies the flatness of the predictive distribution
- The two complementary signals significantly improve known vs. unknown separation

## Datasets

- Pavia University → Pavia Center
- Houston 2013 → Houston 2018
- ZY‑1 02D → GF‑5
