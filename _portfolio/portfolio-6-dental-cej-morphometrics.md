---
title: "Dental Morphometrics: CEJ & Crown-Root Ratio"
excerpt: "Proof-of-concept Python notebooks for exploratory CEJ and crown-root measurements from segmented 3D dental data.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
lang: en
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Tech Stack:** Python, Jupyter, NiBabel, NumPy, SciPy (`ndimage`), Pandas, Matplotlib  

### Overview
Manual 3D measurements in dentistry can be time-consuming. To explore computational dental anatomy, I wrote proof-of-concept Python notebooks in Jupyter for anatomical alignment, exploratory CEJ localization, and crown-root ratio calculations from segmented NIfTI data. The project provided practical experience with 3D voxel manipulation and coordinate transformations.

### Motivation
Manually clicking through 3D dental models to find landmarks like the Cementoenamel Junction (CEJ) is time-consuming and subjective. I explored whether programmatic coordinate alignment and voxel density profiling could assist in standardizing dental morphometric extraction.

### Technical Approach
* Loaded and manipulated 3D volumetric images (NIfTI format) using NiBabel and NumPy.
* Applied 3D binary erosion on segmented tooth masks to isolate the outer shell voxel layer.
* Performed Principal Component Analysis (PCA) on 3D tooth coordinates to calculate the principal anatomical axis and rotate it to the Z-axis using affine transforms.
* Profiled cross-sectional Hounsfield Unit (HU) statistics (mean, min, max, std) along the Z-axis to detect density transitions at the CEJ boundary.
* Scripted functions to compute anatomical ratios (Crown-to-Root) and pulp chamber volume.

### Key Learnings & Future Work
Gained a foundational understanding of manipulating 3D arrays and voxel data in Python. **Future Work:** Assess the repeatability of these exploratory measurements and investigate whether they can be integrated with automated tooth-segmentation models.
