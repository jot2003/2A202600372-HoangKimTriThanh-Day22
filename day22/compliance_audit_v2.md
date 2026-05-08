# Compliance Audit v2 — AI PT Copilot (AI-augmented)

**Ngày audit:** 08/05/2026  
**Nguồn đối chiếu:** PRD Day 17 + pitch/day19 + governance/day21 + workshop day22  
**Chuẩn audit:** Luật AI VN 134/2025/QH15, PDPL 91/2025/QH15, BLHS Điều 198/324, EU AI Act (phạm vi tham chiếu)

---

## Top vi phạm phát hiện (8 mục)

## VI PHẠM 1: Claim "thay thế PT" vượt bằng chứng
- **Luật áp dụng:** BLHS  
- **Điều:** Điều 198 (Lừa dối khách hàng), Khoản 2 nếu thu lợi bất chính vượt ngưỡng
- **Bằng chứng trong sản phẩm:** copy marketing từng dùng: "AI PT Copilot thay thế PT người"
- **Pattern khớp với:** **Kera** (thổi phồng công dụng không có chứng cứ đủ)
- **Hành động sửa (3 việc):**
  1. Gỡ toàn bộ claim tuyệt đối trong landing/deck/livestream script.
  2. Chỉ cho phép claim có evidence link trong approval log.
  3. Bắt buộc founder sign-off trước khi public.
- **Deadline:** 10/05/2026

---

## VI PHẠM 2: Claim hiệu suất "10x" không A/B test
- **Luật áp dụng:** BLHS
- **Điều:** Điều 198
- **Bằng chứng trong sản phẩm:** pitch/deck cũ có câu "AI tăng năng suất 10x"
- **Pattern khớp với:** **Kera**
- **Hành động sửa:**
  1. Thay bằng range có kiểm chứng (vd 10-40% theo cohort cụ thể).
  2. Đính A/B evidence ID cho mỗi claim mức A.
  3. Gắn nhãn "đang đo lường" cho claim mức B.
- **Deadline:** 11/05/2026

---

## VI PHẠM 3: "An toàn tuyệt đối" là claim không thể chứng minh
- **Luật áp dụng:** BLHS
- **Điều:** Điều 198
- **Bằng chứng:** script truyền thông cũ dùng cụm "an toàn tuyệt đối"
- **Pattern:** **Kera**
- **Hành động sửa:**
  1. Đổi toàn bộ copy sang "giảm lỗi phổ biến", không dùng từ tuyệt đối.
  2. Thêm disclaimer "không thay thế tư vấn y tế/chuyên gia".
  3. Review legal text mỗi quý.
- **Deadline:** 10/05/2026

---

## VI PHẠM 4: Chuyển dữ liệu cá nhân xuyên biên giới nhưng chưa hoàn tất CTIA
- **Luật áp dụng:** PDPL
- **Điều:** Điều 30 (chuyển dữ liệu cá nhân ra nước ngoài)
- **Bằng chứng:** sản phẩm dùng vendor AI/cloud ngoài VN, chưa có hồ sơ CTIA nộp
- **Pattern:** **CIC** (thiếu kiểm soát data governance dẫn tới rủi ro lớn)
- **Hành động sửa:**
  1. Lập và nộp CTIA với luồng dữ liệu hiện tại.
  2. Cập nhật privacy policy mô tả rõ nơi xử lý/lưu trữ.
  3. Thiết lập log truy cập dữ liệu cá nhân và retention policy.
- **Deadline:** 15/06/2026

---

## VI PHẠM 5: Quyền xóa dữ liệu chưa self-service rõ ràng
- **Luật áp dụng:** PDPL
- **Điều:** nghĩa vụ bảo vệ và xử lý minh bạch dữ liệu cá nhân (liên quan Điều 8/30)
- **Bằng chứng:** hiện mới có plan xóa dữ liệu, chưa triển khai flow tự phục vụ trong app
- **Pattern:** **CIC**
- **Hành động sửa:**
  1. Thêm nút "Delete my data" in-app + SLA xử lý.
  2. Lưu audit log cho mọi request xóa.
  3. Test định kỳ 1 lần/tháng để đảm bảo flow hoạt động.
- **Deadline:** 24/05/2026

---

## VI PHẠM 6: Chưa formal hóa phân loại tầng rủi ro AI theo Điều 9
- **Luật áp dụng:** Luật AI VN
- **Điều:** Điều 9 (phân tầng rủi ro và nghĩa vụ tương ứng)
- **Bằng chứng:** đã có nhận định "trung bình" trong workshop nhưng chưa thành tài liệu vận hành chính thức
- **Pattern:** không trực tiếp từ Kera/Pips/CIC; là gap tuân thủ hệ thống
- **Hành động sửa:**
  1. Ban hành note nội bộ "Risk tier = Medium" + điều kiện nâng cấp.
  2. Gắn checklist nghĩa vụ theo tier vào release process.
  3. Review lại tier mỗi quý hoặc khi mở thị trường mới.
- **Deadline:** 18/05/2026

---

## VI PHẠM 7: Rủi ro vendor/payment abuse monitoring còn mỏng
- **Luật áp dụng:** BLHS
- **Điều:** Điều 324 (Rửa tiền) — nguy cơ với nền tảng nếu biết dấu hiệu mà không chặn
- **Bằng chứng:** chưa có "abuse monitoring rulebook" đầy đủ cho khách hàng sử dụng sai mục đích
- **Pattern khớp với:** **Mr Pips / Shark Bình**
- **Hành động sửa:**
  1. Thiết lập abuse signals (volume bất thường, keywords lừa đảo, complaint ratio).
  2. Quy định escalation 24h: flag -> review -> block -> report log.
  3. Lưu evidence trail cho mọi quyết định block/allow.
- **Deadline:** 24/05/2026

---

## VI PHẠM 8: Founder approval gate chưa bắt buộc trước campaign
- **Luật áp dụng:** BLHS (gián tiếp phòng ngừa Điều 198)
- **Điều:** Điều 198 (giảm rủi ro claim sai sự thật)
- **Bằng chứng:** chưa có hệ thống bắt buộc "founder sign" trước launch
- **Pattern:** **Kera** (thiếu kiểm soát claim trước public)
- **Hành động sửa:**
  1. Tạo Marketing Approval Log có cột evidence.
  2. Khóa quyền publish nếu không có sign.
  3. Audit random 5 claim mỗi tuần.
- **Deadline:** 16/05/2026

---

## Top 5 nghiêm trọng nhất (ưu tiên xử lý)

1. Vi phạm 4 — CTIA/cross-border data (PDPL Điều 30)  
2. Vi phạm 1 — Claim "thay thế PT" (Điều 198)  
3. Vi phạm 2 — Claim "10x" không test (Điều 198)  
4. Vi phạm 7 — Abuse monitoring/payment risk (Điều 324 risk pattern)  
5. Vi phạm 5 — Data deletion flow chưa rõ (PDPL)

---

## Kết luận founder

Audit này cho thấy rủi ro lớn nhất không nằm ở model accuracy, mà nằm ở **claim marketing + data transfer + evidencing**. Nếu 3 lớp này không khóa trong 30 ngày tới, startup có thể tự đẩy mình vào pattern pháp lý giống Kera/Pips/CIC.

