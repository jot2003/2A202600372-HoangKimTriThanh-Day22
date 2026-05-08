# Territorial Scope — AI PT Copilot

**Date:** 08/05/2026

---

## Câu hỏi 1: User EU?

- Có user EU hiện tại: **0** (chưa mở bán EU).
- Kế hoạch mở rộng EU 12 tháng: **NO** (ưu tiên Việt Nam + SEA trước).
- **Kết luận:** EU AI Act áp dụng trực tiếp hiện tại = **NO** (theo phạm vi kinh doanh hiện tại), nhưng cần theo dõi mốc 02/08/2026 nếu chuyển sang high-risk use case hoặc nhận user EU.

---

## Câu hỏi 2: Dữ liệu Việt Nam?

### Loại dữ liệu cá nhân đang xử lý
1. Định danh cơ bản: tên, email, số điện thoại (nếu đăng ký tài khoản).
2. Dữ liệu hành vi trong app: thời lượng session, số rep, tỷ lệ ignore/accept cue.
3. Dữ liệu kỹ thuật thiết bị: IP, device model, log lỗi.
4. Dữ liệu hình ảnh/pose: keypoint metadata từ camera (không cần lưu video full-time trong mode chuẩn).
5. Dữ liệu hỗ trợ khách hàng: ticket, nội dung phản hồi.

### Có chuyển dữ liệu ra nước ngoài
- Có: dùng API/infra vendor nước ngoài (OpenAI/Anthropic và cloud region ngoài VN cho một số thành phần).

### Kết luận
- **PDPL áp dụng = YES** (gần như chắc chắn).  
- **CTIA = YES** (có chuyển dữ liệu cá nhân xuyên biên giới qua vendor/infra nước ngoài).

---

## Câu hỏi 3: Tầng rủi ro Luật AI VN (Điều 9)?

- **Phân loại hiện tại:** **Trung bình** (chatbot/gen AI coaching, chưa là hệ thống y tế/tài chính/hành pháp bắt buộc cao).
- **Lập luận:** sản phẩm đưa khuyến nghị hành vi luyện tập, không ra quyết định pháp lý/tín dụng/tuyển dụng; tuy nhiên có tác động tới an toàn cá nhân nên cần governance chặt.
- **Nghĩa vụ tương ứng:** minh bạch giới hạn hệ thống, logging/monitoring, quy trình incident response, hồ sơ đánh giá rủi ro định kỳ.

---

## 4 deadlines đã note vào Notion/Calendar

- [x] 01/01/2026 — PDPL hiệu lực (đã qua)
- [x] 01/03/2026 — Luật AI VN hiệu lực (đã qua)
- [x] 02/08/2026 — EU AI Act high-risk milestone (đã note nhắc trước 30 ngày)
- [x] 01/03/2027 — Hết ân hạn chính sách liên quan (đã note nhắc trước 60 ngày)

---

## Founder decision trong 30 ngày

1. Khóa scope thị trường: không nhận user EU trong 12 tháng tới nếu chưa có legal readiness.  
2. Ưu tiên hoàn tất CTIA + cập nhật privacy policy trước khi scale paid UA.  
3. Định nghĩa rõ disclaimer y tế để tránh bị hiểu là medical advice.

