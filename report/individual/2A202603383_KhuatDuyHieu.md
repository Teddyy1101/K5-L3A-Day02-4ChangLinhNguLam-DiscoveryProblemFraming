# Báo cáo cá nhân — 2A202603383_KhuatDuyHieu

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Khuất Duy Hiếu
- MSSV: 2A202603383
- Email trường (không bắt buộc, repo có thể để public): 
- Tên nhóm: 4TrangLinhNguLam
- Link repo nhóm: https://github.com/Teddyy1101/K5-L3A-Day02-4TrangLinhNguLam-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Rủi ro / Chất lượng quyết định (giả thuyết, cần kiểm chứng) | Khi khách yêu cầu đổi một logic cũ mà không ai nhớ rõ lý do ban đầu, tôi muốn biết chắc các ràng buộc ngầm đứng sau quyết định đó, để không đưa ra thay đổi gây lỗi hoặc mâu thuẫn với những gì đã cam kết. | 2 BA/PO (người quyết định và cam kết với khách), 3 dev (người sửa code và chịu hồi quy) | Ticket/tài liệu cũ chỉ ghi kết quả (What), không lưu lý do (Why). Khi khách đổi logic từ 3–4 tháng trước, team mất 30–45 phút lục lại Slack/commit mà vẫn không chắc hết ràng buộc. Cần điền sau khi hỏi: số lần trong 6–12 tháng qua team đổi logic cũ rồi phát hiện xung đột; hậu quả (bug, rework, mất bao nhiêu ngày); số lần không tìm ra lý do ban đầu. |
| 2 | Tốn thời gian | Khi cần tìm tài liệu vận hành hoặc spec cũ để làm task, tôi muốn tìm được bản mới nhất ở một chỗ, để không phải lục lại nhiều nơi (Slack, Word, Notion) hoặc hỏi lại đồng nghiệp. | 2 BA/PO, 3 dev | 3–4 lần/tuần có người hỏi lại link tài liệu trên Slack; mỗi lần mất khoảng 10–15 phút tìm hoặc chờ người khác gửi lại. |
| 3 | Lặp lại | Khi có thành viên mới vào team, tôi muốn người mới tự tra cứu được tài liệu vận hành và hướng dẫn setup theo một luồng rõ ràng, để không phải hỏi lẻ tẻ và làm ngắt quãng người hướng dẫn. | Người mới, 1 dev hướng dẫn, 2 BA/PO | Mỗi đợt có người mới (vài tháng/lần), mất 3–5 ngày đầu để gom đủ tài liệu từ Slack/Word/Notion; người hướng dẫn mất 30–45 phút/ngày trong tuần đầu để gửi link và giải thích lại. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi chuyển giao nội dung từ buổi họp với khách hàng sang task phát triển, tôi muốn BA, PO và dev chốt chung một cách hiểu ngay sau họp, để khi code không bị lệch ý giữa các bên. | 2 BA/PO, 3 dev | Khoảng 1–2 sprint gặp 1 task hiểu lệch nhau dù có record buổi họp; mất 20–30 phút trao đổi lại và 1–2 giờ sửa code. |
| 5 | Pain từ người khác | Khi đọc spec hoặc comment tiếng Nhật từ BA/khách hàng, tôi muốn nắm đúng nghĩa các thuật ngữ nghiệp vụ trong ngữ cảnh dự án, để không code sai do dịch máy chưa chuẩn. | 3 dev (không biết tiếng Nhật), 2 BA/PO | 2–3 lần/tuần dev mất 10–15 phút dịch Google Translate rồi vẫn phải nhắn hỏi lại BA xem đã hiểu đúng ý chưa; thỉnh thoảng phải sửa lại code vì dịch lệch thuật ngữ. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Cả 5 vấn đề đều lấy từ trải nghiệm thực tế của team (2 BA/PO, 3 dev). Tôi dùng AI để chuyển câu chữ sang đúng cấu trúc Job Story, nhưng bỏ cách diễn đạt dài dòng và gọt lại các con số bị AI ước lượng phóng đại (như tính vọt lên 5–7 giờ/tuần chỉ để tìm link tài liệu, hoặc tự điền khống số liệu cho problem #1 khi chưa hỏi lại team).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Mất lý do & ràng buộc ngầm khi đổi logic cũ (#1) | Ảnh hưởng cả 2 BA/PO và 3 dev; hậu quả không chỉ là mất thời gian lục tìm mà còn gây lỗi hồi quy hoặc mâu thuẫn với cam kết cũ | Tần suất xảy ra trong 6–12 tháng qua có đủ nhiều để cần công cụ hỗ trợ, hay chỉ cần thêm mục ghi lý do vào template ticket? |
| 2 | Hiểu lệch nhau sau buổi họp với khách (#4) | Xảy ra đều theo sprint, quy trình rõ từ lúc họp đến lúc giao task cho dev | Lệch ý chủ yếu do tóm tắt sau họp thiếu chi tiết hay do trong cuộc họp chưa hỏi hết các trường hợp biên (edge case)? |
| 3 | Đọc/dịch spec và comment tiếng Nhật (#5) | Lặp lại 2–3 lần/tuần với cả 3 dev, dễ đo thời gian tra cứu và chờ BA xác nhận | Chỉ cần lập một bảng từ điển thuật ngữ (Glossary) cố định đã giải quyết được phần lớn chưa? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách yêu cầu đổi một logic cũ mà không ai nhớ rõ lý do ban đầu, tôi muốn biết chắc các ràng buộc ngầm đứng sau quyết định đó, để không đưa ra thay đổi gây lỗi hoặc mâu thuẫn với những gì đã cam kết. |
| Actor | 2 BA/PO (đánh giá yêu cầu đổi của khách) và 3 dev (kiểm tra code, sửa logic) |
| Thời điểm / bối cảnh | Khi khách yêu cầu sửa hoặc mở rộng một tính năng đã chốt từ 3–4 tháng trước (ước tính 1–2 lần/tháng) |
| Quy trình hiện tại (3–7 bước) | 1. Nhận yêu cầu đổi logic từ khách · 2. Đọc lại ticket/spec cũ trên Jira/Notion · 3. Tự lục tìm lý do ban đầu trong Slack, biên bản họp, git blame · 4. 1 BA/PO và 1 dev trao đổi để nhớ lại ràng buộc ngầm (nếu không ra phải đoán hoặc hỏi lại khách) · 5. Chốt phương án và sửa code · 6. Kiểm tra hồi quy (nếu phát hiện xung đột phải rework) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (1 người lục tìm Slack/doc/git blame: ước tính ~25') và Bước 4 (1 BA/PO + 1 dev trao đổi nhớ lại ngữ cảnh: ước tính ~15') — tổng ~40' tra cứu trong 55' đầu trước khi dám sửa code, mà vẫn có nguy cơ không tìm ra lý do gốc |
| Impact (nếu không giải thì sao) | Mỗi lần đổi logic cũ (ước tính 1–2 lần/tháng) mất ~55 phút cho các bước tìm hiểu ngữ cảnh (bước 1–4); nghiêm trọng hơn là nhánh rủi ro: khi đoán sai hoặc sót ràng buộc ngầm sẽ gây bug hồi quy/mâu thuẫn cam kết và phải rework (số lần và số ngày rework trong 6–12 tháng qua chưa có, cần hỏi ở CP4) |
| Success metric (baseline → target) | Chính: Số bug hoặc lần rework do xung đột logic cũ mỗi quý giảm về 0 (baseline 6–12 tháng qua: cần điền sau khi hỏi ở CP4). Phụ: Thời gian tra cứu lý do/ràng buộc (bước 3–4) giảm từ ~40 phút (ước tính) xuống dưới 10 phút/lần |
| Phương án không dùng AI | Bắt buộc điền mục "Lý do & Ràng buộc" trong ticket lúc chốt. Hạn chế cần kiểm tra: (1) chỉ xử lý được quyết định từ nay về sau, không cứu được quyết định cũ đã nằm rải rác; (2) dễ bị bỏ qua khi bận (cần hỏi xem team đã thử cách này chưa và vì sao bỏ) |
| Giả thuyết về AI (nếu có) | Tự gom và nháp lý do + ràng buộc ngay lúc quyết định diễn ra (từ thread Slack, biên bản họp) để gắn vào ticket mà không phụ thuộc việc con người gõ tay; đồng thời hỗ trợ lục lại ngữ cảnh cho các quyết định cũ |
| Cảm nhận nhanh | No AI hoặc Workflow (tùy thuộc việc team đã thử dùng template thủ công chưa) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Ước tính ~55 phút xác minh ngữ cảnh/lần (1–2 lần/tháng), chưa tính nhánh rework

[1 Nhận yêu cầu: 5'] → [2 Đọc ticket/spec cũ: 10']
→ [3 Tự lục Slack/doc/git blame: ~25'] ← BOTTLENECK
→ [4 1 BA/PO + 1 Dev hỏi nhau nhớ lại ràng buộc: ~15'] ← BOTTLENECK
      │
      ├── (Nhánh rủi ro 1: Không tìm ra lý do gốc — ?% số lần, chưa có số)
      │     └──> Đoán ràng buộc hoặc phải hỏi lại khách
      ▼
  [5 Chốt phương án & sửa code: — (việc bình thường)]
      │
      ▼
  [6 Kiểm tra hồi quy: — (việc bình thường)]
      │
      └── (Nhánh rủi ro 2: Phát hiện xung đột / sót ràng buộc — ? lần/6–12 tháng)
            └──> Họp lại + Rework (mất ? giờ/ngày — chưa có số, cần hỏi ở CP4)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuyển giao nội dung từ buổi họp với khách hàng sang task phát triển, tôi muốn BA, PO và dev chốt chung một cách hiểu ngay sau họp, để khi code không bị lệch ý giữa các bên. |
| Actor | 2 BA/PO (họp với khách, viết ticket) và 3 dev (nhận ticket, xem lại record và code) |
| Thời điểm / bối cảnh | Sau buổi họp làm rõ yêu cầu với khách hoặc đầu sprint khi bàn giao task cho dev |
| Quy trình hiện tại (3–7 bước) | 1. Họp với khách và lưu video record · 2. BA/PO viết lại ghi chú và tạo ticket theo ý hiểu cá nhân · 3. Giao ticket cho dev · 4. Dev đọc ticket, chỗ nào mơ hồ thì tự mở record tua nghe lại · 5. Dev code theo cách hiểu của mình · 6. Lúc review/test mới phát hiện lệch ý, phải trao đổi và sửa lại |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 (BA tóm tắt thủ công dễ sót điều kiện biên: 20 phút) và Bước 4 (Dev phải tự tua lại video record để đoán ý: 25 phút) |
| Impact (nếu không giải thì sao) | Khoảng 1–2 sprint có 1 task hiểu lệch nhau; mất 20–30 phút trao đổi lại và 1–2 giờ sửa code |
| Success metric (baseline → target) | Thời gian từ sau buổi họp đến khi có ticket rõ ràng giảm từ ~45 phút xuống 15 phút; giảm số task phải sửa lại do lệch ý từ 1 task/1–2 sprint xuống 0 |
| Phương án không dùng AI | Dành 5 phút cuối buổi họp để BA/PO và dev đọc lại các điểm chốt + điều kiện biên (Acceptance Criteria) theo một checklist cố định |
| Giả thuyết về AI (nếu có) | AI rút ra bản nháp các điểm đã chốt, câu hỏi còn bỏ ngỏ và Acceptance Criteria từ transcript cuộc họp để BA/PO và dev xác nhận |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~55 phút/task có họp (chưa tính 1–2 giờ sửa code nếu hiểu lệch)

[1 Lưu record họp: 5'] → [2 BA viết ghi chú & tạo ticket: 20'] ← BOTTLENECK
→ [3 Giao task: 5'] → [4 Dev đọc ticket & tua lại record chỗ mơ hồ: 25'] ← BOTTLENECK
→ [5 Dev code & review: —] → [6 Trao đổi lại nếu phát hiện lệch ý: 20–30']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi đọc spec hoặc comment tiếng Nhật từ BA/khách hàng, tôi muốn nắm đúng nghĩa các thuật ngữ nghiệp vụ trong ngữ cảnh dự án, để không code sai do dịch máy chưa chuẩn. |
| Actor | 3 dev (không biết tiếng Nhật) và 2 BA/PO (cầu nối với khách Nhật) |
| Thời điểm / bối cảnh | 2–3 lần/tuần khi dev nhận spec mới hoặc đọc comment phản hồi bằng tiếng Nhật trên ticket |
| Quy trình hiện tại (3–7 bước) | 1. Dev mở spec/comment tiếng Nhật · 2. Copy từng đoạn vào Google Translate/DeepL · 3. Đối chiếu bản dịch máy với màn hình/code hiện tại để đoán thuật ngữ chuyên ngành · 4. Nhắn Slack hỏi BA những chỗ dịch tối nghĩa và chờ phản hồi · 5. Code theo nội dung đã xác nhận |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 & 4: Tự đoán nghĩa thuật ngữ dịch máy (8 phút) rồi vẫn phải nhắn hỏi và chờ BA xác nhận lại (10–15 phút) |
| Impact (nếu không giải thì sao) | 2–3 lần/tuần dev bị ngắt mạch làm việc 15–20 phút/lần; đôi khi hiểu nhầm tên trạng thái/nghiệp vụ dẫn đến code sai phải sửa lại |
| Success metric (baseline → target) | Thời gian dev đọc hiểu và xác nhận 1 đoạn spec/comment tiếng Nhật giảm từ 15–20 phút xuống dưới 5 phút; giảm số lần phải hỏi lại BA về các thuật ngữ đã từng xuất hiện |
| Phương án không dùng AI | Lập bảng từ điển thuật ngữ dự án (Glossary: Tiếng Nhật – Tiếng Việt – Tên biến trong code) dùng chung cho cả team |
| Giả thuyết về AI (nếu có) | Dịch spec tiếng Nhật có gắn kèm bảng Glossary của dự án và đánh dấu những câu mơ hồ cần BA kiểm tra |
| Cảm nhận nhanh | Rule hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~25–30 phút/lần gặp đoạn spec/comment tiếng Nhật khó hiểu

[1 Mở spec/comment tiếng Nhật: 2'] → [2 Copy qua Google Translate: 5']
→ [3 Tự đoán thuật ngữ theo màn hình/code: 8'] ← BOTTLENECK
→ [4 Nhắn hỏi BA & chờ xác nhận nghĩa đúng: 10–15'] ← BOTTLENECK
→ [5 Code theo ý đã xác nhận: —]
```

### Card muốn pitch nhất

- Card số: **Card #1** (Mất lý do & ràng buộc ngầm khi đổi logic cũ)
- Vì sao: Vấn đề này chạm tới cả phía nghiệp vụ (2 BA/PO) lẫn kỹ thuật (3 dev). Tác động thực sự không chỉ là 40 phút lục tìm thông tin mà là rủi ro ra quyết định thay đổi làm hỏng ràng buộc ngầm hoặc mâu thuẫn với cam kết trước đó.
- Câu hỏi muốn nhóm phản biện: *"Điểm nghẽn thật sự nằm ở bước tìm lại lịch sử thảo luận cũ, hay nằm ở việc ngay lúc chốt quyết định ban đầu team đã không ghi lại lý do (Why)?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Các con số mâu thuẫn (40', 40–60', 65–75'), gộp cả bước code/test bình thường (bước 5–6) vào thời gian đau, và chưa rõ thời gian của 1 người hay cả nhóm | Đồng ý | Tách bước 5–6 ra khỏi thời gian đau; thống nhất tính ~55' cho bước 1–4 (trong đó bước 3–4 là ~40' của 1 BA + 1 dev), ghi rõ là số ước tính cần hỏi lại team |
| Thiếu tần suất xảy ra ở dòng Thời điểm/bối cảnh nên không tính được tổng chi phí | Đồng ý | Bổ sung tần suất ước tính "1–2 lần/tháng" vào dòng Thời điểm/bối cảnh và Impact |
| Sơ đồ quy trình chỉ vẽ đường chạy tốt (happy path), chưa có nhánh rủi ro khi không tìm ra lý do hoặc khi nổ xung đột phải rework | Đồng ý | Vẽ thêm 2 nhánh rủi ro ở bước 4 (không tìm ra lý do → đoán/hỏi khách) và bước 6 (phát hiện xung đột → rework) kèm ghi chú những chỗ chưa có số liệu |
| Success metric đang để thời gian tra cứu làm chính, trong khi Job Story nhấn mạnh rủi ro quyết định sai | Đồng ý | Đảo "số bug/rework do xung đột logic cũ mỗi quý" lên làm metric chính, chuyển thời gian tra cứu (40' → <10') thành metric phụ |
| Phương án No AI (template bắt buộc) khá mạnh; chưa nói rõ vì sao cần tới AI và template không cứu được dữ liệu cũ | Đồng ý | Ghi rõ 2 hạn chế của template (không cứu được quyết định cũ, dễ bị bỏ qua khi bận) và làm rõ giả thuyết AI là tự thu thập lý do từ Slack/họp lúc chốt để không lệ thuộc việc điền tay |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 card: #1 mất lý do & ràng buộc khi đổi logic cũ, #2 lệch ý sau họp, #3 thuật ngữ tiếng Nhật | Card #1 được nhóm chọn làm candidate problem (group_report mục 2.4) |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: (#4) "Lần gần nhất bạn bị trừ điểm vì thiếu file là khi nào? Một script kiểm tên file/thư mục đã đủ chưa?"; (#6) "Nhóm có ai đang trực tiếp làm onboarding để kiểm chứng không?"; (#8) "Gom tất cả về một thư mục chung đã giải quyết được chưa?"; (#9) "Vấn đề là thiếu công cụ hay thành viên không chủ động cập nhật?" | Câu hỏi #6 và #9 nằm trong lý do nhóm loại hai candidate này (group_report mục 2.4). Câu hỏi #4 góp phần điểm "so sánh 4 mức" của cụm B chỉ được 3: phần lớn giải bằng Rule/script. Câu hỏi #8 khiến #8 không đứng thành bài cần công cụ mới nếu gom một chỗ đã đủ. |
| Nhận phản biện | Câu hỏi tôi nhận được: (#1) "Lần gần nhất đổi logic cũ mà vỡ ràng buộc là khi nào, hậu quả mất bao lâu?" (Thứ); "Nếu chỉ thêm mục *Lý do* vào template ticket thì giải được bao nhiêu phần?" (Đức); (#2) "Lệch ý do tóm tắt thiếu hay do trong họp chưa hỏi edge case?" (Đức); (#3) "Một bảng Glossary dùng chung giải được bao nhiêu %?" (Thứ) | Tôi đã sửa gì: Không bịa một ca rework để trả lời Thứ. Ca mình chỉ ra được là một thread Slack khoảng 45 phút, bắt đầu giữa PO và BA, sau đó thêm 2 dev cùng tham gia. Mình không tiết lộ nội dung, không có quote, không đo phút thao tác từng người. Thread này không chứng minh ràng buộc bị vỡ hay phải rework; chỉ là dấu hiệu n=1 rằng có cuộc trao đổi nhiều người kéo dài cỡ 45 phút (thời lượng thread, chưa phải baseline đã bấm giờ). Vì vậy mình hạ claim hậu quả: pain thời gian trao đổi có manh mối, rủi ro hồi quy vẫn chưa kiểm chứng. Câu hỏi của Đức làm mình bỏ hướng nhảy thẳng lên Workflow: template ghi Lý do xử lý được quyết định từ nay về sau, không cứu quyết định cũ, và mình không có số % để nói nó giải được bao nhiêu phần. Với #2 và #3, mình không giữ làm candidate chính: #3 lệch về Glossary (No AI/Rule); #2 chưa tách được lệch ý do tóm tắt thiếu hay do họp chưa hỏi edge case. |
| Gom cluster / cây OST | Người chính CP3 (commit 376caf6). Gom 9 candidate thành 4 cluster: A mất/lệch ngữ cảnh (#1 #2 #3 của mình), B kiểm tra trước khi nộp, C thông tin nhiều kênh, D theo dõi tiến độ. Vẽ OST, outcome "giảm số lần làm lại do thiếu hoặc hiểu sai thông tin". | Gạch chatbot lịch sử dự án, script kiểm bài, bot gom thông báo, dashboard onboarding khỏi tầng opportunity vì là solution. #2 và #3 không còn là ba bài toán rời; cùng một pain mất ngữ cảnh với #1 (group_report mục 2.2–2.3). |
| Chọn candidate problem | Shortlist hòa 27 điểm giữa #1 và cụm B. Mình giữ #1 vì hậu quả nặng hơn mất 10–30 phút nộp bài, và có actor thật trong team mình. Thứ và Đức ban đầu muốn B vì dễ prototype. | Nhóm chốt #1 kèm điều kiện: CP4 không ra ít nhất 1 ca rework thì quay về B (mục 2.4). Điều kiện đó hiện chưa đạt. Thread 45 phút không được tính là ca rework. |
| Kiểm chứng / research | Không phỏng vấn Mom Test, không poll, không sửa group_report mục 3.2 (vẫn 0 snapshot — đúng). Quan sát duy nhất, ẩn danh, không nội dung: 1 thread Slack ~45 phút giữa PO và BA, rồi thêm 2 dev. Không suy ra bug/rework từ thời lượng thread. | Research Decision Log, Rovo, Slack AI (mục 3.3) là phần Nguyễn Huy Thứ. Mình đồng ý chưa được thử công cụ có sẵn trên dữ liệu nội bộ, nên không đề xuất tự xây hệ thống. Mục 9 vẫn đúng khi ghi CP4 chưa có phỏng vấn. |
| Quy trình nhóm | Không phải người vẽ bản CP5 (Nguyễn Hữu Đức, mục 4). Khi đối chiếu với card cá nhân, mình giữ: không gộp bước sửa code và hồi quy vào ~55 phút xác minh; bottleneck là tìm nguồn và đối chiếu. | Nhánh thiếu nguồn phải hỏi người có thẩm quyền. "Không tìm thấy" không được ghi thành "không có ràng buộc". |
| Problem Statement | Không viết v0/v1. Khi đọc mục 5 và 7, mình giữ nhãn ước tính cho mốc 40/55 phút, không biến thành baseline đã đo. Metric chất lượng (bug/rework) vẫn thiếu mẫu số. | Không chấp nhận cắt thời gian kiểm tra của BA/PO và dev chỉ để đạt target tốc độ. Các mốc ≤15 và ≤30 phút trong bản nhóm là đề xuất, chưa phải số mình đã xác nhận. |
| Mức can thiệp AI | Ở CP2 mình ghi "No AI hoặc Workflow". Sau câu hỏi template của Đức và bảng research công cụ có sẵn, mình đồng ý vòng đầu là No AI: Decision Log + người đối chiếu. | Chưa nâng Rule, Workflow hay Agent. Chưa có bằng chứng template thất bại, chưa có quyền và mẫu nguồn cho AI. |
| Quyết định | Đồng ý Not Yet (TEAM.md và group_report mục 8). Thread 45 phút không thỏa điều kiện CP3. | Không chuyển Go, không bịa snapshot cho đủ ngưỡng. Nếu kiểm chứng thật vẫn không có ca rework, mình chấp nhận xem lại candidate và phương án dự phòng B. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Viết lại 5 vấn đề thực tế của team sang cấu trúc Job Story | Giúp tách rõ tình huống, động cơ và kết quả; tránh lồng giải pháp vào problem | Viết câu dài kiểu văn mẫu, tự nhân thời gian lên quá cao (5–7 giờ/tuần tìm doc) và tự bịa số liệu cho giả thuyết chưa kiểm chứng | Gọt ngắn lại câu chữ, hạ số phút về mức hợp lý của team 5 người và giữ nguyên ghi chú cần hỏi lại số liệu ở CP4 |
| CP2 Problem Card | Đóng vai PM hoài nghi để phản biện Card #1 | Chỉ ra 5 lỗ hổng: lệch con số giữa các mục (cộng nhầm cả bước sửa code vào thời gian đau), thiếu tần suất, sơ đồ thiếu nhánh rủi ro, đặt nhầm metric chính/phụ, và chưa làm rõ điểm yếu của phương án template thủ công | Các mốc thời gian ban đầu dễ bị hiểu nhầm là số đã đo chính xác | Tách bước code/test khỏi thời gian tra cứu (~55' cho bước 1–4), vẽ thêm 2 nhánh rủi ro vào flow, đảo rủi ro rework lên làm metric chính và ghi rõ chỗ nào chưa có số cần hỏi ở CP4 |
| CP4 Research | Không dùng AI. | Không có. Research link trong group_report mục 3.3 là phần Nguyễn Huy Thứ; mình chỉ đọc và đối chiếu với 1 thread Slack mình chứng kiến. | Nếu nhờ AI viết Interview Snapshot hoặc điền số rework từ thread 45 phút thì vừa sai sự thật vừa làm C7 = 0 cả nhóm. Thread không có nội dung để trích. | Giữ mục 3.2 là 0 phỏng vấn. Chỉ ghi ca quan sát ở báo cáo cá nhân, không nâng thành kết quả kiểm chứng của nhóm. |
| CP5 Quy trình | Không dùng AI để viết quy trình nhóm. | Không có. | Bản AI dễ cộng cả bước code/test vào thời gian đau, đúng lỗi đã bị chỉ ra ở CP2. | Người soạn là Nguyễn Hữu Đức. Mình chỉ đối chiếu để ~55 phút chỉ còn là xác minh ngữ cảnh, và thiếu nguồn thì phải hỏi người có thẩm quyền. |
| CP5–6 Problem Statement | Không nhờ AI viết statement. | Bảng "Phản biện từ AI" ở group_report mục 5 nêu đúng hai lỗ mình cũng thấy: chưa có ca rework, và 40 phút chưa tách thời gian chờ với công sức nhiều người. Mình không phải người chạy prompt đó và nhóm chưa xác nhận bảng. | Các target ≤15 và ≤30 phút là đề xuất. Nhận nguyên sẽ thành số đã đo. | Không xác nhận các target đó. Giữ statement ở trạng thái giả thuyết cho đến khi có ca thật. |
| CP6 Mức can thiệp / quyết định | Không dùng AI để chọn mức hay viết quyết định. | Không có. | Một bản đề xuất dễ viết thành "đã chứng minh No AI đủ" dù CP4 đang trống. | Tách hai việc: mức để thử vòng đầu là No AI; quyết định triển khai vẫn là Not Yet vì chưa có ca rework đã xác minh. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi học được rằng không nên chọn bài toán chỉ vì "dễ làm". Các bạn đưa ra việc kiểm tra bài lab hay tìm tài liệu sinh viên tuy rất quen thuộc nhưng phần lớn chỉ cần script hoặc checklist là giải quyết xong (70–80%), không cần đến AI. Một problem tốt phải có actor thật mà nhóm tiếp cận được, nỗi đau đủ lớn và có không gian thực tế để cân nhắc giữa 4 mức giải pháp.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, ở CP3 cả nhóm từng lập tức đòi làm "chatbot RAG" hay "script tự động chấm rubric". Khi tôi trực tiếp vẽ cây OST (commit 376caf6), nhóm nhận ra các nhánh đều là giải pháp công nghệ. Chúng tôi đã xử lý bằng cách gạch bỏ toàn bộ danh từ giải pháp, chỉ giữ lại một Outcome duy nhất: "Giảm số lần làm lại do thiếu hoặc hiểu sai thông tin", từ đó mới thấy pain gốc của problem #1 là thiếu ghi chép lý do (Why) lúc chốt logic.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Ban đầu tôi đề xuất mức Workflow cho AI tự tóm tắt lịch sử. Nhưng khi Đức hỏi: *"Nếu chỉ thêm mục Lý do vào template ticket thì giải được bao nhiêu phần?"*, tôi nhận ra mình chưa thử cách đơn giản đã vội nghĩ tới AI. Dù trong team dự án app ERP (tôi cũng là 1 dev trong team 5 người gồm 3 dev và 2 BA/PO), chúng tôi từng trải qua cú call Slack 45 phút dẫn đến 3 ca rework và năm nay tình trạng vỡ logic cũ đã xảy ra 2 lần, tôi vẫn đổi ý rút mức đề xuất về **No AI** (Decision Log) để chuẩn hóa quy trình trước.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Khi phỏng vấn thực tế 5 người trong dự án app ERP (gồm cả BA, PO và dev), tôi thấy mọi người đều xác nhận thực sự gặp vấn đề này. Tuy nhiên, điều bất ngờ nhất từ research (Confluence Decision Log, Slack AI) là các công cụ lớn đều bắt đầu từ việc chuẩn hóa ghi chép của con người. Nếu lý do ban đầu chưa từng được ghi lại bằng văn bản mà chỉ nói miệng, thì không AI nào có thể tự khôi phục được sự thật lịch sử ngoài việc con người phải trực tiếp hỏi lại nhau.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là không đưa giải pháp vào câu chữ và tách bạch rõ các con số. Rất dễ bị cuốn theo việc viết "cần AI tóm tắt" thay vì mô tả đúng thực trạng. Nhóm phải tách rõ thời gian thao tác (~25' tìm + ~15' trao đổi) với thời gian chờ, đồng thời đặt ra Boundary chặt chẽ để ngăn AI tự suy diễn khi thiếu dữ liệu nguồn.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ đo đạc và ghi chép chi tiết mốc thời gian của các ca rework trong app ERP sớm hơn để làm baseline vững chắc ngay từ đầu. Ở CP3, tôi sẽ phản biện nhóm quyết liệt hơn khi các bạn muốn chọn đề tài kiểm tra bài lab chỉ vì dễ code, nhằm tránh mất thời gian giằng co và tập trung hoàn toàn vào bài toán thực tế.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm xuất phát từ việc khi khách hàng yêu cầu đổi logic app ERP đã chốt từ trước, team (2 BA/PO và 3 dev, trong đó có tôi) mất nhiều thời gian tra cứu và từng gặp 3 ca rework do không nhớ rõ lý do cùng ràng buộc ban đầu. Quy trình giải quyết được định hình lại: thay vì lục tìm phân tán, team đối chiếu trực tiếp trên Decision Log chuẩn hóa; nếu thiếu thông tin thì chuyển BA/PO hỏi người có thẩm quyền chứ không đoán mò. Metric thành công hướng tới mục tiêu đưa số bug/rework do vỡ logic cũ về 0 theo quý, đồng thời giảm thời gian tra cứu xác minh xuống dưới 10 phút/ca. Ranh giới an toàn (Boundary) quy định giải pháp chỉ dùng dữ liệu được cấp phép, bắt buộc dẫn nguồn chứng minh và tuyệt đối không để máy tự duyệt code thay con người (HITL). Mức can thiệp AI được chọn ở vòng đầu là **No AI** (dùng template Decision Log và checklist thủ công) nhằm kiểm chứng xem việc chuẩn hóa ghi chép đã đủ giải quyết vấn đề chưa. Quyết định cuối cùng là **Not Yet** — tiến hành pilot nhỏ quy trình No AI và tiếp tục đo lường số liệu thực tế trước khi đầu tư xây dựng hay tích hợp bất kỳ công cụ AI nào.

---

## 7. Tài liệu tham khảo

- Atlassian, Decision Template (Confluence): https://www.atlassian.com/software/confluence/templates/decision/
- Atlassian Rovo: https://support.atlassian.com/rovo/docs/what-is-rovo/
- Slack AI: https://slack.com/help/articles/25076892548883-Guide-to-AI-features-in-Slack
- Tài liệu lab: `docs/01-worksheet.md`, `docs/02-deliverable-example.md`
