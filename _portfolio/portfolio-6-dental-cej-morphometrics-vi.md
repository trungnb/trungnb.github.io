---
title: "Hình thái học Nha khoa: CEJ & Tỷ lệ Thân-Chân răng"
excerpt: "Các notebook Python thử nghiệm về CEJ và số đo thân-chân răng từ dữ liệu răng 3D đã phân vùng.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
lang: vi
permalink: /vi/portfolio/portfolio-6-dental-cej-morphometrics/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook & Dữ liệu](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Công nghệ sử dụng:** Python, Jupyter / Google Colab, NiBabel, NumPy, SciPy (`ndimage`), scikit-learn (PCA), Pandas, Matplotlib, Plotly  

### Tổng quan
Notebook Python proof-of-concept về căn chỉnh trục, định vị CEJ thử nghiệm và tính tỷ lệ thân-chân răng từ dữ liệu NIfTI nha khoa 3D đã phân vùng.

### Cách tiếp cận
* Áp dụng căn chỉnh PCA, bào mòn nhị phân và khảo sát HU dọc trục răng.
* Xuất bảng tỷ lệ và trực quan hoá tương tác; cần đánh giá tính lặp lại trước khi dùng cho nghiên cứu.
