# First Pass — Filled Content For Initial Project Files

This file contains the first-pass filled content for the 5 most important project-init files.

Project assumption for this first pass:
The project being initialized is **Hermes Agent for Hau** — a practical AI workspace and operating layer built on top of the Hermes repository to support Hau's real work in AIMS, SOP/document writing, implementation coordination, vendor follow-up, analytics/reporting, governance, and project continuity.

---

# 1) `memory-bank/projectbrief.md`

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
*Cập nhật lần cuối: 2026-04-14 bởi ChatGPT for Hau*

---

# 2) `memory-bank/activeContext.md`

# Active Context — Hermes Agent for Hau

> **🔁 FILE NÀY PHẢI CẬP NHẬT MỖI SESSION.**
> AI đọc file này đầu tiên. Giữ thông tin ngắn gọn, rõ ràng, luôn mới nhất.

---

## 📍 Trạng thái hiện tại
- **Cập nhật lần cuối**: 2026-04-14 07:20
- **Status**: [x] 🟢 On Track   [ ] 🟡 At Risk   [ ] 🔴 Blocked
- **Đang làm**: Hoàn thiện lớp nền project-init và đưa repo vào trạng thái có thể dùng như một AI workspace thật cho Hau.
- **Sprint/Iteration**: Phase 1 — Workspace Foundation & Project Init

---

## ✅ Hoàn thành (session gần nhất)
| Ngày | Task | Ghi chú |
|------|------|---------|
| 2026-04-14 | Tạo lớp identity, user profile, domain context, templates, and skills | `SOUL.md`, `context/`, `skills/` |
| 2026-04-14 | Tạo examples cho 3 skills chính | `skills/*/examples/` |
| 2026-04-14 | Tạo sanitized real examples và redaction policy | `kb/examples-real/` |
| 2026-04-14 | Init bộ `memory-bank/` và project session rules | `memory-bank/`, `CLAUDE.md`, `AGENTS_PROJECT.md` |

---

## 🔄 Đang làm dở (Work In Progress)
| Task | Tiến độ | File chính | Ghi chú |
|------|---------|-----------|---------|
| Điền first-pass cho 5 file memory-bank chính | 90% | `memory-bank/projectbrief.md`, `activeContext.md`, `productContext.md`, `techContext.md`, `progress.md` | Nội dung đã được soạn trong `memory-bank/FIRST_PASS.md` |
| Chuyển workspace từ template sang live operating system | 60% | `memory-bank/`, `README_HAU_WORKSPACE.md` | Cần bắt đầu dùng thật cho các task tiếp theo |

---

## 🔴 Blockers (Đang bị chặn)
| Vấn đề | Nguyên nhân | Kế hoạch giải quyết | Owner |
|--------|-------------|---------------------|-------|
| Chưa overwrite trực tiếp 5 file template bằng nội dung first-pass | GitHub connector hiện tại tạo file mới tốt nhưng không ghi đè file có sẵn theo đường nhanh | Tạm lưu nội dung chuẩn trong `memory-bank/FIRST_PASS.md`; khi cần sẽ copy vào 5 file chính hoặc dùng Git-level update nếu connector hỗ trợ | Agent / Hau |

---

## 🔑 Quyết định quan trọng (session gần nhất)
| Ngày | Quyết định | Lý do |
|------|-----------|-------|
| 2026-04-14 | Dùng repo Hermes hiện tại làm nền cho workspace riêng của Hau | Tận dụng agent framework có sẵn, đồng thời thêm lớp domain-specific và project memory |
| 2026-04-14 | Tạo `AGENTS_PROJECT.md` thay vì ghi đè `AGENTS.md` | Tránh phá file hệ thống đang có sẵn trong repo |
| 2026-04-14 | Lưu case thật dưới dạng sanitized examples | Giữ giá trị pattern nhưng vẫn an toàn dữ liệu |

*Chi tiết hơn → xem `decisions-log.md`*

---

