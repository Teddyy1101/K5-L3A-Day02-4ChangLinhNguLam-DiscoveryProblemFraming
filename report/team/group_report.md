# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: 4TrangLinhNguLam
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi khách yêu cầu đổi một logic đã chốt từ 3–4 tháng trước, team (2 BA/PO + 3 dev) không tìm lại được lý do và ràng buộc ngầm của quyết định cũ, nên mất ~40 phút lục Slack/doc/git và vẫn có nguy cơ sửa sai gây hồi quy hoặc mâu thuẫn cam kết.
- Quyết định cuối: *(điền ở CP6)*

---

## 2. Hội tụ nhóm (CP3)

Nhóm 3 người, mỗi người pitch top 3 → **9 candidate**. Phần pitch và phản biện làm trực tiếp, không dùng AI.

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Khuất Duy Hiếu | Khi khách đổi một logic cũ, tôi muốn biết chắc lý do & ràng buộc ngầm của quyết định ban đầu, để không sửa sai gây lỗi/mâu thuẫn cam kết | 2 BA/PO, 3 dev | Bước 3 lục Slack/doc/git blame (~25') + bước 4 BA và dev hỏi nhau nhớ lại (~15') | "Lần gần nhất đổi logic cũ mà vỡ ràng buộc là khi nào, hậu quả mất bao lâu?" (Thứ) · "Nếu chỉ thêm mục *Lý do* vào template ticket thì giải được bao nhiêu phần?" (Đức) |
| 2 | Khuất Duy Hiếu | Khi chuyển nội dung họp với khách thành task, tôi muốn BA/PO và dev chốt chung một cách hiểu, để code không lệch ý | 2 BA/PO, 3 dev | BA tóm tắt thủ công (20') + dev tua lại record (25') | "Lệch ý do tóm tắt thiếu hay do trong họp chưa hỏi edge case?" (Đức) |
| 3 | Khuất Duy Hiếu | Khi đọc spec/comment tiếng Nhật, tôi muốn hiểu đúng thuật ngữ nghiệp vụ, để không code sai do dịch máy | 3 dev, 2 BA/PO | Tự đoán thuật ngữ (8') + chờ BA xác nhận (10–15') | "Một bảng Glossary dùng chung đã giải được bao nhiêu % trường hợp?" (Thứ) |
| 4 | Nguyễn Huy Thứ | Khi chuẩn bị nộp bài lab, tôi muốn kiểm tra code/README/báo cáo/file đính kèm đã đủ yêu cầu chưa, để không mất điểm | Sinh viên làm lab lập trình | Bước đối chiếu từng yêu cầu với nhiều loại file (15–30', chưa đo) | "Lần gần nhất bạn bị trừ điểm vì thiếu file là khi nào? Một script kiểm tên file/thư mục đã đủ chưa?" (Hiếu) |
| 5 | Nguyễn Huy Thứ | Khi deadline/lịch học đổi qua nhiều kênh, tôi muốn phát hiện thay đổi, để cập nhật lịch kịp thời | Sinh viên học nhiều môn | Kiểm tra LMS, email, Zalo, Messenger và so sánh thủ công (10–20'/ngày) | "Học kỳ này bạn thực sự bỏ lỡ bao nhiêu deadline vì đổi lịch?" (Đức) |
| 6 | Nguyễn Huy Thứ | Khi nhân viên mới vào công ty, tôi muốn biết thủ tục nào xong/còn thiếu/đang chờ ai, để bắt đầu đúng hạn | Nhân viên mới, HR, IT, quản lý | Thông tin tiến độ rải rác giữa HR/IT, phải nhắn hỏi | "Nhóm có ai đang trực tiếp làm onboarding để kiểm chứng không?" (Hiếu) |
| 7 | Nguyễn Ngọc Minh Đức | Khi chuẩn bị nộp bài, tôi muốn đối chiếu bài với toàn bộ yêu cầu của đề, để tránh thiếu nội dung/sai cách nộp | Sinh viên phụ trách nộp bài | Đối chiếu từng yêu cầu với bài làm (~10'/lần, dễ bỏ sót) | "Khó ở chỗ hiểu đề hay ở chỗ đối chiếu? Checklist + kiểm tra chéo có đủ không?" (Thứ) |
| 8 | Nguyễn Ngọc Minh Đức | Khi bắt đầu làm bài, tôi muốn tìm đúng yêu cầu và tài liệu mới nhất, để không dùng thông tin cũ | Sinh viên | Tìm qua nhiều kênh, xác nhận bản mới nhất (10–15'/lần) | "Gom tất cả về một thư mục chung đã giải quyết được chưa?" (Hiếu) |
| 9 | Nguyễn Ngọc Minh Đức | Khi theo dõi bài nhóm trước hạn, nhóm trưởng muốn biết phần nào xong/đang kẹt, để hỗ trợ kịp | Nhóm trưởng, thành viên | Hỏi từng thành viên và chờ phản hồi (30'–1h/lần tổng hợp) | "Vấn đề là thiếu công cụ hay thành viên không chủ động cập nhật?" (Hiếu) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Mất / lệch ngữ cảnh yêu cầu | #1 lý do logic cũ, #2 lệch ý sau họp, #3 thuật ngữ tiếng Nhật | Yêu cầu đi qua nhiều người/nhiều thời điểm, phần **"vì sao" và "nghĩa đúng"** bị rơi → làm sai rồi phải sửa |
| B — Kiểm tra trước khi nộp | #4 kiểm bài lab (Thứ), #7 đối chiếu đề (Đức) | Trùng nhau: đối chiếu thủ công sản phẩm với danh sách yêu cầu, dễ bỏ sót |
| C — Thông tin rải rác nhiều kênh | #5 deadline đổi, #8 tìm tài liệu mới nhất | Phải lục nhiều nguồn để biết bản nào là mới/đúng |
| D — Theo dõi tiến độ phối hợp | #6 onboarding, #9 tiến độ nhóm | Trạng thái công việc nằm ở người khác, phải hỏi đi hỏi lại |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm số lần phải làm lại (rework / sửa / nộp lại) do thiếu hoặc hiểu sai thông tin yêu cầu
├── Opportunity A: Khi đổi một logic cũ, không ai còn nhớ lý do và ràng buộc ban đầu
│     ├── Lý do quyết định không được ghi lại lúc chốt (chỉ ghi "What", không ghi "Why")
│     └── Ngữ cảnh cũ nằm rải rác ở Slack, biên bản họp, commit — tìm lâu và không chắc đủ
├── Opportunity A': Sau họp với khách, BA/PO và dev hiểu yêu cầu khác nhau
├── Opportunity B: Trước khi nộp, đối chiếu sản phẩm với từng yêu cầu dễ bỏ sót
├── Opportunity C: Không chắc thông tin/deadline mình đang dùng là bản mới nhất
└── Opportunity D: Không biết việc của người khác đang ở trạng thái nào nếu không hỏi

     ✗ "Chatbot hỏi đáp lịch sử dự án"       ← solution, gạch khỏi tầng này
     ✗ "Script/checker tự động kiểm bài lab"  ← solution, gạch khỏi tầng này
     ✗ "Bot gom thông báo từ LMS/Zalo/email"  ← solution, gạch khỏi tầng này
     ✗ "Dashboard tiến độ onboarding"         ← solution, gạch khỏi tầng này
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Chatbot hỏi đáp lịch sử dự án" — xuất hiện khi bàn #1; đây là cách giải, pain thật là *không tìm lại được lý do quyết định*.
- "Script kiểm tra bài lab tự động" — xuất hiện ở #4/#7; pain thật là *đối chiếu thủ công dễ sót*.
- "Bot gom thông báo đa kênh" (#5) và "Dashboard tiến độ" (#6, #9) — đều là công cụ, không phải nhu cầu.
- Câu "thiếu bảng Glossary" ở #3 cũng được viết lại thành pain: *dev hiểu sai thuật ngữ nghiệp vụ*.

### 2.4. Chấm điểm shortlist (1–5)

Shortlist 3 candidate (B gộp #4 và #7 vì trùng pattern):

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1 Mất lý do & ràng buộc ngầm khi đổi logic cũ (Hiếu) | 4 | 4 | 3 | 4 | 4 | 5 | 3 | **27** |
| B: Kiểm tra bài trước khi nộp (#4 Thứ + #7 Đức) | 4 | 5 | 2 | 3 | 5 | 3 | 5 | **27** |
| #2 Lệch ý sau họp với khách (Hiếu) | 4 | 5 | 3 | 3 | 4 | 4 | 3 | 26 |

Ghi chú chấm:
- **#1 – So sánh 4 mức = 5:** cả 4 mức đều có phương án thật và khác nhau rõ: No AI (template bắt buộc ghi *Lý do & Ràng buộc*), Rule (chặn đóng ticket nếu trống mục lý do), Workflow (AI nháp lý do từ thread Slack/biên bản lúc chốt, người xác nhận), Agent (tự lục lịch sử cũ). Đây là bài tốt nhất để luyện quyết định mức can thiệp.
- **#1 – Pain bằng chứng = 3:** có ước tính từ trải nghiệm thật (~40' tra cứu, 1–2 lần/tháng) nhưng **chưa có số lần rework** trong 6–12 tháng qua → đưa vào CP4.
- **B – Pain bằng chứng = 2:** cả hai người đều chỉ có số ước lượng cá nhân (10' và 15–30'), chưa ai kể được lần bị trừ điểm cụ thể. **So sánh 4 mức = 3:** phần lớn (tên file, thư mục, file bắt buộc) giải bằng Rule/script; chính AI phản biện ở CP2 của Thứ cũng chỉ ra điều này.
- **#2 – Impact = 3:** tần suất thấp (1 task / 1–2 sprint) và chưa rõ gốc lệch ý nằm ở tóm tắt hay ở cuộc họp.

**Candidate được chọn:** #1 — Mất lý do & ràng buộc ngầm khi đổi logic cũ (problem #1 của Khuất Duy Hiếu).

**Vì sao chọn:**
- Hòa điểm với B nhưng nhóm chọn #1 vì **hậu quả nặng hơn**: không chỉ mất thời gian mà còn rủi ro bug hồi quy và mâu thuẫn với cam kết với khách — đúng outcome "giảm làm lại" ở gốc cây OST.
- Có actor thật (team 5 người: 2 BA/PO + 3 dev) và có người trong nhóm làm việc trực tiếp trong quy trình → phỏng vấn được người thật ở CP4 (BA/PO và dev trong team của Hiếu, không phải thành viên nhóm lab).
- Phương án No AI rất mạnh (template ghi lý do) → buộc nhóm phải trả lời nghiêm túc "có cần AI không", phù hợp mục tiêu lab.

**Vì sao loại các candidate còn lại:**
- **B (kiểm tra bài trước khi nộp):** quy trình rõ nhưng pain yếu (chưa có lần mất điểm cụ thể, 10–30'/lần) và phần lớn giải được bằng checklist + script, khó so sánh có ý nghĩa giữa 4 mức. Giữ lại làm phương án dự phòng nếu CP4 bác bỏ #1.
- **#2 (lệch ý sau họp):** cùng cluster A với #1 nhưng tần suất thấp hơn và chưa rõ gốc rễ; nhóm nhận thấy #2 thực chất là *phiên bản tức thời* của #1 (ghi lại "cái gì đã chốt và vì sao") → bài học từ #1 có thể áp dụng lại.
- **#3 (thuật ngữ tiếng Nhật):** một Glossary dùng chung có thể giải phần lớn → nghiêng mạnh về No AI/Rule.
- **#5, #8 (thông tin rải rác):** phụ thuộc truy cập nhiều nền tảng (Zalo, Messenger), khó vừa sức lab.
- **#6, #9 (theo dõi tiến độ):** #6 không ai trong nhóm làm onboarding thật để kiểm chứng; #9 gốc rễ có vẻ là hành vi (không chủ động cập nhật) hơn là thiếu thông tin.

**Xử lý bất đồng (nếu có):** Thứ và Đức ban đầu muốn chọn B vì cả hai đều tự đưa ra (trùng nhau) và dễ làm prototype. Nhóm thống nhất: B dễ nhưng "dễ" chủ yếu vì có thể giải bằng script, không cần quyết định mức can thiệp AI; #1 có rủi ro thật hơn. Điều kiện kèm theo: nếu ở CP4 phỏng vấn không ra được ít nhất 1 lần rework cụ thể do vỡ ràng buộc logic cũ thì nhóm quay về B.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | BA/PO và Dev thường mất nhiều thời gian tìm lại lý do của logic cũ. | Value | 5 | 1 | Có |
| 2 | Lý do và ràng buộc cũ thường nằm rải rác trong Slack, Jira, Notion và Git. | Value | 5 | 1 | Có |
| 3 | Thiếu ngữ cảnh từng khiến team phải đoán, sửa lại hoặc phát sinh bug. | Value | 5 | 1 | Có |
| 4 | Có thể truy cập và kết nối dữ liệu từ các công cụ đang sử dụng. | Feasibility | 4 | 1 | Có |
| 5 | AI có thể tổng hợp đúng lý do quyết định và dẫn nguồn gốc để kiểm chứng. | Feasibility | 5 | 1 | Có |
| 6 | Công ty cho phép sử dụng AI với dữ liệu nội bộ của dự án. | Viability | 5 | 1 | Có |

**Giả định nhóm kiểm chứng trong buổi này:**

- Thời gian thực tế để tìm lại quyết định cũ có gần 40 phút không?
- Thiếu ngữ cảnh có thực sự gây bug hoặc rework không?
- Các công cụ hiện tại có đủ khả năng tìm lại thông tin không?
- AI có thể tổng hợp chính xác và trích dẫn nguồn không?

### 3.2. Kiểm chứng

**Cách đã dùng:** Chưa có kết quả phỏng vấn thực tế. Dự kiến phỏng vấn 2 BA/PO và 3 Dev không thuộc nhóm thực hiện bài tập; kết hợp kiểm tra ticket, Slack, tài liệu và lịch sử Git nếu được phép.

**Interview snapshot:**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | BA/PO hoặc Dev – chờ phỏng vấn |
| Câu nói đáng nhớ nhất (nguyên văn) | Chưa có dữ liệu |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chờ người được hỏi mô tả tình huống thực tế |
| Hiện đang xử lý bằng cách nào (workaround)? | Dự kiến kiểm tra Slack, Jira, Notion, Git và hỏi đồng nghiệp |
| Mất bao lâu, bao lần? | Chưa đo; cần ghi nhận thời gian và tần suất thực tế |
| Insight / opportunity rút ra | Chưa kết luận trước khi có phỏng vấn |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn BA/PO | 0/2 | Chưa có | Chưa có |
| Phỏng vấn Dev | 0/3 | Chưa có | Chưa có |
| Ticket, Slack, Git, biên bản họp | 0 mẫu | Chưa kiểm tra | Chưa kiểm tra |

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Jira + Confluence Decision Log | [Atlassian Decision Template](https://www.atlassian.com/software/confluence/templates/decision/) | Lưu lý do, người quyết định, phương án và kết quả tại thời điểm chốt. | Có cấu trúc lưu trữ quyết định, dễ tra cứu lại. | Phụ thuộc vào việc BA/PO hoặc Dev chủ động ghi chép đầy đủ. | Ưu tiên chuẩn hóa cách ghi nhận quyết định trước. |
| Atlassian Rovo | [Rovo Documentation](https://support.atlassian.com/rovo/docs/what-is-rovo/) | Tìm kiếm thông tin trên Jira, Confluence và các nguồn đã kết nối như Slack. | Tìm kiếm ngữ nghĩa trên nhiều nguồn, có thể trả lời dựa trên dữ liệu nội bộ theo quyền truy cập. | Phụ thuộc kết nối, quyền truy cập và chất lượng dữ liệu; câu trả lời AI vẫn cần kiểm chứng. | Cần thử công cụ có sẵn trước khi tự xây hệ thống tìm kiếm. |
| Slack AI | [Slack AI Features](https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack) | Tìm kiếm, tóm tắt thread và hội thoại cũ trong Slack. | Giúp nhanh chóng nắm lại nội dung trao đổi và ngữ cảnh hội thoại. | Chủ yếu hỗ trợ dữ liệu Slack; không tự giải quyết việc tìm quyết định trên Jira hoặc Git. Tính năng tùy gói dịch vụ. | Có thể tận dụng để tìm lại trao đổi nhưng vẫn cần đối chiếu nguồn khác. |

**Kết luận Research:**

- Không nên xây hệ thống mới ngay khi chưa thử công cụ hiện có.
- Ưu tiên kiểm tra Jira/Confluence Decision Log và khả năng tìm kiếm bằng Rovo hoặc Slack AI.
- Nếu vẫn thiếu khả năng tổng hợp lý do từ nhiều nguồn, nhóm mới thử nghiệm AI hỗ trợ, bắt buộc dẫn nguồn để BA/PO xác nhận.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
