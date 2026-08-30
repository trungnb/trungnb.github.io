---
title: "PeriApicaI: Nền tảng AI Đào tạo X-quang"
excerpt: "Interactive clinical platform utilizing Gemini Vision LLMs to diagnose periapical X-ray errors.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'>"
collection: portfolio
date: 2026-08-01
lang: vi
permalink: /vi/portfolio/portfolio-1-periapical/
---
**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tech Stack:** Multimodal Large Language Models (Gemini Vision), Prompt Engineering, Web Application  

### Tổng quan
Nhận thấy sinh viên nha khoa thường thiếu phản hồi tức thì về lỗi X-quang do quỹ thời gian của giảng viên eo hẹp, mình muốn tìm hiểu xem AI có thể hỗ trợ được không. Mình đã tự học và thử nghiệm làm một web app sơ bộ dùng AI Gemini để đánh giá lỗi X-quang. Đây là bước đầu để mình khám phá liệu AI tạo sinh có thể đóng vai trò như một trợ giảng ảo cơ bản trong tương lai hay không.

### Động lực thực hiện
Phim X-quang nha khoa đòi hỏi kỹ năng nhận diện hình ảnh rất cao. Giảng viên thường quá tải, khiến sinh viên phải tự loay hoay với các lỗi kỹ thuật (ví dụ: lỗi cắt nón, kéo dài răng). Mình muốn xem liệu các mô hình ngôn ngữ lớn đa phương thức (Multimodal LLMs) có thể lấp đầy khoảng trống giáo dục này.

### Phương pháp Kỹ thuật
* Tích hợp API Gemini Vision của Google để phân tích phim X-quang chóp tải lên.
* Thử nghiệm prompt engineering để định hướng AI chỉ tập trung vào các lỗi kỹ thuật X-quang chuẩn mực.
* Xây dựng giao diện web tương tác đơn giản để trả kết quả tức thời cho người dùng.

### Bài học Rút ra & Hướng phát triển
Học được cách thiết kế câu lệnh (prompt) cho AI đa phương thức nhằm giảm thiểu ảo giác (hallucination) trong bối cảnh hình ảnh y khoa. **Hướng phát triển:** Hy vọng cải thiện độ chính xác của AI bằng các kỹ thuật fine-tuning với một bộ dữ liệu X-quang nha khoa đã được dán nhãn chuẩn.
