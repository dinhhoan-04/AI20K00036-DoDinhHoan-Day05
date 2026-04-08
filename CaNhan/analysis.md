# UX Exercise — Vietnam Airlines NEO

## 1. Marketing promise
Tính năng được giới thiệu là chatbot hỗ trợ khách hàng, giúp tra cứu/thao tác nhanh hơn thay vì tìm thủ công.

## 2. 4 paths

### Path 1 — Khi AI đúng
- User hỏi thông tin cơ bản, câu trả lời khớp ý.
- Hệ thống phản hồi nhanh, user không phải tìm menu sâu.
- Đây là path mạnh nhất vì tiết kiệm thời gian cho tác vụ đơn giản.

### Path 2 — Khi AI không chắc
- Khi câu hỏi mơ hồ hoặc thiếu dữ liệu, hệ thống chưa luôn nói rõ mức độ không chắc.
- Chưa phải lúc nào cũng đưa alternative rõ như nút gợi ý tiếp theo.
- Đây là điểm còn gãy.

### Path 3 — Khi AI sai
- Khi hiểu sai ý user, dấu hiệu sai đôi khi chỉ lộ ra qua câu trả lời lệch.
- Cách sửa còn phụ thuộc user tự gõ lại câu hỏi, chưa có flow “bạn có ý này không?” đủ rõ.
- Chi phí sửa lỗi cho user còn hơi cao.

### Path 4 — Khi user mất tin
- Có fallback sang kênh hỗ trợ khác nhưng chưa luôn nổi bật.
- Nếu user muốn người thật ngay, đường thoát nên rõ hơn trong cùng màn hình chat.

## 3. Path yếu nhất
Path yếu nhất là **low-confidence**.
Lý do: hệ thống chưa luôn biểu đạt “tôi không chắc”, nên user khó phân biệt giữa “AI đang chắc” và “AI đang đoán”.

## 4. Gap giữa marketing và thực tế
- Marketing hứa trải nghiệm hỗ trợ mượt và thông minh.
- Thực tế phù hợp ở câu hỏi đơn giản, nhưng ở trường hợp mơ hồ hoặc ngoài phạm vi thì trải nghiệm giảm nhanh.
- Gap lớn nhất nằm ở chỗ quản lý uncertainty, không phải ở giao diện cơ bản.


- Thêm trạng thái “Tôi chưa chắc, bạn muốn chọn 1 trong 3 hướng này không?”
- Thêm chip action: Tra cứu chuyến bay / Hành lý / Gặp hỗ trợ viên
- Khi AI trả lời có rủi ro sai, thêm nguồn hoặc bước xác nhận lại 
