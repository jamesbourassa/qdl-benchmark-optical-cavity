[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jamesbourassa/qdl-benchmark-optical-cavity/blob/main/notebook.ipynb)

# qdl-benchmark-optical-cavity

Minimal reproducible demonstration of residual-first model comparison using optical cavity resonance scaling.

## Status

This repository is a **methodological demo benchmark**.  
It illustrates the residual-first comparison workflow on a simple cavity-mode dataset.

This is not yet an executed public-data benchmark.

---

## Model

Optical cavity resonance frequencies:

Baseline model:
f = m c / (2L)

Reduced model:
f = m c / (2L0)

where:

- m = mode index
- c = speed of light
- L = fitted cavity length
- L0 = fixed reference length

---

## Method

1. Fit baseline model (estimate L)
2. Compute predicted frequencies
3. Compare residuals:
   - RMSE
   - Durbin–Watson statistic

The goal is to evaluate **residual structure**, not just fit quality.

---

## Files

- `notebook.ipynb` — reproducible benchmark
- `data.csv` — cavity mode dataset

---

## Run

Open `notebook.ipynb` and run all cells.

Compatible with:
- Google Colab
- Jupyter Notebook

---

## Program context

Part of the QDL Physics Institute benchmarking program:

https://qdlphysics.org

---

## Notes

This demo benchmark will be extended to a public-data experimental benchmark in a future version.
