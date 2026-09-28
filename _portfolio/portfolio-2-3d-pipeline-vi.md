---
title: "Prototype Phân tích Hình dạng Sọ mặt 3D-to-2D"
excerpt: "Proof-of-concept trên hai CBCT, khảo sát hình chiếu sọ mặt đa hướng gọn nhẹ cho quy trình định danh pháp y tiềm năng.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_Python-purple'>"
collection: portfolio
translation_key: portfolio-2-3d-pipeline
date: 2026-07-17
lang: vi
permalink: /vi/portfolio/portfolio-2-3d-pipeline/
---
**Kho lưu trữ dự án (GitHub):** [3D-Craniofacial-Pipeline](https://github.com/trungnb/3D-Craniofacial-Pipeline)  
**Công nghệ sử dụng:** Python, TotalSegmentator, NiBabel, NumPy, Pandas  

### Tổng quan
Proof-of-concept trên hai CBCT, so sánh các hình chiếu 2D gọn nhẹ của cấu trúc sọ mặt đã phân vùng với mask 3D tương ứng. Các lần chạy đã lưu được dùng để khảo sát tính lặp lại tính toán, thời gian so sánh, dung lượng lưu trữ và độ chồng lấp giữa hai ca.

### Cách tiếp cận
* Phân vùng cấu trúc sọ mặt, chiếu từng mask theo ba hướng axial, coronal và sagittal, rồi so sánh đầu ra 2D với 3D bằng thời gian, dung lượng, Dice và IoU.
* Các hình chiếu lặp lại từ cùng một scan có độ nhất quán cao và đầu ra 2D có chi phí so sánh đã lưu thấp hơn; với chỉ hai ca, kết quả chưa chứng minh độ chính xác định danh hay giá trị lâm sàng.