## ⏭️ Bước tiếp theo (Ưu tiên từ cao xuống thấp)
1. 🔥 **Copy first-pass content từ `memory-bank/FIRST_PASS.md` vào 5 file memory-bank chính** — Ước tính: 20m — `memory-bank/*.md`
2. 📌 **Bắt đầu dùng workspace cho một use case thật đầu tiên** — ví dụ SOP AIMS user creation hoặc vendor clarification note — Ước tính: 1-2h — `skills/`, `context/`, `kb/examples-real/`
3. 💡 **Bổ sung 1-2 real sanitized cases mới sau khi dùng thật** — Ước tính: 1h — `kb/examples-real/`

---

## 📌 Lưu ý cho session tiếp theo
- ⚠️ Repo này hiện là workspace layer trên Hermes, không phải một application product độc lập.
- 💡 Ưu tiên dùng workspace này ngay cho task thật để tinh chỉnh rules và examples theo output thực tế.
- 📎 Khi bắt đầu session mới, AI nên đọc `memory-bank/activeContext.md`, `memory-bank/progress.md`, và `README_HAU_WORKSPACE.md` trước.

---

## 🔃 Cách cập nhật file này
Cuối session, yêu cầu AI:
```
"Hãy cập nhật memory-bank/activeContext.md dựa trên những gì chúng ta đã làm.
Điền: trạng thái mới, task đã xong, WIP, blockers, bước tiếp theo, lưu ý."
```

---

# 3) `memory-bank/productContext.md`

# Product Context — Hermes Agent for Hau

> Giải thích "tại sao" đằng sau mỗi quyết định sản phẩm. Cập nhật khi có feature mới lớn.

---

## 🧩 Vấn đề đang giải quyết
Hiện tại, nhiều công việc của Hau phải bắt đầu lại từ đầu trong mỗi session AI: giải thích context, style, domain, audience, template và cấu trúc output. Điều này làm mất thời gian, giảm tính nhất quán, và khiến output khó đạt đúng chất lượng mong muốn ngay từ vòng đầu.

**Trước khi có tool này:**
- Mỗi lần dùng AI phải giải thích lại bối cảnh AIMS, SOP, vendor, project, management output.
- Output có thể đúng nội dung nhưng không đúng structure, tone, hoặc mức sử dụng thực tế.
- Session continuity yếu, khó handoff, khó track decisions và progress.

**Sau khi có tool này:**
- Agent có sẵn identity, domain knowledge, templates, examples, sanitized real examples, và project memory.
- Giảm thời gian re-prompt và giảm số vòng chỉnh sửa.
- Dễ tiếp tục công việc qua nhiều session và nhiều loại task.

---

## 💡 Cách hoạt động (User Journey)
1. Hau mở repo hoặc session AI mới.
2. AI đọc `memory-bank/activeContext.md`, `progress.md`, và các file context/skill liên quan.
3. Hau giao task thực tế như SOP, fit-gap, vendor note, project plan, analytics summary.
4. Agent dùng identity + rules + templates + examples để tạo output đúng chất.
5. Cuối session, agent cập nhật lại `activeContext.md`, `progress.md`, và nếu cần thì `decisions-log.md` hoặc `SESSION_HANDOFF.md`.

---

## 🎨 UX Goals
- **Simplicity**: Hau không cần viết prompt quá dài mới ra đúng output.
- **Speed**: Có thể tạo first useful draft nhanh và chỉnh ít hơn.
- **Reliability**: Session mới vẫn hiểu dự án và tiếp tục được công việc mà không lệ thuộc hoàn toàn vào lịch sử chat.
- **Reuse**: Một output tốt có thể trở thành template, example, hoặc rule cho lần sau.

---

## 📏 Business Rules quan trọng
- **Rule 1**: Mọi output phải ưu tiên practical use hơn là lý thuyết hay wording hoa mỹ.
- **Rule 2**: Với management audience, output phải ngắn, sắc, decision-oriented.
- **Rule 3**: Với vendor audience, output phải formal English, rõ context, rõ câu hỏi, dễ trả lời.
- **Rule 4**: Không đưa dữ liệu vận hành nhạy cảm, thông tin cá nhân, credentials, hoặc chi tiết thương mại mật vào examples hoặc repo-safe files.
- **Rule 5**: Mỗi session phải có khả năng tiếp tục nhờ `memory-bank`, không dựa hoàn toàn vào trí nhớ chat.

