---
title: "Dental Morphometrics: CEJ & Crown-Root Ratio"
excerpt: "Proof-of-concept Python notebooks for exploratory CEJ and crown-root measurements from segmented 3D dental data.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
lang: en
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Tech Stack:** Python, Jupyter / Google Colab, NiBabel, NumPy, SciPy (`ndimage`), scikit-learn (PCA), Pandas, Matplotlib, Plotly  

### Overview
Proof-of-concept Python notebooks for anatomical alignment, exploratory CEJ localisation, and crown-root ratios from segmented 3D dental NIfTI data.

### Approach
* Applied PCA alignment, binary erosion, and HU profiling along the tooth axis.
* Exported ratio tables and interactive visualisations; repeatability must be assessed before research use.
