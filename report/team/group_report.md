# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: 4ChangLinhNguLam
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): 
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

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

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

Chưa thay đổi Problem Statement vì chưa có dữ liệu thực tế. Nhóm giữ nguyên phạm vi ban đầu nhưng sẽ xem xét thu hẹp nếu phỏng vấn cho thấy thời gian tìm kiếm hoặc tần suất phát sinh rework thấp hơn ước tính.

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
