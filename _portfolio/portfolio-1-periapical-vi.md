---
title: "PeriApicaI: Nền tảng AI Đào tạo X-quang"
excerpt: "Prototype web thử nghiệm dùng Gemini Vision để hỗ trợ rà soát phim X-quang quanh chóp.<br/><img src='https://img.shields.io/badge/Prototype-periapical.ai.studio-blue'> <img src='https://img.shields.io/badge/Methodology-AI--assisted_development_%26_prompt_design-purple'>"
collection: portfolio
date: 2026-08-01
lang: vi
permalink: /vi/portfolio/portfolio-1-periapical/
---
**Đường dẫn dự án:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Công nghệ sử dụng:** Multimodal LLMs (Gemini Vision), Thiết kế Prompt, Phát triển có hỗ trợ AI  

### Tổng quan
Đọc phim X-quang nha khoa đòi hỏi sự thận trọng, nhưng người học không phải lúc nào cũng có thể nhận được phản hồi ngay từ giảng viên. Mình phát triển **PeriApicaI** như một prototype web thử nghiệm để tìm hiểu liệu AI đa phương thức có thể hỗ trợ việc học từ phim X-quang quanh chóp hay không. Dự án được xây dựng từ góc nhìn lâm sàng với phương pháp phát triển có hỗ trợ AI và thiết kế prompt; ứng dụng đưa ra phản hồi tự động về chất lượng kỹ thuật và các vùng phát hiện tiềm năng để người học rà soát. Kết quả chỉ có tính tham khảo; dự án chưa được thẩm định lâm sàng và không phải thiết bị y tế.

### Tính năng Nổi bật & Kỹ thuật

* **Hai luồng đánh giá:** Hỗ trợ rà soát chất lượng kỹ thuật (ví dụ: cắt nón, kéo dài răng) và khoanh vùng phát hiện tiềm năng theo taxonomy của dự án.
* **Đối chiếu hai mô hình tùy chọn:** Có thể chạy Gemini Flash và Gemini Pro song song, so sánh kết quả và tọa độ polygon, sau đó gắn nhãn mức độ đồng thuận hoặc trường hợp cần rà soát.
* **Xác thực và lưu vết:** Schema backend chuẩn hóa đầu ra theo từ điển nha khoa; lineage của lượt suy luận và trạng thái rà soát nối tiếp giúp tách kết quả của mô hình khỏi quyết định rà soát về sau.
* **Các cơ chế tăng độ ổn định:** Có xử lý fallback mô hình, giới hạn thực thi, hủy request bằng `AbortController` và cơ chế khôi phục có giới hạn cho lỗi tạm thời.

### Bài học Rút ra & Hướng phát triển
Dự án giúp mình có kinh nghiệm thực hành về thiết kế prompt đa phương thức, đối chiếu mô hình, xác thực schema và xây dựng luồng rà soát của con người. **Hướng phát triển:** Đánh giá prototype trên bộ dữ liệu có quản trị phù hợp, có nhãn và được rà soát độc lập trước khi đưa ra bất kỳ kết luận nào về hiệu năng hoặc ứng dụng lâm sàng.
