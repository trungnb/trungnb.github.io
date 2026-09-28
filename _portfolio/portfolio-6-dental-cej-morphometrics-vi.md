---
title: "Hình thái Thân–Chân răng — Prototype Thử nghiệm"
excerpt: "Prototype CT hai ca dùng profile cường độ lớp vỏ ngoài để suy ra proxy thử nghiệm cho vùng chuyển tiếp thân–chân răng."
collection: portfolio
translation_key: portfolio-6-dental-cej-morphometrics
date: 2026-07-28
lang: vi
permalink: /vi/portfolio/portfolio-6-dental-cej-morphometrics/
---
**Kho lưu trữ dự án (GitHub):** [Dental-CEJ-Morphometrics](https://github.com/trungnb/Dental-CEJ-Morphometrics)  
**Công nghệ sử dụng:** Python, NiBabel, NumPy, SciPy, scikit-learn (PCA), Pandas  

### Tổng quan
Prototype CT trên hai ca, khảo sát liệu profile cường độ ở lớp vỏ ngoài của răng có thể xác định một proxy dựa trên cường độ cho vùng chuyển tiếp thân–chân răng hay không. Phương pháp này không xác lập vị trí CEJ giải phẫu và chưa phải phép đo hình thái đã được thẩm định.

### Cách tiếp cận
* Căn chỉnh mask răng theo các trục chính, lấy mẫu lớp vỏ ngoài, tóm tắt profile cường độ theo từng lát và áp dụng heuristic để tạo tỷ lệ thân–chân răng thử nghiệm.
* Giữ lại các ca thất bại thay vì loại bỏ; phương pháp chưa có mốc CEJ thủ công, đánh giá giữa người đo, thẩm định ngoài hay ước lượng hiệu năng ở mức quần thể.
