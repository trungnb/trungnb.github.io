---
title: "Master's Thesis: Upper Airway Dimensions in OSA (R Analysis)"
excerpt: "Reproducible R workflow for non-parametric group comparisons and publication-ready visualization of CBCT airway dimensions in OSA.<br/><img src='https://img.shields.io/badge/Tech-R_%7C_ggplot2_%7C_dplyr-blue'>"
collection: portfolio
date: 2025-09-09
---

**Tech Stack:** R, RMarkdown, `dplyr`, `tidyr`, `ggplot2`, `ggpubr`, `effsize`  
**Related Publication:** *Upper Airway Dimensions on CBCT in Vietnamese Subjects with and without Obstructive Sleep Apnea: A Case Series* (Vietnam Medical Journal, 2025)

### Overview
This repository contains the reproducible data analysis scripts developed for my Master's thesis on Obstructive Sleep Apnea (OSA). Working with CBCT data, I wrote R scripts to clean, visualize, and perform statistical group comparisons of upper airway morphometrics, directly supporting a peer-reviewed publication in the Vietnam Medical Journal (2025).

### Motivation
For my Master's thesis, I needed to process and analyze volumetric and cross-sectional measurements of the upper airway. Instead of relying solely on point-and-click statistical software (SPSS), I chose to learn R to ensure reproducibility, programmatic data wrangling, and publication-standard visualization.

### Technical Approach
* Curated and preprocessed clinical and CBCT morphometric data from 11 subjects (Vietnamese case series with and without OSA).
* Assessed distributional assumptions using the Shapiro-Wilk test for normality and F-test for homogeneity of variance.
* Performed group comparisons using the Mann-Whitney U / Wilcoxon rank-sum test for airway parameters (MinCSA, Volume, MinAP, MinLR) and Fisher's exact test for categorical variables.
* Calculated non-parametric effect sizes using Cliff's delta (`effsize`).
* Generated publication-quality boxplots with jittered data points and automated p-value brackets using `ggplot2` and `ggpubr` (exported at 1200 DPI).

### Key Learnings & Future Work
Mastered programmatic data cleaning, non-parametric hypothesis testing, and high-resolution scientific visualization in R. **Future Work:** Successfully used this workflow to publish a paper; next steps involve using Python to automate the initial 3D data extraction phase.
