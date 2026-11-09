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
---

## 6. Mức can thiệp AI (CP6)

> **Trạng thái:** Bản đề xuất để nhóm rà soát và tự chốt. CP4 hiện có 0 cuộc phỏng vấn, 0 mẫu tài liệu được kiểm tra; CP5 chưa có quy trình chi tiết và Problem Statement v0. Vì vậy, các mục dưới đây phân biệt dữ liệu đang có, giả thuyết và ngưỡng thử nghiệm đề xuất; chưa phải kết quả kiểm chứng.

### 6.1. Ma trận độ mơ hồ × độ phức tạp

| Độ phức tạp | Độ mơ hồ thấp | Độ mơ hồ cao |
|---|---|---|
| **Độ phức tạp thấp** | Kiểm tra ticket có đủ trường bắt buộc hay không: Rule có thể đủ. | Tóm tắt một gói nguồn đã được người chọn: có thể thử Workflow. |
| **Độ phức tạp cao** | Đối chiếu nhiều nguồn theo danh sách và quy tắc rõ. | **Bài toán đầy đủ của nhóm:** tìm và xác minh lý do/ràng buộc của logic cũ từ nhiều nguồn. |

**Bài toán đầy đủ nằm ở ô mơ hồ cao × phức tạp cao, theo mô tả ban đầu ở CP2–CP3:**

- **Mơ hồ cao:** lý do nằm trong ngôn ngữ tự nhiên, có thể là đề xuất chưa chốt, quyết định đã chốt hoặc nội dung đã bị thay thế; cần hiểu bối cảnh. Có nhiều cách tóm tắt chấp nhận được, nhưng sự kiện lịch sử vẫn phải có nguồn chứng minh.
- **Phức tạp cao:** cần nối ticket/spec với Slack, biên bản và Git; bước xác minh ràng buộc phụ thuộc kết quả tìm nguồn. Quyền truy cập và mức đầy đủ của các nguồn này chưa được kiểm chứng.
- Vị trí trên ma trận **không tự động dẫn đến chọn Agent**. Trước hết cần kiểm tra nguyên nhân: thông tin **đã ghi nhưng rải rác**, hay lý do **chưa từng được ghi**. Trường hợp thứ hai cần người có trách nhiệm xác nhận; AI không thể khôi phục một lý do chưa có trong dữ liệu thành sự thật lịch sử.

**Thu hẹp vòng kiểm chứng đầu:** một dự án, một loại yêu cầu đổi logic, dùng Decision Log do BA/PO và dev đối chiếu thủ công. Đồng thời ghi lý do/ràng buộc ngay khi chốt quyết định mới. Chưa mở bài toán tìm kiếm tự động trên toàn bộ lịch sử dự án.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | BA/PO ghi Decision Log gắn với ticket: quyết định, lý do, ràng buộc, nguồn, thời điểm/phiên bản, người xác nhận, trạng thái. Với quyết định cũ, BA/PO và dev lập chỉ mục từ nguồn còn tồn tại; ghi rõ phần chưa biết. | Người dùng tìm đúng ngữ cảnh đủ nhanh và không bỏ sót ràng buộc quan trọng; chi phí ghi/duyệt chấp nhận được. Chưa có kết quả thử. | Không phục hồi được lý do chưa từng ghi; có thể bỏ qua template hoặc mất công bổ sung lịch sử. | **Chọn để kiểm chứng trước.** |
| **Rule** | Kiểm tra các trường bắt buộc và trạng thái duyệt trước khi chuyển ticket sang bước tiếp theo; nhắc bổ sung nếu thiếu. | Đã có template hữu ích, nhưng dữ liệu thử cho thấy lỗi chính là quên điền hoặc thiếu trường. | Có thể điền cho đủ hình thức; Rule không đánh giá được lý do đúng hay ràng buộc đủ chưa. Chưa xác nhận khả năng cấu hình công cụ. | Chưa chọn; chỉ thêm nếu có bằng chứng cần. |
| **Workflow** | Các bước cố định: người có quyền chọn gói nguồn cho một ticket → AI nháp lý do/ràng buộc kèm nguồn → BA/PO xác minh → dev đối chiếu ảnh hưởng → người lưu bản đã duyệt. | No AI/Rule vẫn không đạt metric vì việc đọc và tổng hợp **nguồn đã tồn tại** còn tốn thời gian; có dữ liệu, quyền sử dụng và bộ eval. | Bịa lý do, bỏ sót ràng buộc, dùng quyết định lỗi thời; thời gian kiểm tra có thể lớn hơn thời gian tiết kiệm. | Hướng thử tiếp theo có điều kiện. |
| **Agent** | AI tự chọn nơi tìm, công cụ, truy vấn và bước tiếp theo để lần theo lịch sử quyết định. | Có bằng chứng Workflow cố định không đủ và thực sự cần AI tự quyết đường tìm kiếm. | Khó kiểm soát phạm vi, chi phí và khả năng kết luận sai từ lịch sử thiếu/mâu thuẫn. | Chưa chọn; chưa chứng minh cần vượt Workflow. |

