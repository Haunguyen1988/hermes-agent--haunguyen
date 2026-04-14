# Project Brief — Hermes Agent for Hau

> **⚠️ File này là nền tảng của toàn bộ Memory Bank. Chỉ cập nhật khi scope thay đổi lớn.**

---

## 🎯 Mục tiêu dự án
Xây dựng một workspace AI thực chiến trên nền Hermes để hỗ trợ Nguyễn Đình Hậu trong công việc hàng ngày liên quan đến AIMS, SOP/document writing, project coordination, vendor management, analytics/reporting, và governance.
Mục tiêu là biến repo này thành một "professional AI operating layer" giúp giảm rework, giữ context qua nhiều session, và tạo ra output dùng được ngay trong công việc.

## 👤 Người dùng mục tiêu
- **Primary user — Hau**: cần AI copilot hiểu đúng domain hàng không, AIMS, cách viết tài liệu, cách làm việc với vendor, và cách chuẩn bị output cho management.
- **Future collaborators / AI sessions**: cần đọc context nhanh, hiểu trạng thái dự án, và tiếp tục công việc mà không phải hỏi lại từ đầu.

## 📋 Yêu cầu cốt lõi (Core Requirements)
1. Tạo một lớp identity + style + domain knowledge + templates + examples để agent làm việc đúng "chất Hau".
2. Thiết lập memory-bank để mỗi session có thể tiếp tục mượt, có progress tracking, decisions log, và handoff.
3. Tạo các skill và reusable templates cho SOP, AIMS analysis, project coordination, vendor communication, analytics/reporting, governance, và execution tracking.
4. Tạo sanitized real examples để agent học từ pattern thật nhưng không làm lộ dữ liệu nhạy cảm.
5. Cho phép mở rộng dần workspace thành một AI operating system cho công việc chuyên môn của Hau.

## 🚫 Ngoài scope (Out of Scope)
- Không build production application hoàn chỉnh ở giai đoạn init này.
- Không đưa dữ liệu vận hành nhạy cảm, credentials, hay tài liệu raw confidential vào repo.
- Không cố gắng cấu hình toàn bộ automation/platform integration ngay trong bước khởi tạo đầu tiên.

## 📅 Timeline
- **Bắt đầu**: 2026-04-14
- **Deadline**: Ongoing
- **Milestones**:
  - 2026-04-14: Hoàn thành lớp nền workspace, templates, skills, examples, sanitized examples, memory-bank init
  - 2026-04-15: Điền first-pass các file memory-bank và bắt đầu dùng repo như một project operating workspace
  - 2026-04-16 trở đi: Bổ sung real cases, refine rules, và dùng thật cho các task AIMS / SOP / project / vendor

## 🔗 Tài liệu liên quan
- `README_HAU_WORKSPACE.md`
- `SOUL.md`
- `AGENTS_HAU_LAYER.md`
- `skills/`
- `context/`
- `kb/examples-real/`

---
*Cập nhật lần cuối: 2026-04-14 bởi AWF/Antigravity*
