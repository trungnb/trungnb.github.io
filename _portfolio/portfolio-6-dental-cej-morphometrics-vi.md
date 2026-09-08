---
title: "Hình thái học Nha khoa: CEJ & Tỷ lệ Thân-Chân răng"
excerpt: "Các notebook Python thử nghiệm về CEJ và số đo thân-chân răng từ dữ liệu răng 3D đã phân vùng.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
date: 2026-07-28
lang: vi
permalink: /vi/portfolio/portfolio-6-dental-cej-morphometrics/
---
**Kho lưu trữ dự án (Google Drive):** [Xem Notebook & Dữ liệu](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Công nghệ sử dụng:** Python, Jupyter, NiBabel, NumPy, SciPy (`ndimage`), Pandas, Matplotlib  

### Tổng quan
Việc đo đạc 3D thủ công trong nha khoa có thể tốn nhiều thời gian. Để khám phá giải phẫu răng bằng lập trình, mình đã viết các notebook Python thử nghiệm trong Jupyter về căn chỉnh trục giải phẫu, định vị CEJ ở mức thăm dò và tính tỷ lệ thân-chân răng từ dữ liệu NIfTI đã phân vùng. Dự án giúp mình có kinh nghiệm thực tế về thao tác voxel 3D và biến đổi hệ tọa độ.

### Động lực thực hiện
Việc click chuột thủ công trên các mô hình 3D nha khoa để tìm các mốc giải phẫu như Đường nối men-xê măng (CEJ) rất tốn thời gian và phụ thuộc chủ quan vào người đo. Mình thực hiện dự án này nhằm thử nghiệm xem việc tự động căn chỉnh tọa độ và quét tỷ trọng voxel có thể hỗ trợ chuẩn hóa quy trình trích xuất hình thái răng hay không.

### Phương pháp Kỹ thuật
* Tải và thao tác với các hình ảnh khối 3D (định dạng NIfTI) bằng NiBabel và NumPy.
* Ứng dụng phép bào mòn nhị phân 3D (Binary Erosion) trên mặt nạ răng để phân tách riêng lớp vỏ ngoài (outer shell voxels).
* Áp dụng Phân tích thành phần chính (PCA) trên tọa độ 3D của răng để tính toán trục giải phẫu chính và xoay trục dài của răng thẳng đứng theo trục Z qua biến đổi affine.
* Quét và phân tích biến thiên tỷ trọng Hounsfield Unit (HU) (mean, min, max, std) theo từng lát cắt trục Z để tìm ranh giới chuyển tiếp men-xê măng (CEJ).
* Viết các hàm tính toán tỷ lệ giải phẫu (thân-chân răng / Crown-to-Root) và thể tích buồng tủy.

### Bài học Rút ra & Hướng phát triển
Có được hiểu biết nền tảng về thao tác mảng 3D và dữ liệu voxel trong Python. **Hướng phát triển:** Đánh giá tính lặp lại của các số đo thử nghiệm và tìm hiểu khả năng kết hợp với mô hình phân vùng răng tự động.
