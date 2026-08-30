---
title: "PeriApicaI: Nền tảng AI Đào tạo X-quang"
excerpt: "Nền tảng lâm sàng tương tác sử dụng LLM Đa phương thức (Gemini Vision) để phân tích lỗi X-quang và khoanh vùng tổn thương.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'>"
collection: portfolio
date: 2026-08-01
lang: vi
permalink: /vi/portfolio/portfolio-1-periapical/
---
**Đường dẫn dự án:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Công nghệ sử dụng:** Multimodal LLMs (Gemini Vision), React/TypeScript, Prompt Engineering, Firebase  

### Tổng quan
Nhận thấy sinh viên nha khoa thường thiếu phản hồi tức thì về phim X-quang do quỹ thời gian của giảng viên eo hẹp, mình đã phát triển PeriApicaI. Với bản nâng cấp v2.8.9, ứng dụng hiện tích hợp luồng hội chẩn AI song song (Dual-model Consensus) và các lớp giáp bảo vệ ngữ nghĩa (Semantic Guardrails), biến AI tạo sinh thành một trợ giảng ảo an toàn và đáng tin cậy hơn.

### Tính năng Nổi bật & Kỹ thuật
* **Luồng Hội chẩn AI Song song:** Khởi chạy đồng thời 2 mô hình (VD: Gemini Pro & Flash) để đối chiếu chéo tọa độ vùng tổn thương (IoU Matching), giúp loại bỏ các ảo giác (hallucination) đơn lẻ và gán nhãn độ tin cậy rõ ràng ("Hội chẩn" vs "Cần rà soát").
* **Semantic Validation Engine:** Xây dựng cơ chế xác thực lược đồ (schema) backend cứng, bắt lỗi đầu ra của AI, giới hạn điểm tin cậy, và ép buộc AI chỉ được phép dùng các thuật ngữ bệnh lý chuẩn.
* **Phân đoạn Tổn thương (Pathology Segmentation):** Nâng cấp năng lực phân tích từ các lỗi kỹ thuật cơ bản (cắt nón, giãn ảnh) lên khả năng phát hiện và khoanh vùng 8 loại bệnh lý nha khoa khác nhau.
* **Tối ưu Quản lý Tài nguyên:** Xây dựng Execution Budget và AbortController để tự động dừng các luồng AI thừa khi người dùng thoát tab, bảo vệ hạn mức API và tăng độ ổn định.

### Bài học Rút ra & Hướng phát triển
Học được cách kỹ nghệ câu lệnh (prompt engineering) phức tạp cho AI đa phương thức và cách kiềm chế "ảo giác" của LLM thông qua xác thực cấu trúc JSON và đối chiếu song song. **Hướng phát triển:** Tinh chỉnh (fine-tune) mô hình với tập dữ liệu X-quang y khoa riêng để cải thiện độ chính xác không gian.
