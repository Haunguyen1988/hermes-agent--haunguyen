# 🚀 Hướng dẫn Setup Memory Bank cho Dự án Mới

## Bước 1: Copy template vào dự án
```bash
# Copy thư mục memory-bank vào root của project
cp -r memory-bank-template/memory-bank ./
cp memory-bank-template/CLAUDE.md ./
cp memory-bank-template/AGENTS.md ./
cp memory-bank-template/.cursorrules ./
```

## Bước 2: Điền thông tin vào từng file (theo thứ tự)

### Ưu tiên 1 — Làm ngay (mất ~15 phút)
- [ ] `CLAUDE.md` — Điền tech stack, quy tắc dự án, lệnh build/test
- [ ] `memory-bank/projectbrief.md` — Điền mục tiêu, scope, deadline
- [ ] `memory-bank/activeContext.md` — Điền trạng thái ban đầu

### Ưu tiên 2 — Làm trong ngày đầu
- [ ] `memory-bank/techContext.md` — Điền stack chi tiết, setup guide
- [ ] `memory-bank/productContext.md` — Điền business rules, user journey

### Ưu tiên 3 — Bổ sung dần
- [ ] `memory-bank/systemPatterns.md` — Cập nhật khi có kiến trúc rõ ràng
- [ ] `memory-bank/decisions-log.md` — Ghi quyết định từ ngày đầu

## Bước 3: Thêm vào .gitignore (nếu có thông tin nhạy cảm)
```bash
# Thêm vào .gitignore nếu memory-bank chứa thông tin nội bộ
# Hoặc giữ trong repo nếu muốn team cùng dùng
```

## Bước 4: Workflow hàng ngày
Xem `memory-bank/README.md` để biết cách dùng hàng ngày.

---

## 🔧 Tùy chỉnh theo công cụ AI

| Công cụ | File cần đổi tên | Ghi chú |
|---------|-----------------|---------|
| **Claude Code** | `CLAUDE.md` | Đọc tự động |
| **Cursor** | `.cursorrules` | Đọc tự động |
| **Windsurf** | `.windsurfrules` | Copy nội dung CLAUDE.md |
| **GitHub Copilot** | `.github/copilot-instructions.md` | Copy nội dung CLAUDE.md |
| **OpenAI Codex** | `AGENTS.md` | Đọc tự động |
| **ChatGPT/Claude web** | Paste thủ công | Copy activeContext.md vào đầu chat |
