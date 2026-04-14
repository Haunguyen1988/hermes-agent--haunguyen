# Tech Context — Hermes Agent for Hau

> Cập nhật khi thay đổi dependencies hoặc tech stack.

---

## 🛠️ Tech Stack chi tiết

| Layer | Technology | Version | Ghi chú |
|-------|-----------|---------|---------|
| Language | Python | Existing in Hermes repo | Nền agent/runtime hiện có |
| Framework / Agent Runtime | Hermes agent codebase | Existing repo version | Dùng làm base platform |
| Knowledge Layer | Markdown files | N/A | Context, templates, skills, examples, memory-bank |
| Repository | GitHub | N/A | Lưu toàn bộ workspace và project memory |
| Frontend | None at init stage | N/A | Chưa có UI riêng cho project này |
| Automation | Future optional | N/A | Có thể bổ sung sau nếu cần |
| Deployment | Local / repo-based workspace | N/A | Giai đoạn init ưu tiên file-based workflow |

## 📦 Dependencies chính
```
# Hiện tại kế thừa dependencies có sẵn từ Hermes repo.
# Phase init này chưa thêm dependency mới cho project layer của Hau.
```

## 🔧 Setup môi trường local
```bash
# 1. Clone repo
git clone https://github.com/Haunguyen1988/hermes-agent--haunguyen.git
cd hermes-agent--haunguyen

# 2. Đọc workspace guidance
# - README_HAU_WORKSPACE.md
# - memory-bank/README.md
# - memory-bank/activeContext.md

# 3. Nếu chạy Hermes local, dùng setup của repo gốc
# (theo tài liệu / môi trường hiện có của Hermes repository)

# 4. Bắt đầu dùng workspace layer
# - Chọn skill liên quan
# - Dùng template phù hợp
# - Cập nhật memory-bank sau mỗi session
```

## 🔐 Biến môi trường (.env)
```
# Workspace layer này không yêu cầu thêm env mới ở bước init.
# Nếu chạy Hermes hoặc các integration sau này, dùng env theo repo gốc và không commit giá trị thật.
```

## 🗂️ External Services / Integrations
| Service | Mục đích | Auth method |
|---------|----------|-------------|
| GitHub | Lưu file workspace | GitHub auth / repo access |
| Hermes runtime | Chạy agent framework | Theo config repo gốc |
| Future vendor/project docs | Context cho task thật | Tùy connector / manual upload |
| Future reporting tools | Dashboard/reporting support | Tùy nền tảng sau này |

## ⚠️ Known Issues / Gotchas kỹ thuật
- Workspace layer hiện dựa mạnh vào markdown context files, nên chất lượng phụ thuộc vào việc cập nhật đều và dùng thật.
- Repo gốc đã có `AGENTS.md`, vì vậy project rules được đặt tại `AGENTS_PROJECT.md` để tránh xung đột.
- GitHub connector hiện thuận tiện cho việc tạo file mới, nhưng việc ghi đè file sẵn có có thể cần thao tác khác hoặc copy thủ công.

---
*Cập nhật lần cuối: 2026-04-14*
