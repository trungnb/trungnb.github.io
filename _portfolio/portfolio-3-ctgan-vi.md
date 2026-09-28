---
title: "Benchmark Dữ liệu Tổng hợp ANSUR II với CTGAN & ctdGAN"
excerpt: "Benchmark ANSUR II hai giai đoạn: thử nghiệm fidelity–utility ban đầu và bản thiết kế phương pháp được cải tiến với hỗ trợ AI."
collection: portfolio
translation_key: portfolio-3-ctgan
date: 2026-06-15
lang: vi
permalink: /vi/portfolio/portfolio-3-ctgan/
---
**Kho lưu trữ dự án (GitHub):** [ANSUR-II-CTGAN-Benchmark](https://github.com/trungnb/ANSUR-II-CTGAN-Benchmark)  
**Công nghệ sử dụng:** Python, CTGAN, ctdGAN, SDMetrics, Scikit-Learn, XGBoost, GitHub Actions  

### Tổng quan
Dự án hai giai đoạn trên bộ dữ liệu nhân trắc học ANSUR II (n=6.068). V1 gồm các thử nghiệm ban đầu của tôi kết hợp độ tương đồng thống kê với tính hữu ích dự đoán; V2 là bản thiết kế lại có hỗ trợ AI, tập trung vào so sánh công bằng hơn, khả năng tái lập và benchmark nhiều seed.

### Cách tiếp cận
* Đánh giá CTGAN và ctdGAN bằng các chỉ số chất lượng phân phối cùng TRTR/TSTR trên nhiều mô hình hạ nguồn và biến đích.
* Thiết kế lại benchmark với chia dữ liệu thực cố định, chọn đặc trưng chỉ trên tập huấn luyện, cấu hình generator tương ứng, năm seed, khoảng tin cậy, baseline và GitHub Actions; đây là benchmark nhân trắc học, không phải nghiên cứu lâm sàng hay thẩm định riêng tư.
