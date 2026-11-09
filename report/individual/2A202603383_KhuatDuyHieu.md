# Báo cáo cá nhân — 2A202603383_KhuatDuyHieu

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
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
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Viết lại 5 vấn đề thực tế của team sang cấu trúc Job Story | Giúp tách rõ tình huống, động cơ và kết quả; tránh lồng giải pháp vào problem | Viết câu dài kiểu văn mẫu, tự nhân thời gian lên quá cao (5–7 giờ/tuần tìm doc) và tự bịa số liệu cho giả thuyết chưa kiểm chứng | Gọt ngắn lại câu chữ, hạ số phút về mức hợp lý của team 5 người và giữ nguyên ghi chú cần hỏi lại số liệu ở CP4 |
| CP2 Problem Card | Đóng vai PM hoài nghi để phản biện Card #1 | Chỉ ra 5 lỗ hổng: lệch con số giữa các mục (cộng nhầm cả bước sửa code vào thời gian đau), thiếu tần suất, sơ đồ thiếu nhánh rủi ro, đặt nhầm metric chính/phụ, và chưa làm rõ điểm yếu của phương án template thủ công | Các mốc thời gian ban đầu dễ bị hiểu nhầm là số đã đo chính xác | Tách bước code/test khỏi thời gian tra cứu (~55' cho bước 1–4), vẽ thêm 2 nhánh rủi ro vào flow, đảo rủi ro rework lên làm metric chính và ghi rõ chỗ nào chưa có số cần hỏi ở CP4 |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
