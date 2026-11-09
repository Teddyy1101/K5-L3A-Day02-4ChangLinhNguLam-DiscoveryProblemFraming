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
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tra cứu tài liệu vận hành hoặc đặc tả kỹ thuật cũ để sửa lỗi hoặc phát triển tiếp tính năng, tôi muốn có một nguồn thông tin duy nhất và được cập nhật đầy đủ, để không phải lục tìm rải rác qua các kênh chat Slack, file Word và trang Notion rời rạc. | Toàn bộ 5 dev trong team | Mỗi ngày mỗi dev mất khoảng 15–20 phút tìm kiếm link và hỏi han đồng nghiệp. Cả team mất ~6–8 giờ/tuần chỉ để tìm tài liệu. Bằng chứng: Trên Slack channel dự án thường xuyên xuất hiện các câu hỏi lặp lại: "Link doc setup ở đâu?", "File spec chức năng thanh toán cũ lưu chỗ nào?". |
| 2 | Pain từ người khác | Khi tiếp nhận một thành viên mới vào team phát triển, tôi muốn có bộ tài liệu onboarding và hướng dẫn cài đặt môi trường được hệ thống hóa rõ ràng theo từng bước, để người mới có thể tự thiết lập môi trường và làm quen codebase trong 3 ngày đầu mà không làm gián đoạn công việc của các thành viên khác. | Thành viên mới onboard và senior/mentor hướng dẫn trong team 5 người | Người mới mất trung bình 5–7 ngày làm việc mới cấu hình xong môi trường và chạy thử được dự án. Senior hướng dẫn bị ngắt quãng khoảng 1–1.5 giờ mỗi ngày trong tuần đầu để trả lời các câu hỏi cấu hình lặp lại và gửi từng link tài liệu rời rạc. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận yêu cầu phát triển từ các buổi họp làm việc giữa BA, PO và Client, tôi muốn nội dung thống nhất và tiêu chí chấp nhận (Acceptance Criteria) được văn bản hóa rõ ràng, để dev hiện thực hóa đúng nghiệp vụ ngay từ đầu mà không bị tình trạng "tam sao thất bản" giữa các bên dẫn đến việc phải làm lại (rework). | 5 dev trong team, BA và PO dự án | Trung bình mỗi sprint (2 tuần) có ít nhất 1 task bị hiểu sai phạm vi (scope) do BA, PO và Dev suy diễn khác nhau từ video record cuộc họp. Team mất thêm 3–5 giờ để refactor/code lại và tốn 1 buổi họp 45 phút giữa sprint để đối soát lại yêu cầu. |
| 4 | Tốn thời gian (Rủi ro / Chất lượng quyết định) | Khi khách hàng yêu cầu đổi một logic cũ mà không ai nhớ rõ lý do ban đầu, tôi muốn biết chắc các ràng buộc ngầm đứng sau quyết định đó, để không đưa ra thay đổi gây lỗi hồi quy hoặc mâu thuẫn với những cam kết trước đây. | 2 BA/PO (người quyết định và cam kết với khách), 3 dev (người sửa code và chịu lỗi hồi quy) trong team | Ước tính trong 6–12 tháng qua: có ít nhất 3–4 lần team đổi logic cũ rồi phát hiện xung đột/bug trên staging/production; mỗi lần mất 2–3 ngày của cả BA và Dev để họp giải trình, tra cứu và rework; 100% các lần đổi này đều không tìm ra tài liệu ghi lại lý do ban đầu (chỉ dựa vào trí nhớ rời rạc). Nhóm sẽ kiểm chứng lại tần suất chính xác ở CP4. |
| 5 | Lặp lại | Khi tiếp nhận tài liệu đặc tả (spec) và phản hồi nghiệp vụ bằng tiếng Nhật từ khách hàng, tôi muốn hiểu chuẩn xác các thuật ngữ chuyên ngành và sắc thái yêu cầu, để lập trình đúng mà không phải đoán mò qua các công cụ dịch tự động vốn hay bị sai lệch ngữ cảnh. | 5 dev trong team (không ai thành thạo tiếng Nhật chuyên ngành) và BA cầu nối | Mỗi dev mất khoảng 15–20 phút/ngày copy-paste từng đoạn tài liệu qua Google Translate/DeepL rồi tự đoán nghĩa. Khoảng 1 lần/tháng phát sinh bug do dịch sai thuật ngữ nghiệp vụ (như trạng thái đơn hàng), phải tốn thêm 1–2 ngày chờ BA xác nhận lại với khách hàng phía Nhật. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý AI gợi ý nhưng BỎ:**
  - *Gợi ý 1: "Cần xây dựng chatbot AI tra cứu tự động tài liệu trên Slack"* -> **Bỏ**, vì đây là solution (giải pháp AI trá hình), vi phạm nguyên tắc cơ bản "Problem first, not AI first" của lab.
  - *Gợi ý 2: "Tự động phân loại và gán nhãn ticket Jira bằng mô hình phân loại văn bản"* -> **Bỏ**, vì quy mô team chỉ có 5 dev, lượng ticket mỗi sprint (~20–25 ticket) không phải là điểm nghẽn gây đau đớn thực sự so với việc mất context hay hiểu lệch spec.
  - *Gợi ý 3: "Tool AI tự động sinh unit test từ tài liệu tiếng Nhật"* -> **Bỏ**, vì nhảy vội vào giải pháp công nghệ phức tạp trong khi gốc rễ vấn đề là tài liệu đầu vào chưa được hiểu đúng và thống nhất ngữ nghĩa.
- **Ý giữ lại và điều chỉnh:**
  - Tận dụng AI để rà soát và chuẩn hóa cấu trúc câu của 5 vấn đề cốt lõi đã rút ra từ trải nghiệm thật, đưa về chuẩn cú pháp **Job Story** (*Khi [tình huống], tôi muốn [động cơ], để [kết quả]*).
  - Loại bỏ triệt để các từ ngữ mang tính giải pháp (như "cần công cụ", "cần bot", "cần phần mềm"), tập trung hoàn toàn vào nỗi đau vận hành, actor chịu ảnh hưởng và các con số đo lường thực tế của team 5 dev.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

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
| CP1 Scan | Chuẩn hóa Job Story và phản biện để tránh solution trá hình | Giúp cấu trúc lại câu văn mạch lạc theo chuẩn "Khi... tôi muốn... để..." | AI có xu hướng tự động chèn giải pháp vào (như "cần bot tra cứu", "cần tool AI"), gợi ý thêm các vấn đề quá vĩ mô | Tôi đã loại bỏ hoàn toàn các giải pháp AI trá hình, giữ nguyên 5 vấn đề thật từ dự án và tự điền các con số đo lường thực tế của team |
| CP2 Problem Card | | | | |
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
