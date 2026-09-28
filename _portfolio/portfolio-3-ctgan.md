---
title: "Tabular Synthetic Data with CTGAN & ctdGAN"
excerpt: "Two-stage ANSUR II benchmark: original fidelity-plus-utility experiments followed by an AI-assisted methodological redesign."
collection: portfolio
lang: en
translation_key: portfolio-3-ctgan
date: 2026-06-15
---

**Project Repository (GitHub):** [Medical-CTGAN-Synthesis](https://github.com/trungnb/Medical-CTGAN-Synthesis)  
**Tech Stack:** Python, CTGAN, ctdGAN, SDMetrics, Scikit-Learn, XGBoost, GitHub Actions  

### Overview
Two-stage project using the ANSUR II anthropometric dataset (n=6,068). V1 contains my original experiments combining statistical fidelity with downstream predictive utility; V2 is an AI-assisted redesign focused on fairer comparison, reproducibility, and multi-seed benchmarking.

### Approach
* Evaluated CTGAN and ctdGAN with distributional quality metrics and TRTR/TSTR utility across multiple downstream classifiers and targets.
* Reworked the benchmark with a fixed real-data split, train-only feature selection, matched generator settings, five seeds, confidence intervals, baselines, and automated GitHub Actions; this is an anthropometric benchmark, not a clinical or privacy-validation study.
