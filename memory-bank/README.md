# 📚 Memory Bank — Hướng dẫn sử dụng

Thư mục này là "bộ nhớ ngoài" của AI. Mỗi file phục vụ một mục đích khác nhau.

---

## 📁 Danh sách file & mục đích

| File | Mục đích | Cập nhật khi nào |
|------|----------|-----------------|
| `projectbrief.md` | Mục tiêu, scope, timeline dự án | Hiếm — chỉ khi scope thay đổi |
| `productContext.md` | Business logic, user journey, rules nghiệp vụ | Khi có feature lớn mới |
| `systemPatterns.md` | Kiến trúc, design patterns, quan hệ modules | Sau quyết định kiến trúc |
| `techContext.md` | Tech stack, setup, dependencies, env vars | Khi thay đổi tech |
| `activeContext.md` | **Trạng thái hiện tại, bước tiếp theo** | **Mỗi session** |
| `progress.md` | Log tiến độ, backlog, known bugs | **Mỗi session** |
| `decisions-log.md` | Lịch sử quyết định kiến trúc + lý do | Khi có quyết định quan trọng |
| `SESSION_HANDOFF.md` | Handoff khi context đầy | Khi cần chuyển session |

---

## 🔄 Workflow hàng ngày

### ⏰ Đầu session (2 phút)
```
1. Mở session AI mới
2. Paste nội dung activeContext.md vào đầu conversation
   HOẶC gõ: "Đọc memory-bank/activeContext.md và cho tôi biết bạn hiểu gì"
3. AI xác nhận context → bắt đầu làm việc
```

### ⏰ Cuối session (3 phút)
```
Yêu cầu AI:
"Hãy cập nhật memory-bank/activeContext.md và memory-bank/progress.md.
Tóm tắt: (1) đã hoàn thành gì, (2) quyết định quan trọng,
(3) bước tiếp theo, (4) lưu ý cho session mai."
```

### 🔁 Khi context sắp đầy
```
"Context sắp đầy. Hãy tạo SESSION_HANDOFF.md với tóm tắt đầy đủ
và prompt để tôi bắt đầu session mới ngay lập tức."
```

---

## 📐 Nguyên tắc cốt lõi
1. **AI không nhớ** — bạn phải cho nó đọc context mỗi lần
2. **File = memory** — cập nhật thường xuyên = AI luôn hiểu đúng
3. **Ngắn gọn > dài dòng** — file quá dài AI bị overwhelm
4. **Luôn cập nhật activeContext.md** — đây là file quan trọng nhất
