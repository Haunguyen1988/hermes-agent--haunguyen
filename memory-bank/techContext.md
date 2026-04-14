# Tech Context — [TÊN DỰ ÁN]

> Cập nhật khi thay đổi dependencies hoặc tech stack.

---

## 🛠️ Tech Stack chi tiết

| Layer | Technology | Version | Ghi chú |
|-------|-----------|---------|---------|
| Language | [Python] | [3.11] | |
| Framework | [FastAPI] | [x.x] | |
| Database | [PostgreSQL] | [15] | |
| ORM | [SQLAlchemy] | [x.x] | |
| Frontend | [React / Power BI] | [x.x] | |
| Automation | [N8N] | [x.x] | |
| Container | [Docker] | [x.x] | |
| CI/CD | [GitHub Actions] | | |

## 📦 Dependencies chính
```
# requirements.txt hoặc package.json chính
[dependency 1]==[version]
[dependency 2]==[version]
```

## 🔧 Setup môi trường local
```bash
# 1. Clone repo
git clone [repo-url]
cd [project-folder]

# 2. Tạo virtual environment (Python)
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

# 3. Cài dependencies
pip install -r requirements.txt

# 4. Setup biến môi trường
cp .env.example .env
# Điền các giá trị cần thiết vào .env

# 5. Chạy migrations (nếu có)
[lệnh migration]

# 6. Chạy app
[lệnh chạy]
```

## 🔐 Biến môi trường (.env)
```
# Không điền giá trị thật vào đây — chỉ liệt kê tên biến
DATABASE_URL=
API_KEY=
SECRET_KEY=
[tên biến khác]=
```

## 🗂️ External Services / Integrations
| Service | Mục đích | Auth method |
|---------|----------|-------------|
| [AIMS API] | [lấy flight data] | [API Token] |
| [Power BI] | [dashboard] | [OAuth] |
| [N8N] | [automation] | [Webhook] |

## ⚠️ Known Issues / Gotchas kỹ thuật
- [Vấn đề kỹ thuật cần biết khi làm việc với codebase này]
- [Quirk hoặc workaround đã áp dụng]

---
*Cập nhật lần cuối: [YYYY-MM-DD]*
