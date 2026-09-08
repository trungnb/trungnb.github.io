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
Dự án gồm các notebook nhỏ để tìm hiểu cách CTGAN và ctdGAN mô hình hóa dữ liệu dạng bảng. Mình sử dụng các biến nhân trắc học giả lập như tuổi, chủng tộc và giới tính, sau đó so sánh dữ liệu tạo ra với phân phối ban đầu. Đây là các thử nghiệm phục vụ học tập; dự án không chứng minh khả năng ẩn danh hay bảo đảm riêng tư cho dữ liệu lâm sàng.

### Động lực thực hiện
Mình quan tâm đến dữ liệu tổng hợp vì dữ liệu lâm sàng cần được quản trị cẩn thận và không phải lúc nào cũng có thể chia sẻ công khai. Mục tiêu của dự án là hiểu quy trình cơ bản và các giới hạn của nó, không phải khẳng định dữ liệu tổng hợp tự động giải quyết rủi ro riêng tư.

### Phương pháp Kỹ thuật
* Sử dụng các triển khai CTGAN và ctdGAN để tạo mẫu từ các bộ dữ liệu nhân trắc học giả lập nhỏ.
* So sánh một số phân phối và thống kê tóm tắt giữa dữ liệu đầu vào và dữ liệu được tạo ra.
* Sử dụng SDMetrics và một số kiểm tra bằng mô hình hạ nguồn để tìm hiểu độ trung thực và tính hữu ích; đây không phải một cuộc kiểm toán riêng tư chính thức.

### Bài học Rút ra & Hướng phát triển
Nắm được các khái niệm cơ bản về mô hình sinh dữ liệu dạng bảng, đánh giá phân phối và sự khác nhau giữa dữ liệu tổng hợp với bảo vệ riêng tư đã được chứng minh. **Hướng phát triển:** Tìm hiểu đánh giá rủi ro riêng tư và quản trị dữ liệu trước khi thử nghiệm với các biến lâm sàng phức tạp hơn.
