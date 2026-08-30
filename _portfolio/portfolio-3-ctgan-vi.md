---
title: "Tổng hợp Dữ liệu Y tế Dạng bảng"
excerpt: "Conditional Tabular GANs for generating privacy-preserving synthetic demographic medical data.<br/><img src='https://img.shields.io/badge/Tech-Generative_AI_%7C_CTGAN-green'>"
collection: portfolio
date: 2026-06-15
lang: vi
permalink: /vi/portfolio/portfolio-3-ctgan/
---
**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1qInNhtiGobzpOIexIhhCxGZT5zZTeWID?usp=sharing)  
**Tech Stack:** Python, CTGAN, ctdGAN, Scikit-Learn, Differential Privacy  

### Tổng quan
Một rào cản lớn khi làm AI y tế là sự khan hiếm các bộ dữ liệu lâm sàng mã nguồn mở do luật bảo mật nghiêm ngặt. Để tìm hiểu về bảo mật dữ liệu, mình đã thử nghiệm dùng CTGAN và ctdGAN để tổng hợp dữ liệu nhân trắc học nhân tạo (Tuổi, Chủng tộc, Giới tính). Dự án khám phá này là bước đầu giúp mình hiểu cách các nhà nghiên cứu có thể chia sẻ dữ liệu y tế an toàn trong tương lai.

### Động lực thực hiện
Khi đọc các bài báo nghiên cứu AI, mình nhận thấy việc tiếp cận dữ liệu lâm sàng rất khó khăn do đạo luật HIPAA và quyền bảo mật bệnh nhân. Mình trở nên tò mò muốn biết việc Tổng hợp Dữ liệu Nhân tạo (Synthetic Data Generation) có thể giải quyết điểm nghẽn này như thế nào.

### Phương pháp Kỹ thuật
* Sử dụng hệ sinh thái Synthetic Data Vault (SDV) để huấn luyện các mô hình CTGAN và ctdGAN.
* Cung cấp một mẫu dữ liệu nhân trắc học giả định để mô hình học các phân phối thống kê.
* Đánh giá độ trung thực của dữ liệu được tạo ra và các chỉ số bảo mật so với bộ dữ liệu gốc.

### Bài học Rút ra & Hướng phát triển
Nắm bắt các khái niệm cơ bản về Mạng đối nghịch tạo sinh (GANs) và các chiến lược ẩn danh dữ liệu hiện đại. **Hướng phát triển:** Thử nghiệm tổng hợp các đặc trưng lâm sàng phức tạp hơn (như chẩn đoán và kết quả điều trị) trong khi vẫn giữ nguyên các mối quan hệ thống kê ẩn.
