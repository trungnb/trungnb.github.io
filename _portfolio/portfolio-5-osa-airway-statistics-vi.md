---
title: "Luận văn Thạc sĩ: Phân tích Kích thước Đường thở trên Bệnh nhân OSA (R)"
excerpt: "Luồng phân tích R có tính tái lập để so sánh nhóm và trực quan hóa số đo đường thở trên CBCT ở người có OSA.<br/><img src='https://img.shields.io/badge/Tech-R_%7C_ggplot2_%7C_dplyr-blue'>"
collection: portfolio
date: 2025-09-09
lang: vi
permalink: /vi/portfolio/portfolio-5-osa-airway-statistics/
---
**Công nghệ sử dụng:** R, RMarkdown, `dplyr`, `tidyr`, `ggplot2`, `ggpubr`, `effsize`  
**Bài báo liên quan:** *Kích thước đường thở trên phim CBCT ở người Việt có và không có hội chứng ngưng thở khi ngủ: Báo cáo hàng loạt ca* (Tạp chí Y học Việt Nam, 2025)

### Tổng quan
Kho lưu trữ này chứa các kịch bản phân tích dữ liệu có tính tái lập được phát triển cho Luận văn Thạc sĩ của mình về Hội chứng ngưng thở khi ngủ (OSA). Làm việc với dữ liệu phim CBCT, mình đã trực tiếp viết kịch bản R để tiền xử lý số liệu, trực quan hóa và thực hiện các kiểm định thống kê so sánh kích thước hình thái đường thở trên giữa hai nhóm, trực tiếp hỗ trợ cho bài báo khoa học công bố trên Tạp chí Y học Việt Nam (2025).

### Động lực thực hiện
Đối với Luận văn Thạc sĩ, mình cần xử lý và so sánh các số đo thể tích và diện tích tiết diện cắt ngang của đường thở trên. Thay vì chỉ phụ thuộc vào các phần mềm thống kê thao tác bằng chuột (như SPSS), mình chọn học và sử dụng ngôn ngữ R để đảm bảo tính tái lập (reproducibility), làm sạch dữ liệu bằng code và xuất biểu đồ đạt chuẩn quy cách bài báo quốc tế.

### Phương pháp Kỹ thuật
* Làm sạch và tiền xử lý dữ liệu lâm sàng và số đo CBCT từ 11 ca (loạt ca người Việt có và không có OSA).
* Kiểm tra các giả định phân phối bằng kiểm định Shapiro-Wilk (phân phối chuẩn) và F-test (tính đồng nhất phương sai).
* So sánh giữa 2 nhóm bằng kiểm định phi tham số Wilcoxon rank-sum (Mann-Whitney U) cho các biến kích thước đường thở (MinCSA, Thể tích, MinAP, MinLR) và kiểm định chính xác Fisher cho biến giới tính.
* Đo lường độ lớn ảnh hưởng phi tham số bằng chỉ số Cliff's delta (`effsize`).
* Lập trình hàm vẽ biểu đồ Boxplot kết hợp điểm dữ liệu phân tán (jitter) và thanh chú thích giá trị p tự động bằng `ggplot2` và `ggpubr` (xuất ảnh 1200 DPI phục vụ bài báo).

### Bài học Rút ra & Hướng phát triển
Có thêm kinh nghiệm thực hành về tiền xử lý dữ liệu bằng code, kiểm định giả thuyết phi tham số và trực quan hóa khoa học trong R. **Hướng phát triển:** Mở rộng luồng bằng Python để hỗ trợ trích xuất số đo 3D, đi kèm bước kiểm chứng phù hợp.
