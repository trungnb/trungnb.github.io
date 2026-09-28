---
title: "Crown–Root Transition Morphometrics — Exploratory Prototype"
excerpt: "Two-case CT prototype using outer-shell intensity profiles to derive an exploratory crown–root transition proxy.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
lang: en
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
---

**Project Repository (GitHub):** [Dental-CEJ-Morphometrics](https://github.com/trungnb/Dental-CEJ-Morphometrics)  
**Tech Stack:** Python, NiBabel, NumPy, SciPy, scikit-learn (PCA), Pandas  

### Overview
Two-case CT prototype exploring whether outer-shell tooth intensity profiles can identify an intensity-derived crown–root transition proxy. It does not establish anatomical CEJ localisation or validated crown–root morphometry.

### Approach
* Aligned tooth masks by principal axes, sampled an outer shell, summarised slice-wise intensity profiles, and applied a heuristic transition search to generate exploratory crown–root ratios.
* Preserved failure cases rather than filtering them; the method has no manual CEJ reference, inter-rater assessment, external validation, or population-level performance estimate.
