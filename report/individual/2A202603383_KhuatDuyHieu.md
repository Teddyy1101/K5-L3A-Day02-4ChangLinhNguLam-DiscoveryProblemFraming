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
| CP1 Scan | Viết lại 5 vấn đề thực tế của team sang cấu trúc Job Story | Giúp tách rõ tình huống, động cơ và kết quả; tránh lồng giải pháp vào problem | Viết câu dài kiểu văn mẫu, tự nhân thời gian lên quá cao (5–7 giờ/tuần tìm doc) và tự bịa số liệu cho giả thuyết chưa kiểm chứng | Gọt ngắn lại câu chữ, hạ số phút về mức hợp lý của team 5 người và giữ nguyên ghi chú cần hỏi lại số liệu ở CP4 |
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
