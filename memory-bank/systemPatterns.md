# System Patterns — [TÊN DỰ ÁN]

> Ghi lại kiến trúc và design patterns đã chọn. Cập nhật sau mỗi quyết định kiến trúc lớn.

---

## 🏗️ Kiến trúc tổng quan
```
[Vẽ sơ đồ bằng text hoặc mô tả luồng dữ liệu]

Ví dụ:
[Data Source] → [ETL/Parser] → [Database] → [API Layer] → [Frontend/Dashboard]
      ↑                                           ↓
  [Scheduler]                              [Notification]
```

## 📐 Design Patterns đang dùng

| Pattern | Áp dụng ở đâu | Lý do chọn |
|---------|--------------|-----------|
| [Repository Pattern] | [Data access layer] | [Tách logic DB khỏi business logic] |
| [Factory Pattern] | [Message parser] | [Xử lý nhiều loại message format] |
| [Observer Pattern] | [Event notifications] | [Loosely coupled components] |

## 🔄 Data Flow chính
1. **[Flow 1 - Tên]**: [Mô tả luồng từ input → output]
2. **[Flow 2 - Tên]**: [Mô tả luồng từ input → output]

## 🧩 Các module/component chính

| Module | Trách nhiệm | File/Folder |
|--------|-------------|-------------|
| [Module A] | [Làm gì] | `src/module_a/` |
| [Module B] | [Làm gì] | `src/module_b/` |

## 🔗 Quan hệ giữa các components
- [Component A] gọi [Component B] khi [điều kiện]
- [Component C] phụ thuộc vào [Component D]
- [Module X] là singleton, không khởi tạo lại

## 📏 Coding Conventions
- **Naming**: [snake_case cho Python / camelCase cho JS]
- **File structure**: [Mỗi module trong folder riêng]
- **Error handling**: [Dùng custom exceptions, log tất cả errors]
- **Testing**: [Unit test cho business logic, integration test cho API]

---
*Cập nhật lần cuối: [YYYY-MM-DD]*
