---
title: "Hình thái học Nha khoa: CEJ & Tỷ lệ Thân-Chân răng"
excerpt: "Quantitative Python analysis workflow for calculating Crown-Root ratios and identifying the Cementoenamel Junction (CEJ) from 3D dental models.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
date: 2026-07-28
lang: vi
permalink: /vi/portfolio/portfolio-6-dental-cej-morphometrics/
---
**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Tech Stack:** Python, Jupyter, Scikit-Image, Pandas, Data Visualization

### Tổng quan
Việc đo đạc 3D thủ công trong nha khoa vô cùng tốn thời gian. Với mong muốn tự học kiến thức cơ bản về thị giác máy tính, mình đã viết một kịch bản Python thử nghiệm để tự động hóa việc nhận diện CEJ và tính tỷ lệ thân-chân răng từ file NIfTI. Dù mới ở bước đầu, dự án nhỏ này giúp mình làm quen với các thuật toán trích xuất đặc trưng hình ảnh.

### Động lực thực hiện
Việc click chuột thủ công qua các mô hình 3D nha khoa để tìm các mốc giải phẫu như Đường nối men-ngà (CEJ) cực kỳ tốn thời gian. Mình bắt đầu dự án này để xem liệu các thuật toán Python cơ bản có thể gánh vác phần việc nặng nhọc này và giảm thiểu sai số của con người hay không.

### Phương pháp Kỹ thuật
* Tải và thao tác với các hình ảnh khối 3D (định dạng NIfTI) bằng Python.
* Thử nghiệm các kỹ thuật phát hiện biên (edge detection) và tạo mặt nạ (masking) cơ bản để phân lập ranh giới răng.
* Viết các hàm toán học thử nghiệm để tính toán các tỷ lệ giải phẫu (ví dụ: Thân-Chân răng).

### Bài học Rút ra & Hướng phát triển
Có được hiểu biết nền tảng về thao tác mảng 3D và dữ liệu voxel trong Python. **Hướng phát triển:** Mục tiêu là tích hợp các kịch bản này với các mô hình phân vùng răng tự động để tạo ra một luồng đo lường hình thái học hoàn toàn tự động.
