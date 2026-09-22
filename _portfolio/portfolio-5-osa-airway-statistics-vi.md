---
title: "Luận văn Thạc sĩ: Phân tích Kích thước Đường thở trên Bệnh nhân OSA (R)"
excerpt: "Luồng phân tích R có tính tái lập để so sánh nhóm và trực quan hóa số đo đường thở trên CBCT ở người có OSA.<br/><img src='https://img.shields.io/badge/Tech-R_%7C_ggplot2_%7C_dplyr-blue'>"
collection: portfolio
translation_key: portfolio-5-osa-airway-statistics
date: 2025-09-09
lang: vi
permalink: /vi/portfolio/portfolio-5-osa-airway-statistics/
---
**Công nghệ sử dụng:** R, RMarkdown, `dplyr`, `tidyr`, `ggplot2`, `ggpubr`, `effsize`  
**Bài báo liên quan:** *Kích thước đường thở trên phim CBCT ở người Việt có và không có hội chứng ngưng thở khi ngủ: Báo cáo hàng loạt ca* (Tạp chí Y học Việt Nam, 2025)

### Tổng quan
Luồng R có tính tái lập cho luận văn Thạc sĩ và bài báo *Tạp chí Y học Việt Nam* về hình thái đường thở trên CBCT ở loạt ca 11 người Việt có và không có OSA.

### Cách tiếp cận
* Làm sạch dữ liệu và so sánh số đo đường thở bằng Wilcoxon rank-sum, Fisher và Cliff's delta.
* Lập biểu đồ bài báo bằng `ggplot2` và `ggpubr`; mọi mở rộng trích xuất 3D bằng Python cần được kiểm chứng.
