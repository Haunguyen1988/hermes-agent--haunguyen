# [TÊN DỰ ÁN] — AI Session Rules

> File này được thêm dưới tên `AGENTS_PROJECT.md` để tránh ghi đè `AGENTS.md` hệ thống đang có sẵn trong repo.
> Khi cần dùng cho một codebase dự án riêng, có thể đổi tên file này thành `AGENTS.md`.

## 🚨 BẮT ĐẦU MỖI SESSION: ĐỌC NGAY CÁC FILE SAU
1. `memory-bank/activeContext.md` — Trạng thái hiện tại & bước tiếp theo
2. `memory-bank/progress.md` — Những gì đã làm & còn lại

Sau khi đọc, **xác nhận ngắn gọn**: "Tôi đã đọc context. Hiện tại dự án đang [X], bước tiếp theo là [Y]. Tôi sẵn sàng tiếp tục."

---

## 📦 Tech Stack
- **Language**: [Python 3.x / Node.js / etc.]
- **Framework**: [FastAPI / Django / React / etc.]
- **Database**: [PostgreSQL / MongoDB / etc.]
- **Tools**: [Docker / VSCode / Power BI / N8N / etc.]
- **Deployment**: [Local / Docker / Cloud / etc.]

## 📁 Cấu trúc thư mục
```
project-root/
├── src/              # Source code chính
├── tests/            # Unit & integration tests
├── docs/             # Documentation
├── memory-bank/      # AI context files (đọc đầu session)
└── scripts/          # Utility scripts
```

## ✅ Quy tắc bắt buộc (DO)
- Luôn đọc `activeContext.md` trước khi làm bất cứ gì
- Đặt tên biến/function theo [camelCase / snake_case]
- Viết docstring cho mọi function
- Hỏi trước khi tạo file mới hoặc thay đổi cấu trúc
- Xác nhận hiểu yêu cầu trước khi code

## ❌ Tuyệt đối không làm (DON'T)
- Không xóa file chưa hỏi ý kiến
- Không thêm dependency mới chưa được approve
- Không hardcode credentials, API key
- Không push thẳng lên branch main/master
- Không tự ý thay đổi database schema

## 🔧 Lệnh quan trọng
```bash
# Setup môi trường
[lệnh setup]

# Chạy local
[lệnh run]

# Chạy test
[lệnh test]

# Build
[lệnh build]
```

## 🔚 KẾT THÚC MỖI SESSION
Trước khi đóng, cập nhật:
- `memory-bank/activeContext.md` — trạng thái mới, bước tiếp theo
- `memory-bank/progress.md` — log những gì đã làm hôm nay
