# Active Context — Hermes Agent for Hau

> **🔁 FILE NÀY PHẢI CẬP NHẬT MỖI SESSION.**
> AI đọc file này đầu tiên. Giữ thông tin ngắn gọn, rõ ràng, luôn mới nhất.

---

## 📍 Trạng thái hiện tại
- **Cập nhật lần cuối**: 2026-04-14 14:47
- **Status**: [x] 🟢 On Track   [ ] 🟡 At Risk   [ ] 🔴 Blocked
- **Đang làm**: Workspace fully operational — 6 production outputs tạo trong 1 session. AIMS Crew Module upgrade package hoàn chỉnh.
- **Sprint/Iteration**: Phase 4 — Real Use And Refinement

---

## ✅ Hoàn thành (session gần nhất)
| Ngày | Task | Ghi chú |
|------|------|---------|
| 2026-04-14 | Tạo lớp identity, user profile, domain context, templates, and skills | `SOUL.md`, `context/`, `skills/` |
| 2026-04-14 | Tạo examples cho 3 skills chính | `skills/*/examples/` |
| 2026-04-14 | Tạo sanitized real examples và redaction policy | `kb/examples-real/` |
| 2026-04-14 | Init bộ `memory-bank/` và project session rules | `memory-bank/`, `CLAUDE.md`, `AGENTS_PROJECT.md` |
| 2026-04-14 | Copy first-pass content vào 5 file memory-bank chính | `memory-bank/*.md` |
| 2026-04-14 | ✨ Tạo SOP thật đầu tiên: AIMS User Access Creation & Management | `docs/output/SOP-AIMS-User-Access-Creation-and-Management.md` |
| 2026-04-14 | ✨ Tạo Fit-Gap Assessment: AIMS Crew Management Module (12 gaps, 5 areas) | `docs/output/FitGap-AIMS-Crew-Management-Module.md` |
| 2026-04-14 | ✨ Tạo Vendor Question Pack: 18 questions từ Fit-Gap (6 topics, priority matrix, email template) | `docs/output/Vendor-Question-Pack-AIMS-Crew-Module-Gaps.md` |
| 2026-04-14 | ✨ Tạo Executive Memo: Crew Module Upgrade recommendation cho management | `docs/output/Executive-Memo-AIMS-Crew-Module-Upgrade.md` |
| 2026-04-14 | ✨ Tạo Weekly Status Report: AIMS Crew Module (progress, blockers, actions) | `docs/output/Weekly-Status-AIMS-Crew-Module.md` |
| 2026-04-14 | ✨ Tạo Project Plan: 14-week, 6-phase implementation plan | `docs/output/Project-Plan-AIMS-Crew-Module-Upgrade.md` |

---

## 🔄 Đang làm dở (Work In Progress)
| Task | Tiến độ | File chính | Ghi chú |
|------|---------|-----------|---------|
| Bắt đầu dùng workspace cho use case thật | 100% ✅ | `docs/output/` | SOP AIMS User Access — use case thật đầu tiên hoàn thành |
| Chuyển workspace từ template sang live operating system | 90% | `memory-bank/`, `README_HAU_WORKSPACE.md` | Đã dùng thật, cần thêm cases để tinh chỉnh |

---

## 🔴 Blockers (Đang bị chặn)
| Vấn đề | Nguyên nhân | Kế hoạch giải quyết | Owner |
|--------|-------------|---------------------|-------|

*None — Không có blocker*

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
1. 🔥 **Push toàn bộ changes lên GitHub** — Ước tính: 5m
2. 📌 **Tạo thêm output: vendor question hoặc executive memo** — Ước tính: 30m — `docs/output/`
3. 📌 **Bổ sung sanitized versions vào kb/examples-real/** — Ước tính: 30m — `kb/examples-real/`
4. 💡 **Tạo decision entry trong decisions-log.md** — Ước tính: 15m — `memory-bank/decisions-log.md`

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