---

## 🔗 Integrations & Dependencies bên ngoài
| System | Dùng để làm gì | Data lấy về |
|--------|---------------|-------------|
| Hermes repository | Nền agent framework | Skills, session rules, workspace structure |
| AIMS / airline operational context | Domain knowledge source | Workflow, access, issue, governance logic |
| GitHub repo | Lưu workspace, templates, sanitized examples, memory-bank | File-based project memory |
| Future tools (Power BI, n8n, vendor docs, project files) | Có thể bổ sung sau | Dashboard/reporting logic, automation context, case materials |

---
*Cập nhật lần cuối: 2026-04-14*

---

# 4) `memory-bank/techContext.md`

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
git clone [repo-url]
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

---

# 5) `memory-bank/progress.md`

# Progress Log — Hermes Agent for Hau

> Log tất cả những gì đã làm theo từng ngày. Append-only — không xóa lịch sử cũ.

---

## 📊 Tổng quan tiến độ

| Phase | Status | % Done | Target Date |
|-------|--------|--------|-------------|
| Phase 1: Workspace Foundation | 🟢 Done | 100% | 2026-04-14 |
| Phase 2: Memory Bank Init | 🟢 Done | 100% | 2026-04-14 |
| Phase 3: First-Pass Project Fill | 🟡 In Progress | 90% | 2026-04-14 |
| Phase 4: Real Use And Refinement | ⚪ Not Started | 0% | Ongoing |

---

## ✅ Đã hoàn thành

### 2026-04 — Workspace Init
- **2026-04-14**: Tạo `SOUL.md`, profile files, writing rules, airline domain context, templates, skills, and project-init plan.
- **2026-04-14**: Tạo examples cho `sop_writer`, `aims_analyst`, và `project_coordinator`.
- **2026-04-14**: Tạo `README_HAU_WORKSPACE.md` để giải thích cách dùng workspace.
- **2026-04-14**: Tạo sanitized real examples trong `kb/examples-real/` và `redaction-policy.md`.
- **2026-04-14**: Tạo `memory-bank/` templates, `CLAUDE.md`, và `AGENTS_PROJECT.md`.
- **2026-04-14**: Soạn first-pass filled content cho 5 file memory-bank chính trong `memory-bank/FIRST_PASS.md`.

---

## 🚧 Còn lại (Backlog)

### Must Have (P0 - Bắt buộc)
- [ ] Copy nội dung first-pass vào 5 file memory-bank chính
- [ ] Bắt đầu dùng workspace cho 1 use case thật đầu tiên
- [ ] Cập nhật `activeContext.md` và `progress.md` sau session dùng thật đầu tiên

### Should Have (P1 - Nên có)
- [ ] Bổ sung 1-2 sanitized real examples mới sau khi có task thật
- [ ] Tạo một decision entry đầu tiên trong `memory-bank/decisions-log.md`
- [ ] Chuẩn hóa naming / usage guide cho future collaborators nếu cần

### Nice to Have (P2 - Tốt nếu có)
- [ ] Tạo `.cursorrules` / Copilot instruction version nếu muốn dùng đa công cụ AI
- [ ] Tạo một small checklist cho "how to add new real example safely"

---

## 🐛 Known Bugs / Issues

| Bug | Severity | Phát hiện | Status |
|-----|----------|-----------|--------|
| First-pass chưa overwrite trực tiếp 5 file template chính | 🟡 Medium | 2026-04-14 | Workaround available |
| Một số project-init files vẫn đang ở dạng template và cần chuyển sang live content | 🟡 Medium | 2026-04-14 | In Progress |

---

## 📈 Metrics (nếu có)
| Metric | Target | Current | Updated |
|--------|--------|---------|---------|
| Workspace foundation completeness | 100% | 100% | 2026-04-14 |
| Core skill examples created | 3 skills fully covered | 3 skills covered | 2026-04-14 |
| Sanitized real examples created | 3-5 | 5 | 2026-04-14 |
| Memory-bank first-pass readiness | 100% | 90% | 2026-04-14 |
