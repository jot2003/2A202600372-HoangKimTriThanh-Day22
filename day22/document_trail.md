# Document Trail — AI PT Copilot

**Date:** 08/05/2026

---

## Bảng đối chiếu 5 loại hồ sơ

| # | Loại | Status | Link/Path | Deadline build |
|---|------|--------|-----------|----------------|
| 1 | Nhật ký kiểm thử claim AI | ✓ | `day22/marketing_claims_audit.md` | Duy trì hằng quý / trước campaign |
| 2 | Hồ sơ rà soát điều khoản vendor | ✗ | Chưa có file chuẩn | 20/05/2026 |
| 3 | Nhật ký giám sát giao dịch bất thường / abuse | ✗ | Chưa có dashboard rulebook | 24/05/2026 |
| 4 | DPIA / CTIA | ✗ | Chưa nộp chính thức | 15/06/2026 |
| 5 | Phê duyệt nội dung marketing (founder ký) | ✗ | Chưa có mẫu sign-off | 16/05/2026 |

---

## TOP 1 ưu tiên

**Loại:** **#5 — Phê duyệt nội dung marketing (founder ký)**  
**Lý do:** Rủi ro gần nhất và lặp lại hằng tuần; nếu không có gate ký duyệt, team rất dễ lặp pattern Kera (claim vượt evidence) và chạm Điều 198 BLHS.

---

## Template build trong 1 tuần

### Người chịu trách nhiệm
- **Owner:** Hoàng Kim Trí Thành (Founder)
- **Reviewer:** 1 PM + 1 Marketing lead

### Tần suất cập nhật
- Trước mỗi launch campaign, mỗi livestream, và mỗi lần thay hero copy landing page.

### Sample 3-5 dòng (mẫu sign-off)

```markdown
# Marketing Approval Log — [YYYY-MM-DD]
- Campaign: [Tên chiến dịch]
- Claim chính: "[câu claim]"
- Evidence đính kèm: [link A/B test / benchmark / user study]
- Risk level (A/B/C): [A/B/C]
- Founder decision: APPROVE / REVISE / REJECT
- Founder sign: [Tên + timestamp]
```

---

## Kế hoạch tuần này (concrete)

- Day 1: tạo Notion database "Marketing Approval Log".  
- Day 2: migrate 10 claim đang chạy vào log + gán mức A/B/C.  
- Day 3: khóa publish rights: campaign mới không có founder sign thì không live.

---

## Kế hoạch 30 ngày để đóng 4 ô còn thiếu

| Loại hồ sơ thiếu | Tuần 1 | Tuần 2 | Tuần 3-4 | Chi phí ước tính |
|---|---|---|---|---:|
| Vendor terms review | Liệt kê toàn bộ vendor + điều khoản dữ liệu | Chốt review checklist hằng quý | Lưu biên bản review phiên đầu | $0-$100 |
| Abuse monitoring log | Định nghĩa abuse signals + threshold | Bật dashboard + escalation 24h | Chạy dry-run 2 incident giả lập | $0-$50 |
| DPIA/CTIA | Vẽ luồng dữ liệu chi tiết | Soạn draft hồ sơ | Nộp và lưu proof nộp | $0-$300 (tư vấn) |
| Marketing approval gate | Tạo template + owner matrix | Khóa publish nếu chưa sign | Audit random 5 claim/tuần | $0 |

---

## KPI theo dõi document trail

- Tỷ lệ campaign có founder sign trước publish: **100%**  
- Tỷ lệ incident có đủ evidence trail trong 24h: **>= 95%**  
- Tỷ lệ vendor có biên bản review trong quý: **100%**

