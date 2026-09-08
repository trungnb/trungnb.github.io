---
title: "Dental Morphometrics: CEJ & Crown-Root Ratio"
excerpt: "Quantitative Python analysis workflow for calculating Crown-Root ratios and identifying the Cementoenamel Junction (CEJ) from 3D dental models.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
date: 2026-07-28
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Tech Stack:** Python, Jupyter, NiBabel, NumPy, SciPy (`ndimage`), Pandas, Matplotlib  

### Overview
Manual 3D measurements in dentistry are highly tedious. Driven by a desire to explore computational dental anatomy, I wrote proof-of-concept Python scripts in Jupyter to automate anatomical alignment, CEJ detection, and crown-root ratio calculations from NIfTI segmentations. This hands-on project provided practical experience in 3D voxel manipulation and coordinate transformations.

### Motivation
Manually clicking through 3D dental models to find landmarks like the Cementoenamel Junction (CEJ) is time-consuming and subjective. I explored whether programmatic coordinate alignment and voxel density profiling could assist in standardizing dental morphometric extraction.

### Technical Approach
* Loaded and manipulated 3D volumetric images (NIfTI format) using NiBabel and NumPy.
* Applied 3D binary erosion on segmented tooth masks to isolate the outer shell voxel layer.
* Performed Principal Component Analysis (PCA) on 3D tooth coordinates to calculate the principal anatomical axis and rotate it to the Z-axis using affine transforms.
* Profiled cross-sectional Hounsfield Unit (HU) statistics (mean, min, max, std) along the Z-axis to detect density transitions at the CEJ boundary.
* Scripted functions to compute anatomical ratios (Crown-to-Root) and pulp chamber volume.

### Key Learnings & Future Work
Gained a foundational understanding of manipulating 3D arrays and voxel data in Python. **Future Work:** Aim to integrate these scripts with automated tooth segmentation models for a fully hands-off morphometric measurement pipeline.
