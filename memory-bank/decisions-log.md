# Decisions Log — [TÊN DỰ ÁN]

> Ghi lại TẤT CẢ quyết định quan trọng về kiến trúc, công nghệ, business logic.
> Mục đích: Không bao giờ phải tranh luận lại quyết định đã có lý do rõ ràng.
> Append-only — không xóa quyết định cũ.

---

## Template cho mỗi quyết định:

### [YYYY-MM-DD] — [Tiêu đề quyết định ngắn gọn]
- **Context**: [Tại sao phải đưa ra quyết định này? Bối cảnh là gì?]
- **Options đã xem xét**:
  - Option A: [Tên] — Pros: [...] | Cons: [...]
  - Option B: [Tên] — Pros: [...] | Cons: [...]
- **Quyết định**: Chọn **[Option X]**
- **Lý do**: [Giải thích tại sao chọn option này]
- **Trade-offs chấp nhận**: [Điều gì bị đánh đổi]
- **Có thể thay đổi nếu**: [Điều kiện nào thì sẽ xem xét lại]

---

## Lịch sử quyết định

### [YYYY-MM-DD] — [Ví dụ: Chọn PostgreSQL làm database chính]
- **Context**: Cần lưu trữ dữ liệu có cấu trúc, cần ACID transactions
- **Options đã xem xét**:
  - PostgreSQL — Pros: ACID, rich query, mature | Cons: scale horizontal khó
  - MongoDB — Pros: flexible schema, scale out | Cons: eventual consistency
- **Quyết định**: Chọn **PostgreSQL**
- **Lý do**: Schema cố định, cần JOIN phức tạp, team có kinh nghiệm sẵn
- **Trade-offs chấp nhận**: Setup phức tạp hơn
- **Có thể thay đổi nếu**: Dataset tăng >10TB, cần horizontal scaling

---
*(Thêm quyết định mới phía dưới)*
