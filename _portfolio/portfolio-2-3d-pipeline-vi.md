---
title: "Thử nghiệm Phân tích Sọ mặt 3D"
excerpt: "Luồng Python thử nghiệm với TotalSegmentator và NiBabel trên dữ liệu NIfTI 3D.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_Python-purple'>"
collection: portfolio
translation_key: portfolio-2-3d-pipeline
date: 2026-07-17
lang: vi
permalink: /vi/portfolio/portfolio-2-3d-pipeline/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook & Dữ liệu](https://drive.google.com/drive/folders/1M2Ebwdb7axTtll17ci1lYitd3eLlkHBu?usp=sharing)  
**Công nghệ sử dụng:** Python, TotalSegmentator, NiBabel, Pandas, Matplotlib  

### Tổng quan
Các nghiên cứu giải phẫu có thể tốn nhiều thời gian ở khâu phân vùng thủ công. Để tự học xử lý ảnh y khoa, mình đã thử nghiệm TotalSegmentator trên dữ liệu NIfTI 3D và kiểm tra các cấu trúc, số đo đầu ra. Đây là một bài thực hành ban đầu về việc sử dụng một công cụ deep learning có sẵn cho dữ liệu sọ mặt.

### Động lực thực hiện
Trong quá trình thu thập dữ liệu nghiên cứu, mình nhận ra việc tô vẽ mặt nạ (masking) trên từng lát cắt CBCT thủ công là cực kỳ kém hiệu quả. Mình muốn bước ra khỏi lối mòn lâm sàng để tìm hiểu các công cụ deep learning mã nguồn mở có thể tự động hóa quy trình nhàm chán này.

### Phương pháp Kỹ thuật
* Thiết lập môi trường Python để chạy TotalSegmentator trên các khối dữ liệu NIfTI.
* Thử nghiệm trích xuất các cấu trúc như hộp sọ, xương hàm dưới, răng và vùng liên quan đến đường thở.
* Tính một số thể tích mẫu và tạo hình chiếu 2D từ các mảng 3D đã phân vùng.

### Bài học Rút ra & Hướng phát triển
Làm quen với việc chạy một công cụ phân vùng có sẵn và xử lý mảng dữ liệu 3D y khoa bằng NiBabel. **Hướng phát triển:** Đánh giá chất lượng phân vùng và, nếu phù hợp, kết nối luồng này với phân tích hình thái học thống kê trong nghiên cứu chỉnh nha.
