---
title: "Medical Tabular Data Synthesis (CTGAN & ctdGAN)"
excerpt: "Exploratory CTGAN and ctdGAN notebooks using mock demographic data.<br/><img src='https://img.shields.io/badge/Tech-CTGAN_%7C_ctdGAN_%7C_Python-green'>"
collection: portfolio
lang: en
translation_key: portfolio-3-ctgan
date: 2026-06-15
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1qInNhtiGobzpOIexIhhCxGZT5zZTeWID?usp=sharing)  
**Tech Stack:** Python, CTGAN, ctdGAN, SDMetrics, Pandas, NumPy, Scikit-Learn  

### Overview
This project contains small exploratory notebooks for learning how CTGAN and ctdGAN can model tabular data. I used mock demographic variables such as age, race, and sex, then compared generated outputs with the input distributions. The experiments are educational and do not establish anonymization or a privacy guarantee for clinical data.

### Motivation
I became interested in synthetic data because clinical datasets require careful governance and are not always openly shareable. The goal here was to understand the basic workflow and its limitations, not to claim that synthetic data automatically solves privacy risks.

### Technical Approach
* Used CTGAN and ctdGAN implementations to generate samples from small mock demographic datasets.
* Compared selected distributions and summary statistics between input and generated data.
* Used SDMetrics and simple downstream-model checks to explore fidelity and utility; these checks are not a formal privacy audit.

### Key Learnings & Future Work
Learned the basic concepts of tabular generative models, distributional evaluation, and the difference between synthetic data and proven privacy protection. **Future Work:** Study privacy risk assessment and governance before experimenting with more complex clinical variables.
