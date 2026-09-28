---
title: "Crown–Root Transition Morphometrics — Exploratory Prototype"
excerpt: "Two-case CT prototype using outer-shell intensity profiles to derive an exploratory crown–root transition proxy."
collection: portfolio
lang: en
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
---

**Project Repository (GitHub):** [Crown-Root-Transition-Morphometrics](https://github.com/trungnb/Crown-Root-Transition-Morphometrics)  
**Tech Stack:** Python, NiBabel, NumPy, SciPy, scikit-learn (PCA), Pandas  

### Overview
Two-case CT prototype exploring whether outer-shell tooth intensity profiles can identify an intensity-derived crown–root transition proxy. It does not establish anatomical CEJ localisation or validated crown–root morphometry.

### Approach
* Aligned tooth masks by principal axes, sampled a three-voxel outer shell, summarised slice-wise intensity profiles, and used a heuristic transition search to derive an exploratory (crown + transition)/root-extent ratio.
* Historical PCA used voxel-index coordinates; there is no anatomical CEJ reference, inter-rater assessment, external validation, or population-level performance estimate.
