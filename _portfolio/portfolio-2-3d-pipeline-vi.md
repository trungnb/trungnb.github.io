---
title: "Thử nghiệm Phân tích Sọ mặt 3D"
excerpt: "Luồng Python thử nghiệm với TotalSegmentator và NiBabel trên dữ liệu NIfTI 3D.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_Python-purple'>"
collection: portfolio
translation_key: portfolio-2-3d-pipeline
date: 2026-07-17
lang: vi
permalink: /vi/portfolio/portfolio-2-3d-pipeline/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook](https://drive.google.com/drive/folders/1M2Ebwdb7axTtll17ci1lYitd3eLlkHBu?usp=sharing)  
**Công nghệ sử dụng:** Python, TotalSegmentator, NiBabel, Pandas, Matplotlib  

### Tổng quan
Notebook thử nghiệm TotalSegmentator và NiBabel trên dữ liệu NIfTI sọ mặt 3D. Đây là thực hành giai đoạn đầu với công cụ phân vùng có sẵn, không phải luồng đã được thẩm định.

### Cách tiếp cận
* Trích xuất cấu trúc sọ mặt, tạo hình chiếu 2D và tính thể tích mẫu.
* So sánh các lần chạy bằng Dice và IoU; cần đánh giá chất lượng phân vùng trước khi dùng cho nghiên cứu.
