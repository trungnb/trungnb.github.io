---
title: "Phân tích Hình thái Sọ mặt 3D"
excerpt: "Automated deep learning workflow using TotalSegmentator for processing 3D CBCT/CT scans.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_PyTorch-purple'>"
collection: portfolio
date: 2026-07-17
lang: vi
permalink: /vi/portfolio/portfolio-2-3d-pipeline/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook & Dữ liệu](https://drive.google.com/drive/folders/1M2Ebwdb7axTtll17ci1lYitd3eLlkHBu?usp=sharing)  
**Công nghệ sử dụng:** Python, TotalSegmentator, NiBabel, PyTorch, Pandas  

### Tổng quan
Các nghiên cứu giải phẫu thường bị đình trệ do khâu phân vùng CBCT thủ công chậm chạp. Nhằm mục đích tự học xử lý ảnh y khoa, mình đã thử nghiệm TotalSegmentator để xem liệu có thể tự động hóa việc trích xuất sọ mặt hay không. Những thử nghiệm bước đầu này giúp mình làm quen với cách deep learning có thể hỗ trợ thu thập dữ liệu chỉnh nha.

### Động lực thực hiện
Trong quá trình thu thập dữ liệu nghiên cứu, mình nhận ra việc tô vẽ mặt nạ (masking) trên từng lát cắt CBCT thủ công là cực kỳ kém hiệu quả. Mình muốn bước ra khỏi lối mòn lâm sàng để tìm hiểu các công cụ deep learning mã nguồn mở có thể tự động hóa quy trình nhàm chán này.

### Phương pháp Kỹ thuật
* Thiết lập môi trường Python cơ bản để chạy TotalSegmentator trên phim CBCT (định dạng NIfTI).
* Thử nghiệm trích xuất tự động hộp sọ, xương hàm dưới và các răng riêng lẻ.
* Thử nghiệm tạo các hình chiếu vuông góc 2D từ khối dữ liệu 3D đã được phân vùng.

### Bài học Rút ra & Hướng phát triển
Làm quen với quy trình deep learning qua terminal và cách xử lý mảng dữ liệu 3D y khoa bằng thư viện NiBabel. **Hướng phát triển:** Mục tiêu là kết hợp bước phân vùng tự động này với các luồng phân tích hình thái học thống kê trong nghiên cứu chỉnh nha.
