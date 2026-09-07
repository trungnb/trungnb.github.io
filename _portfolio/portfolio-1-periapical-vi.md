---
title: "PeriApicaI: Nền tảng AI Đào tạo X-quang"
excerpt: "Nền tảng lâm sàng tương tác sử dụng LLM Đa phương thức (Gemini Vision) để phân tích lỗi X-quang và khoanh vùng tổn thương.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'> <img src='https://img.shields.io/badge/Ph%C6%B0%C6%A1ng_ph%C3%A1p-Vibe_Coding_%26_Prompt_Eng-purple'>"
collection: portfolio
date: 2026-08-01
lang: vi
permalink: /vi/portfolio/portfolio-1-periapical/
---
**Đường dẫn dự án:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Công nghệ sử dụng:** Multimodal LLMs (Gemini Vision), Kỹ nghệ câu lệnh (Prompt Engineering), Phát triển có AI hỗ trợ (Vibe Coding), Express, Firebase  

### Tổng quan
Phim X-quang nha khoa đòi hỏi kỹ năng nhận diện hình ảnh rất cao, nhưng sinh viên thường thiếu phản hồi tức thì do quỹ thời gian của giảng viên eo hẹp. Để lấp đầy khoảng trống này, mình đã phát triển **PeriApicaI**—một ứng dụng web đóng vai trò như trợ giảng ảo. Được xây dựng từ góc nhìn của một bác sĩ lâm sàng thông qua phương pháp **phát triển có AI hỗ trợ (vibe coding)** kết hợp cùng **kỹ nghệ câu lệnh (prompt engineering)** chuyên sâu, nền tảng đã nhanh chóng chuyển mình từ bản thử nghiệm sơ bộ thành một hệ thống sẵn sàng vận hành thực tế (production-ready). Nền tảng đánh giá phim X-quang quanh chóp theo thời gian thực, cung cấp phản hồi tức thì về lỗi kỹ thuật chụp cũng như khoanh vùng tổn thương, giúp sinh viên và nha sĩ rèn luyện kỹ năng chẩn đoán với các rào chắn an toàn y khoa chặt chẽ.

### Tính năng Nổi bật & Kỹ thuật

* **Luồng Phân tích Toàn diện:** Hỗ trợ song song hai luồng đánh giá: Phát hiện lỗi kỹ thuật chụp (VD: cắt nón, kéo dài răng) và Phân đoạn Tổn thương (nhận diện và khoanh vùng 8 loại bệnh lý nha khoa khác nhau).
* **Kiến trúc Hội chẩn AI (Dual-Model Consensus):** Khởi chạy đồng thời 2 mô hình (VD: Gemini Pro & Flash) để đối chiếu chéo tọa độ vùng bệnh lý. Cơ chế này loại bỏ các ảo giác (hallucination) đơn lẻ và gán nhãn độ tin cậy rõ ràng ("Hội chẩn" vs "Cần rà soát").
* **Xác thực Ngữ nghĩa & Lưu trữ Nguồn gốc (Provenance):** Hệ thống schema backend bắt lỗi đầu ra của AI và ép buộc sử dụng các thuật ngữ bệnh lý y khoa chuẩn. Mọi chẩn đoán đều được lưu vết chi tiết (lineage) gồm ID mô hình, thông tin xác thực, và điểm tin cậy gốc trước khi có sự can thiệp của con người.
* **Hạ tầng Ổn định cấp Production:** Tối ưu hóa API quota với các cơ chế dự phòng mô hình (fallback ladders), Execution Budget, và AbortController để chặn luồng AI thừa. Tích hợp hàng đợi ngoại tuyến (offline-recovery queue) đảm bảo đồng bộ dữ liệu mượt mà kể cả khi rớt mạng.

### Bài học Rút ra & Hướng phát triển
Dự án giúp mình làm chủ kỹ nghệ câu lệnh (prompt engineering) phức tạp cho AI đa phương thức và cách kiềm chế "ảo giác" của LLM thông qua thuật toán đối chiếu tọa độ. **Hướng phát triển:** Triển khai thử nghiệm lâm sàng quy mô lớn thông qua bộ công cụ thẩm định/duyệt kết quả (human-review adjudication) vừa được xây dựng, tạo tiền đề fine-tune mô hình với bộ dữ liệu chuẩn y khoa.
