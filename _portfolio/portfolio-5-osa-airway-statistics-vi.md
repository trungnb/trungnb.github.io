---
title: "Luận văn: Mô hình Thống kê Đường thở"
excerpt: "Statistical analysis workflow in R for evaluating airway morphometrics in Obstructive Sleep Apnea (Master's Graduation Thesis).<br/><img src='https://img.shields.io/badge/Tech-R_%7C_ggplot2_%7C_dplyr-blue'>"
collection: portfolio
date: 2025-09-09
lang: vi
permalink: /vi/portfolio/portfolio-5-osa-airway-statistics/
---
**Tech Stack:** R, RMarkdown, `dplyr`, `ggplot2`, `ggpubr`, `effsize`  
**Related Publication:** *Upper Airway Dimensions on CBCT in Vietnamese Subjects with and without Obstructive Sleep Apnea* (Vietnam Medical Journal, 2025)

### Tổng quan
Kho lưu trữ này chứa các kịch bản mô hình hóa thống kê được phát triển cho Luận văn Thạc sĩ của mình về Hội chứng ngưng thở khi ngủ (OSA). Làm việc với dữ liệu CBCT, mình đã viết các kịch bản R để làm sạch, trực quan hóa và phân tích thống kê hình thái học đường thở trên, trực tiếp hỗ trợ cho một bài báo khoa học đã được công bố.

### Động lực thực hiện
Đối với Luận văn Thạc sĩ, mình cần xử lý và phân tích các số đo thể tích phức tạp của đường thở trên. Thay vì chỉ phụ thuộc vào các phần mềm thống kê thao tác bằng chuột (như SPSS), mình muốn học ngôn ngữ R để đảm bảo tính tái lập (reproducibility) và vẽ biểu đồ dữ liệu bằng code.

### Phương pháp Kỹ thuật
* Xử lý và làm sạch một bộ dữ liệu lâm sàng gồm 111 số đo từ phim CBCT.
* Viết kịch bản R có tính tái lập sử dụng `dplyr` để thao tác dữ liệu và `ggplot2`/`ggpubr` để vẽ biểu đồ thống kê.
* Thực hiện các phân tích đa biến để đánh giá mối tương quan giữa kích thước đường thở và mức độ nghiêm trọng của OSA.

### Bài học Rút ra & Hướng phát triển
Nắm vững các kiến thức cơ bản về thao tác dữ liệu bằng code, xử lý giá trị thiếu (missing values) và trực quan hóa khoa học trong R. **Hướng phát triển:** Đã sử dụng thành công luồng làm việc này để xuất bản một bài báo; bước tiếp theo là sử dụng Python để tự động hóa giai đoạn trích xuất dữ liệu ban đầu.
