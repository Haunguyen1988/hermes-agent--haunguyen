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
