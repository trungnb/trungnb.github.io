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
Phim X-quang nha khoa đòi hỏi kỹ năng nhận diện hình ảnh rất cao, nhưng sinh viên thường thiếu phản hồi tức thì do quỹ thời gian của giảng viên eo hẹp. Để lấp đầy khoảng trống này, mình đã phát triển **PeriApicaI**—một ứng dụng web đóng vai trò như trợ giảng ảo. Nền tảng đánh giá phim X-quang quanh chóp theo thời gian thực, cung cấp phản hồi tức thì về lỗi kỹ thuật chụp cũng như khoanh vùng tổn thương, giúp sinh viên và nha sĩ nhanh chóng rèn luyện kỹ năng chẩn đoán.

### Tính năng Nổi bật & Kỹ thuật

* **Luồng Phân tích Toàn diện:** Hỗ trợ song song hai luồng đánh giá: Phát hiện lỗi kỹ thuật chụp (VD: cắt nón, kéo dài răng) và Phân đoạn Tổn thương (nhận diện và khoanh vùng 8 loại bệnh lý nha khoa khác nhau).
* **Kiến trúc Hội chẩn AI (Dual-Model Consensus):** Khởi chạy đồng thời 2 mô hình (VD: Gemini Pro & Flash) để đối chiếu chéo tọa độ vùng bệnh lý. Cơ chế này loại bỏ các ảo giác (hallucination) đơn lẻ và gán nhãn độ tin cậy rõ ràng ("Hội chẩn" vs "Cần rà soát").
* **Semantic Validation Engine:** Xây dựng cơ chế xác thực lược đồ (schema) backend cứng, bắt lỗi đầu ra của AI, giới hạn điểm tin cậy, và ép buộc AI chỉ được phép dùng các thuật ngữ bệnh lý y khoa chuẩn nhằm đảm bảo tính chính xác lâm sàng.
* **Hạ tầng Ổn định & Tối ưu:** Tối ưu hóa API quota với Execution Budget và AbortController để tự động dừng các luồng AI thừa khi người dùng thoát tab. Tích hợp hàng đợi ngoại tuyến (offline queue) để đồng bộ dữ liệu mượt mà kể cả khi rớt mạng.

### Bài học Rút ra & Hướng phát triển
Dự án giúp mình làm chủ kỹ nghệ câu lệnh (prompt engineering) phức tạp cho AI đa phương thức và cách kiềm chế "ảo giác" của LLM thông qua xác thực cấu trúc JSON và thuật toán đối chiếu tọa độ song song. **Hướng phát triển:** Tinh chỉnh (fine-tune) mô hình với tập dữ liệu X-quang y khoa riêng để cải thiện độ chính xác không gian tuyệt đối.