**Mức chọn hiện tại: No AI, cho vòng kiểm chứng nhỏ.** Đây là lựa chọn thiết kế tạm thời; quyết định triển khai chính thức vẫn là **Not Yet** ở mục 8.

**Vì sao không chọn mức đơn giản hơn:** No AI là mức thấp nhất trong bốn mức. Khác với giữ nguyên cách làm hiện tại, phương án này gắn trách nhiệm ghi nhận và xác nhận lý do với từng quyết định để kiểm tra trực tiếp giả thuyết gốc: thiếu ghi chép có cấu trúc có phải nguyên nhân chính không?

**Vì sao chưa nâng mức:** chưa có bằng chứng template thủ công thất bại, chưa đo phần việc Rule có thể giải quyết và chưa kiểm tra chất lượng nguồn cho AI. Không thể kết luận No AI giải được 70–80% trường hợp, cũng chưa thể kết luận Workflow là mức tối thiểu. Ưu tiên ghi nhận quyết định có cấu trúc phù hợp với pattern trong [Atlassian Decision documentation template](https://www.atlassian.com/software/confluence/templates/decision/); mức phù hợp với team phải được thử riêng.

### 6.3. AI Canvas rút gọn

**Không áp dụng cho mức No AI đang chọn**, theo ngoại lệ tại [worksheet CP6](../../docs/01-worksheet.md#nếu-nhóm-chọn-no-ai-hoặc-rule). Chưa có bước AI dự đoán hay tạo nội dung; BA/PO và dev đọc nguồn, ghi nhận và xác minh quyết định. Việc thêm AI chỉ được cân nhắc khi có bằng chứng bước tổng hợp thủ công vẫn là bottleneck sau khi đã thử cách đơn giản hơn.

### 6.4. Hai câu hỏi của Google PAIR

**Không bắt buộc áp dụng với No AI.** Hiện chưa có phỏng vấn để khẳng định người dùng muốn augment hay automate.

Nếu đủ điều kiện thử Workflow sau này, **giả thuyết thiết kế** là augment: AI chỉ nháp, BA/PO xác nhận nghiệp vụ, dev xác nhận ảnh hưởng kỹ thuật. Với nhiệm vụ phát hiện ràng buộc ảnh hưởng đến thay đổi, **bỏ sót** có thể gây hồi quy hoặc vi phạm cam kết; **báo nhầm** làm tăng công kiểm tra. Đây là đánh giá rủi ro ban đầu cần kiểm chứng, không phải kết quả phỏng vấn. Bịa lý do lịch sử là lỗi không được chấp nhận; thiếu hoặc mâu thuẫn nguồn phải chuyển người xác minh.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

### 7.1. Problem Statement v1 — bản đề xuất

**Phát biểu bài toán:** Khi khách yêu cầu thay đổi một logic cũ, BA/PO và dev cần tìm lại được lý do, ràng buộc và trạng thái hiệu lực của quyết định trước khi chốt cách sửa. Hiện thông tin được mô tả là rải rác hoặc thiếu phần lý do, khiến bước tra cứu/xác minh mất khoảng 40 phút theo ước tính cá nhân và có nguy cơ bỏ sót ràng buộc. Nhóm đề xuất kiểm chứng Decision Log và đối chiếu nguồn thủ công trước khi quyết định có cần AI hay không.

| Trường | Nội dung |
|---|---|
| **Actor** | Team làm việc được mô tả trong Card #1 của Hiếu: 2 BA/PO và 3 dev. Mỗi yêu cầu cần BA/PO phụ trách nghiệp vụ và dev phụ trách phần bị ảnh hưởng xác nhận. |
| **Quy trình** | Nhận yêu cầu đổi → đọc ticket/spec → tìm Decision Log và nguồn gốc → BA/PO cùng dev kiểm tra lý do, ràng buộc, phiên bản → ghi kết luận đã xác nhận hoặc đánh dấu chưa đủ bằng chứng → mới chốt phương án sửa và kiểm tra hồi quy. Quyết định mới được ghi vào log ngay khi chốt. |
| **Bottleneck** | Bước tìm lại lịch sử khoảng 25 phút và trao đổi xác minh khoảng 15 phút; tổng khoảng 40 phút/lần, **ước tính từ CP2, chưa đo ở CP4**. Không gộp thời gian code/test vào metric tra cứu. |
| **Impact** | Tần suất ước tính 1–2 lần/tháng; có thể chậm chốt phương án và phải làm lại khi hiểu sai ràng buộc. Chưa có số bug, số lần rework hoặc chi phí thiệt hại được xác minh. |
| **Success Metric** (baseline → target, cách đo) | Metric chất lượng chính, thời gian phụ và cách đo được định nghĩa ở mục 7.2. Baseline thực đo chưa có; các target là ngưỡng đề xuất để thử nghiệm, chưa phải kết quả đã đạt. |
| **Boundary** | Chỉ dùng tài liệu người thực hiện có quyền truy cập. Mỗi khẳng định về lịch sử phải dẫn nguồn; phân biệt quyết định cũ với xác nhận mới. Thiếu nguồn, nguồn mâu thuẫn hoặc thiếu người có thẩm quyền xác nhận thì ghi “chưa đủ bằng chứng”, chuyển BA/PO xử lý và chưa chốt thay đổi. Dev vẫn review ảnh hưởng và kiểm tra hồi quy. |
| **AI intervention point** | **Không có trong vòng kiểm chứng đang chọn.** Chưa chứng minh lợi ích tăng thêm của AI so với template và đối chiếu thủ công. |
| **Mức chọn** | **No AI** — Decision Log, checklist và người kiểm tra. Rule/Workflow chỉ được xem xét sau khi có dữ liệu cho thấy mức dưới chưa đủ. |
| **Rủi ro & người kiểm tra** | Lý do ghi lại có thể sai, thiếu ràng buộc hoặc đã lỗi thời: BA/PO xác minh nghiệp vụ, dev đối chiếu kỹ thuật. Người quyết định ban đầu được hỏi lại nếu cần; nếu không liên hệ được thì giữ trạng thái chưa xác minh. Người quản lý dự án xác nhận phạm vi dữ liệu và người duy trì log trước khi thử với dữ liệu nội bộ. Đây là phân công đề xuất theo vai trò, chưa phải cam kết đã nhận. |

### 7.2. Success Metric và cách đo

| Chỉ số | Baseline hiện có | Target đề xuất | Cách đo |
|---|---|---|---|
| **Chính — bug/rework do bỏ sót hoặc hiểu sai ràng buộc cũ** | Chưa biết; cần rà ticket và phỏng vấn về 6–12 tháng gần nhất. Chưa được coi là 0. | Hướng tới 0 ca/quý sau khi áp dụng; chưa thể xác nhận bằng một thử nghiệm ngắn. | BA/PO và dev cùng xác nhận nguyên nhân từng ca, ghi số yêu cầu đổi logic làm mẫu số. Theo dõi theo quý; không suy diễn từ việc chưa thấy lỗi trong 2 tuần. |
| **Chất lượng trong thử nghiệm — xác minh đúng lý do/ràng buộc** | Chưa có bộ ca chuẩn. | Mọi ca được đánh dấu “đã xác minh” phải có nguồn và không thiếu ràng buộc quan trọng trong bản đối chiếu; ca thiếu/mâu thuẫn nguồn phải được nhận diện. | BA/PO và dev lập bản đối chiếu trước từ tài liệu được phép dùng. Chấm 5 tiêu chí tại mục 7.4; một ca không đạt nếu trượt bất kỳ tiêu chí nào. |
| **Phụ — thời gian tra cứu và xác minh mỗi yêu cầu** | Khoảng 40 phút/lần, là ước tính CP2 cho bước 3–4. | Ít nhất 8/10 ca có đủ nguồn được xác minh đúng trong **dưới 10 phút/ca**. | Bấm giờ từ lúc bắt đầu tìm lý do đến lúc có kết luận xác minh; gồm tìm, đọc, hỏi và sửa log nếu cần, không gồm code/test. Đo thời gian trôi qua, không nhân với cả 5 người. Ca chưa giải được vẫn ghi nhận và không tính đạt tốc độ. |
| **Chi phí duy trì log** | Chưa đo. | Thời gian chủ động ghi và duyệt một quyết định mới không quá 5 phút/ca; báo cáo riêng thời gian bổ sung lịch sử. | Ghi phút làm việc của từng người, gồm soạn và review; cộng thành công sức duy trì. Nếu chưa có quyết định mới trong thời gian thử thì ghi thiếu mẫu, không kết luận đạt. |

**Thiết kế đo đề xuất:** chọn 10 yêu cầu lịch sử có đủ nguồn, kèm ít nhất 2 tình huống thiếu hoặc mâu thuẫn nguồn để kiểm tra cách xử lý. Đo cách cũ trước khi lập log; ghi riêng công sức tạo log và kiểm tra. Khi so sánh, đổi người đọc hoặc dùng ca tương đương để giảm việc nhớ đáp án. Báo cáo kết quả theo từng ca, cỡ mẫu và hạn chế; không coi đây là thử nghiệm chứng minh quan hệ nhân quả. Với tần suất ước tính 1–2 lần/tháng, không kỳ vọng có đủ 10 yêu cầu mới trong 2 tuần.

### 7.3. Đối chiếu với v0 và lý do bổ sung

**Mục 5 hiện chưa có v0**, nên chưa thể báo cáo một thay đổi v0 → v1 đã diễn ra. Bảng sau ghi khoảng trống và nội dung v1 đề xuất; nhóm cần hoàn thành CP5 rồi đối chiếu lại trước khi nộp.

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Success Metric | Chưa lập; CP2 mới có ước tính khoảng 40 phút và mục tiêu dưới 10 phút. | Tách metric chất lượng, tốc độ và công duy trì; thêm mẫu số, cách đo và nhãn “chưa đo”. | Tránh nhanh hơn nhưng xác minh sai, hoặc tiết kiệm thời gian tra cứu bằng cách tăng quá nhiều công ghi chép. |
| Boundary | Chưa lập. | Thiếu/mâu thuẫn nguồn phải đánh dấu; phân biệt bằng chứng lịch sử với xác nhận mới; BA/PO và dev kiểm tra. | Không biến suy đoán thành lý do cũ và không bỏ bước review trước khi sửa logic. |
| AI intervention point, mức chọn | Chưa lập; CP2 còn cân nhắc No AI hoặc Workflow. | Không có bước AI; chọn No AI cho vòng kiểm chứng đầu. | Chưa có bằng chứng phương án đơn giản hơn không đủ. |
| Rủi ro & người kiểm tra | Chưa lập. | Nêu vai trò xác minh nghiệp vụ, kỹ thuật và phạm vi dữ liệu. | Một bản log đầy đủ trường chưa đồng nghĩa đúng hoặc còn hiệu lực. |

### 7.4. Tiêu chí đánh giá giải pháp No AI

Theo [rubric C9–C10](../../RUBRIC.md), khi chọn No AI, eval được viết cho template/checklist và kết quả xác minh của con người.

Ca thiếu/mâu thuẫn nguồn có thể đạt eval nếu được nhận diện đúng và chuyển sang trạng thái chờ xác minh; không phải điền các trường chưa biết cho đủ. Ca đó vẫn **không tính là đã giải quyết đúng trong ngưỡng tốc độ** và chưa được dùng làm căn cứ sửa logic.

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Truy được nguồn, không đoán lý do** | Mỗi lý do/ràng buộc được ghi là sự thật lịch sử có nguồn hỗ trợ trực tiếp. Xác nhận mới được ghi ngày và người có thẩm quyền theo vai trò. | Viết suy đoán như quyết định cũ; có link nhưng nội dung không hỗ trợ kết luận. |
| 2 | **Đủ ràng buộc quan trọng** | Bao phủ toàn bộ ràng buộc được BA/PO và dev đánh dấu quan trọng trong bản đối chiếu, hoặc ghi rõ phần chưa xác minh và dừng chốt thay đổi. | Bỏ sót ràng buộc quan trọng nhưng vẫn ghi “đủ để sửa”. |
| 3 | **Đúng trạng thái và phiên bản** | Ca đã xác minh ghi được thời điểm, quyết định đã chốt/đã bị thay thế và phạm vi áp dụng. Nếu chưa xác định được trạng thái/phiên bản, nêu rõ trường chưa biết và giữ “chờ xác minh”. | Dùng đề xuất chưa chốt hoặc quyết định hết hiệu lực làm căn cứ hiện tại; tự điền phiên bản khi chưa có bằng chứng. |
| 4 | **Xử lý thiếu/mâu thuẫn thông tin** | Chỉ rõ phần chưa biết hoặc nguồn xung đột, chuyển BA/PO xác minh; không tự kết luận hai nguồn đã thống nhất. | Điền cho đủ template, che mất mâu thuẫn hoặc coi không tìm thấy là không có ràng buộc. |
| 5 | **Đúng phạm vi và có người kiểm tra** | Chỉ dùng nguồn được phép. Ca đã xác minh có vai trò/ngày duyệt của BA/PO và dev trước khi chốt cách sửa. Ca chưa xác minh ghi người tiếp nhận theo vai trò và trạng thái chờ, không ghi là đã duyệt. | Dùng nguồn ngoài quyền; chốt cách sửa khi thiếu một bên xác nhận; hoặc lấy log chưa duyệt làm căn cứ sửa. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

Đánh giá dưới đây áp dụng cho **phương án No AI đang đề xuất**, dựa trên dữ liệu hiện có; chưa phải đánh giá sau thử nghiệm.

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Cao** | CP4 có 0 phỏng vấn, chưa có ca rework được xác minh; thời gian và tần suất mới là ước tính từ người đưa ra candidate. Chưa biết lợi ích có bù công ghi/duyệt log không. Cần kiểm tra điều kiện nhóm đã đặt ở CP3: có ít nhất 1 ca rework cụ thể do thiếu ngữ cảnh. |
| **Usability** | Người dùng có dùng được, hiểu và sửa được log không? | **Trung bình** | Template đơn giản nhưng chưa quan sát BA/PO và dev thực hiện; có thể khó phân biệt lý do, ràng buộc, đề xuất và quyết định đã chốt. Thử bằng nhiệm vụ tìm lại ngữ cảnh và đối chiếu nguồn. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Trung bình** | Có thể bắt đầu bằng Markdown/bảng thủ công, chưa cần tích hợp. Tuy nhiên chưa kiểm tra mẫu nguồn; lý do chưa từng được ghi không thể phục hồi bằng log hay AI. Cần kiểm kê khả năng truy cập và mức đầy đủ của tài liệu. |
| **Viability** | Có hợp chi phí, quy định tổ chức không? Ai vận hành? | **Trung bình** | Không cần mua công cụ mới cho vòng thử thủ công, nhưng chưa có người nhận duy trì và chưa xác nhận phạm vi dùng dữ liệu nội bộ. Cần người quản lý đồng ý phạm vi và đo công ghi/duyệt. Nếu dùng AI sau này, phải đánh giá lại chính sách dữ liệu và chi phí. |

### 8.2. Kết luận

**Quyết định đề xuất: Not Yet — chưa triển khai chính thức, chưa đầu tư xây hoặc tích hợp AI.**

**Lý do:** Value đang ở mức Cao vì chưa có kiểm chứng hành vi và hậu quả; chưa có baseline thực đo, CP5 cũng chưa hoàn thành. Đây là các khoảng trống có thể kiểm tra bằng phỏng vấn và một thử nghiệm nhỏ. Chưa chọn Go; cũng chưa đủ bằng chứng kết luận pain không đáng giải để chọn No-Go. No AI là cách kiểm chứng đầu tiên, không phải kết quả đã chứng minh đủ dùng.

**Việc cần làm trước, trong một vòng kiểm chứng tối đa 2 tuần:**

| Việc | Vai trò phụ trách đề xuất | Bằng chứng cần có / điều kiện hoàn thành |
|---|---|---|
| Phỏng vấn 2–3 người thật ngoài nhóm lab, có cả BA/PO và dev; hỏi lần gần nhất đổi logic cũ, nguồn đã tìm, thời gian và hậu quả thực tế. | Người phụ trách kiểm chứng; Hiếu hỗ trợ kết nối nếu phù hợp. | Snapshot ghi vai trò, thời điểm, cách hỏi. Chủ động tìm tín hiệu phản bác như ca tìm nhanh bằng cách cũ hoặc template từng không hữu ích; ghi điều thực sự quan sát được, nếu chưa thấy thì nêu rõ. Xác minh có ít nhất 1 ca rework do thiếu ngữ cảnh theo điều kiện CP3, hoặc ghi rõ điều kiện chưa đạt. |
| Kiểm kê tài liệu và quyền sử dụng trong một dự án. | BA/PO và người quản lý dự án. | Phân biệt “đã ghi nhưng khó tìm” với “chưa từng ghi”; xác nhận phạm vi được dùng. Chỉ ghi bản đã ẩn danh và được phép vào repo. |
| Hoàn thành CP5 trước khi chốt v1. | Nhóm phụ trách quy trình. | Quy trình trước/sau, thời gian từng bước, baseline được gắn nguồn, boundary, phương án quay về và v0; đối chiếu lại mục 7.3. |
| Thử Decision Log/checklist trên các ca lịch sử. | BA/PO lập log; dev đối chiếu; một người ghi số đo. | 10 ca đủ nguồn và ít nhất 2 ca thiếu/mâu thuẫn nguồn nếu được phép tiếp cận; ghi rõ số mẫu thực có, thời gian tạo log, thời gian tra cứu và kết quả 5 tiêu chí. Đây là kế hoạch, hiện có 0 ca đã thử. |

**Nếu đủ điều kiện chuyển Go:** chỉ mở pilot No AI trong một dự án, một loại yêu cầu đổi logic, một cặp BA/PO–dev chịu trách nhiệm. Điều kiện: không rủi ro nào còn Cao; có phạm vi dữ liệu và người duy trì; đạt tiêu chí chất lượng và ngưỡng tốc độ ở mục 7.2. Chưa mở sang toàn công ty và chưa coi pilot ngắn là bằng chứng đã giảm bug theo quý.

**Khi nào cân nhắc mức cao hơn:** nếu log hữu ích nhưng thường thiếu trường do quên điền, thử Rule nhắc/kiểm tra trường trước. Nếu nguồn đã đủ, No AI/Rule vẫn không đạt tốc độ vì đọc/tổng hợp, mới lập thử nghiệm Workflow có nguồn do người chọn, eval riêng và người duyệt. Nếu không có lý do trong nguồn, hỏi người quyết định thay vì tăng mức AI.

**Nếu No AI đã đủ:** giữ template, chỉ mục nguồn và kiểm tra chéo; chọn No-Go đối với việc xây AI cho phạm vi này. Nếu kiểm chứng không tìm được ca rework như điều kiện CP3, nhóm cần xem lại candidate; B là phương án dự phòng đã nêu, không tự chuyển mà bỏ qua kiểm chứng.

**Ngưỡng dừng đề xuất:**

- **Sau 2 tuần**, nếu vẫn chưa có tối thiểu 2 cuộc phỏng vấn hợp lệ hoặc chưa xác minh được ca rework theo điều kiện CP3, giữ Not Yet và xem lại candidate. Nếu thiếu mẫu/quyền dữ liệu, không mở pilot và không diễn giải thiếu dữ liệu thành pain đã bị bác bỏ.
- **Dừng dùng log làm căn cứ ngay ở ca đang xét** khi có một lý do không có nguồn, một ràng buộc quan trọng bị bỏ sót hoặc một quyết định hết hiệu lực được ghi là hiện hành; BA/PO và dev quay về đọc nguồn/hỏi người có trách nhiệm. Ghi lỗi để sửa, chưa mở rộng áp dụng.
- **Sau bộ thử đủ 10 ca có nguồn**, nếu dưới 8/10 ca được xác minh đúng trong dưới 10 phút, không coi No AI đạt mục tiêu tốc độ. Phân loại nguyên nhân trước khi quyết định sửa template, thêm Rule hay thử Workflow.
- Nếu công duy trì vượt 5 phút/ca hoặc công bổ sung lịch sử lấn át lợi ích, thu hẹp loại quyết định cần ghi và đo lại; chưa tăng mức tự động hóa chỉ để bù một quy trình chưa hữu ích. Nếu chưa có mẫu quyết định mới, chỉ báo thiếu dữ liệu cho chỉ số này.

---

## 9. Hạn chế và hướng tiếp theo

## 10. Tài liệu tham khảo


-
