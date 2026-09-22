---
title: "Tổng hợp Dữ liệu Y tế Dạng bảng"
excerpt: "Các notebook CTGAN và ctdGAN thử nghiệm trên dữ liệu nhân trắc học giả lập.<br/><img src='https://img.shields.io/badge/Tech-CTGAN_%7C_ctdGAN_%7C_Python-green'>"
collection: portfolio
translation_key: portfolio-3-ctgan
date: 2026-06-15
lang: vi
permalink: /vi/portfolio/portfolio-3-ctgan/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook & Dữ liệu](https://drive.google.com/drive/folders/1qInNhtiGobzpOIexIhhCxGZT5zZTeWID?usp=sharing)  
**Công nghệ sử dụng:** Python, CTGAN, ctdGAN, SDMetrics, Pandas, NumPy, Scikit-Learn  

### Tổng quan
Notebook thử nghiệm CTGAN và ctdGAN trên dữ liệu nhân trắc học giả lập. Dự án phục vụ học cách đánh giá phân phối, không chứng minh khả năng ẩn danh hay bảo đảm riêng tư cho dữ liệu lâm sàng.

### Cách tiếp cận
* Tạo mẫu và so sánh một số phân phối, thống kê tóm tắt giữa dữ liệu đầu vào và dữ liệu được tạo ra.
* Dùng SDMetrics và kiểm tra mô hình hạ nguồn đơn giản để tìm hiểu độ trung thực và tính hữu ích; đây không phải kiểm toán riêng tư chính thức.
