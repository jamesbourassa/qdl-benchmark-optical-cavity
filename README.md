
# Optical Cavity Residual-First Benchmark

Minimal reproducible benchmark demonstrating **residual-first model comparison** using optical cavity resonance data.

This repository accompanies the Quantized Dimensional Ledger (QDL) benchmarking program.

---

## Benchmark idea

Two model families are compared.

### Baseline model

f = m c / (2L)

where

- f = resonance frequency
- m = mode index
- c = speed of light
- L = cavity length (fitted)

### Reduced model

f = m c / (2L0)

where L0 is fixed.

---

## Residual-first interpretation

Evaluation proceeds in the following order:

1. Fit both model families
2. Inspect residual structure
3. Compare RMSE / AIC / BIC afterward

The goal is to detect structured residual trends rather than simply minimize error magnitude.

---

## Repository structure

qdl-benchmark-optical-cavity
│
├── notebook.ipynb
├── data/data.csv
└── outputs/

---

## Running the benchmark

Open **notebook.ipynb** and run all cells.

The notebook will:

- load the dataset
- fit the baseline model
- compute the reduced model
- generate residual statistics

---

## Program context

This repository is part of the **QDL Physics Institute experimental benchmarking program**.

https://qdlphysics.org
