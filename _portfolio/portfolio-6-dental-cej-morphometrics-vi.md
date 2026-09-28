---
title: "Hình thái Thân–Chân răng — Prototype Thử nghiệm"
excerpt: "Prototype CT hai ca dùng profile cường độ lớp vỏ ngoài để suy ra proxy thử nghiệm cho vùng chuyển tiếp thân–chân răng."
collection: portfolio
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
lang: vi
permalink: /vi/portfolio/portfolio-6-dental-cej-morphometrics/
---
**Kho lưu trữ dự án (GitHub):** [Crown-Root-Transition-Morphometrics](https://github.com/trungnb/Dental-CEJ-Morphometrics)  
**Công nghệ sử dụng:** Python, NiBabel, NumPy, SciPy, scikit-learn (PCA), Pandas  

### Tổng quan
Prototype CT trên hai ca, khảo sát liệu profile cường độ ở lớp vỏ ngoài của răng có thể xác định một proxy dựa trên cường độ cho vùng chuyển tiếp thân–chân răng hay không. Phương pháp này không xác lập vị trí CEJ giải phẫu và chưa phải phép đo hình thái đã được thẩm định.

### Cách tiếp cận
* Căn chỉnh mask răng theo các trục chính, lấy mẫu lớp vỏ ngoài dày ba voxel, tóm tắt profile cường độ theo từng lát và dùng heuristic để suy ra tỷ lệ thử nghiệm (thân + vùng chuyển tiếp)/độ dài chân răng.
* PCA lịch sử dùng tọa độ chỉ số voxel; phương pháp chưa có mốc CEJ giải phẫu, đánh giá giữa người đo, thẩm định ngoài hay ước lượng hiệu năng ở mức quần thể.
