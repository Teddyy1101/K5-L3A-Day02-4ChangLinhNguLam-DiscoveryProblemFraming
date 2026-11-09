# Báo cáo cá nhân — 2A202603429_NguyenHuuDuc

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Hữu Đức
- MSSV:2A202603429
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 4TrangLinhNguLam
- Link repo nhóm:[github.com/Teddyy1101/K5-L3A-Day02-4ChangLinhNguLam-DiscoveryProblemFraming](https://github.com/Teddyy1101/K5-L3A-Day02-4TrangLinhNguLam-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính                              | Job Story: Khi… tôi muốn… để…                                                                                                                                                                                                    | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng)                   |
| -: | ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | -------------------------------------------------------------------------------------- |
| 1 | Lặp lại                                | Khi viết báo cáo tiến độ hằng tuần, tôi muốn giảm việc nhập lại những thông tin đã cập nhật trong công việc hằng ngày, để dành thời gian cho phát triển ứng dụng.                                       | Developer              | 60 phút viết báo cáo/ tuần                                                        |
| 2 | Lặp lại                                | Khi nhận yêu cầu làm rõ tiến độ của cùng một đầu việc từ nhiều người, tôi muốn giảm số lần phải giải thích lại trạng thái, để giữ thời gian làm việc tập trung.                                     | Developer              | 5 lần trả lời nội dung trong tuần, mỗi lần mất 30 phút                       |
| 3 | Tốn thời gian                          | Khi tiếp nhận một lỗi từ người dùng, tôi muốn có đủ thông tin để tái hiện lỗi, để bắt đầu tìm nguyên nhân sớm hơn.                                                                                         | Developer              | 1h30p từ lúc báo lỗi đến khi tái hiện được, 4 lần hỏi bổ sung thông tin |
| 4 | Tốn thời gian                          | Khi công việc phụ thuộc vào quyết định của bộ phận khác, tôi muốn biết ai chịu trách nhiệm phản hồi và khi nào có kết quả, để chủ động sắp xếp phần việc tiếp theo.                                  | Developer              | 5 tiếng bị chặn/ tuần                                                              |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị báo cáo tuần từ đầu việc, thay đổi mã nguồn và trao đổi trong nhóm, tôi muốn xác định đúng phần đã hoàn thành, còn dang dở và đang bị chặn, để báo cáo phản ánh đúng thực tế. | Developer              | Cần 60 phút tổng hợp                                                              |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi đánh giá khả năng hoàn thành mục tiêu tuần, tôi muốn hiểu các phụ thuộc và rủi ro từ tiến độ của từng thành viên, để đưa ra cam kết phù hợp với năng lực thực tế của nhóm.                  | Tech lead              | Cần 2 tiếng tổng hợp tình hình                                                   |
| 7 | Pain từ người khác                   | Khi nhận tính năng để kiểm thử, tôi muốn biết phạm vi thay đổi, điều kiện kiểm thử và các giới hạn đã biết, để tránh mất thời gian xác minh lại với developer.                                         | Tester                 | 5 lượt hỏi lại bổ sung/ tính năng                                              |
| 8 | Pain từ người khác                   | Khi đọc báo cáo tiến độ của developer, tôi muốn phân biệt rõ phần đã hoàn thành với phần chỉ mới bắt đầu hoặc đang chờ, để đánh giá đúng khả năng bàn giao.                                       | PM                     | Mất 4 lần hỏi lại sau báo cáo                                                    |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                                     | Vì sao chọn                                                                                                                                                           | Điều còn chưa chắc                                                                                                                                                       |
| ---: | ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    1 | Báo cáo tuần(#5)                         | Lặp lại hằng tuần, mất  **60 phút/developer/tuần** ; phạm vi rõ và dễ đo trước–sau.                                                                | Có bao nhiêu developer gặp vấn đề?  Phần nào tốn thời gian nhất?                                                                                                  |
|    2 | Thiếu thông tin tái hiện lỗi(#3)       | Có bằng chứng cụ thể về thời gian và số lần hỏi lại; ảnh hưởng đến cả developer lẫn người báo lỗi; phạm vi rõ, dễ đo hiệu quả cải thiện. | Có bao nhiêu ticket như vậy mỗi tuần? Trong 90 phút, bao nhiêu là thao tác và bao nhiêu là chờ? Thông tin nào thường thiếu nhất?                          |
|    3 | Chờ quyết định từ bộ phận khác (#4) | Đầu việc bị chặn  **5 giờ/tuần** , có thể ảnh hưởng trực tiếp đến thời hạn bàn giao và công việc phụ thuộc.                               | Trong thời gian chờ có thể làm việc khác không? Nguyên nhân chính là chưa rõ người phụ trách, thiếu thông tin hay người quyết định chưa phản hồi? |

### Problem Card #1

| Trường                                        | Nội dung                                                                                                                                                                                                                               |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                       | Khi chuẩn bị báo cáo tuần từ đầu việc, thay đổi mã nguồn và trao đổi trong nhóm, tôi muốn xác định đúng phần đã hoàn thành, còn dang dở và đang bị chặn, để báo cáo phản ánh đúng thực tế. |
| Actor                                           | Developer                                                                                                                                                                                                                               |
| Thời điểm / bối cảnh                       | Sáng thứ 2, trước 10h                                                                                                                                                                                                               |
| Quy trình hiện tại (3–7 bước)             | 1. Xem công việc trên Jira. 2. Kiểm tra commit/PR. 3. Đọc lại trao đổi trong nhóm. 4. Tổng hợp kết quả và vướng mắc. 5. Viết báo cáo. 6. Review và gửi.                                                          |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4–5: phải nối thông tin rời rạc thành nội dung rõ ràng; dễ bỏ sót kết quả hoặc mô tả chưa đúng trạng thái.                                                                                                |
| Impact (nếu không giải thì sao)             | Giả định mất 60 phút/người/tuần. Nếu 10 developer cùng gặp vấn đề, tổng thời gian là 10 giờ/tuần. Cần kiểm chứng thêm số lần gửi trễ và phải đính chính.                                                |
| Success metric (baseline → target)             | Giảm thời gian từ 60 xuống dưới 30 phút/báo cáo; số nội dung phải đính chính và số câu hỏi làm rõ từ quản lý không tăng.                                                                                      |
| Phương án không dùng AI                    | Mẫu báo cáo cố định và tiêu chí trạng thái thống nhất; giảm thời gian trình bày nhưng vẫn cần tự đọc và tổng hợp.                                                                                             |
| Giả thuyết về AI (nếu có)                  | AI có thể soạn nháp báo cáo từ dữ liệu công việc đã chọn; developer kiểm tra tính chính xác, bổ sung và duyệt trước khi gửi.                                                                                    |
| Cảm nhận nhanh                                | Workflow — nhiều bước thu thập và tổng hợp lặp lại theo tuần.                                                                                                                                                                |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút/tuần

[Xem Jira: 10'] → [Kiểm tra commit/PR: 5'] → [Đọc trao đổi: 10']
→ [Tổng hợp kết quả và vướng mắc: 15'] → [Viết báo cáo: 15'] ← BOTTLENECK
→ [Review và gửi: 5']
```

### Problem Card #2

| Trường                                        | Nội dung                                                                                                                                                                                      |
| ----------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                       | Khi nhận một báo lỗi chưa đủ thông tin, tôi muốn hiểu điều kiện và các bước xảy ra lỗi, để tái hiện được và bắt đầu xác định nguyên nhân sớm hơn.        |
| Actor                                           | Developer                                                                                                                                                                                      |
| Thời điểm / bối cảnh                       | Có báo lỗi mới từ QA hoặc người dùng.                                                                                                                                                 |
| Quy trình hiện tại (3–7 bước)             | 1. Đọc ticket. 2. Thử tái hiện. 3. Xác định thông tin còn thiếu. 4. Hỏi người báo lỗi. 5. Chờ phản hồi. 6. Thử lại và xác nhận lỗi.                                   |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4–5: hỏi đáp nhiều lượt vì thiếu môi trường, dữ liệu đầu vào hoặc bước thao tác.                                                                                   |
| Impact (nếu không giải thì sao)             | Giả định tốn 30 phút thao tác và 2 giờ chờ cho mỗi ticket thiếu thông tin. Nếu gặp 5 ticket/tuần, developer mất 2,5 giờ thao tác; việc bắt đầu sửa lỗi bị trì hoãn. |
| Success metric (baseline → target)             | Giảm trung vị thời gian từ nhận ticket đến tái hiện được từ 2,5 giờ xuống dưới 1 giờ; giảm số lượt hỏi bổ sung xuống tối đa 1 lượt/ticket.                        |
| Phương án không dùng AI                    | Biểu mẫu báo lỗi với các trường bắt buộc và checklist trước khi bàn giao; vẫn phụ thuộc vào mức độ đầy đủ, chính xác của người nhập.                            |
| Giả thuyết về AI (nếu có)                  | AI có thể nhận diện thông tin còn thiếu và soạn câu hỏi làm rõ từ nội dung ticket; developer xác nhận trước khi trao đổi.                                                 |
| Cảm nhận nhanh                                | Workflow — điểm nghẽn nằm ở chất lượng đầu vào và vòng hỏi đáp.                                                                                                               |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30 phút thao tác + 2 giờ chờ/ticket

[Đọc ticket: 5'] → [Thử tái hiện: 10'] → [Xác định thông tin thiếu: 5']
→ [Viết câu hỏi bổ sung: 5'] → [Chờ phản hồi: 2 giờ] ← BOTTLENECK
→ [Thử lại và xác nhận: 5']
```

### Problem Card #3

| Trường                                        | Nội dung                                                                                                                                                                                                                   |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                       | Khi một đầu việc phụ thuộc vào quyết định của bộ phận khác, tôi muốn biết người chịu trách nhiệm và thời điểm có phản hồi, để sắp xếp công việc và dự báo tiến độ bàn giao.       |
| Actor                                           | Developer                                                                                                                                                                                                                   |
| Thời điểm / bối cảnh                       | Đang phát triển tính năng nhưng gặp yêu cầu chưa rõ hoặc quyết định chưa được chốt.                                                                                                                     |
| Quy trình hiện tại (3–7 bước)             | 1. Phát hiện điểm chưa rõ. 2. Tìm người có quyền quyết định. 3. Gửi câu hỏi và ngữ cảnh. 4. Chờ hoặc nhắc phản hồi. 5. Nhận quyết định. 6. Đọc lại ngữ cảnh và tiếp tục                |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và 4: chưa rõ ai chốt quyết định và chưa có thời điểm phản hồi cụ thể.                                                                                                                            |
| Impact (nếu không giải thì sao)             | Giả định mỗi trường hợp làm đầu việc bị chặn 8 giờ làm việc và mất thêm 15 phút để lấy lại ngữ cảnh. Thời gian chờ có thể ảnh hưởng mốc bàn giao dù developer chuyển sang việc khác. |
| Success metric (baseline → target)             | Giảm trung vị thời gian bị chặn từ 8 xuống dưới 4 giờ làm việc; giảm số lần nhắc phản hồi; giảm số đầu việc trễ do chờ quyết định.                                                              |
| Phương án không dùng AI                    | Quy định người chịu trách nhiệm chốt, thời hạn phản hồi và cách chuyển cấp khi quá hạn; hiệu quả phụ thuộc vào việc thực hiện giữa các bộ phận.                                               |
| Giả thuyết về AI (nếu có)                  | AI có thể tổng hợp ngữ cảnh, câu hỏi chưa được trả lời và tác động đến tiến độ để người phụ trách xem xét; quyết định vẫn do người có thẩm quyền đưa ra.                           |
| Cảm nhận nhanh                                | Workflow và phối hợp — cần kiểm chứng trách nhiệm phản hồi trước khi đánh giá giá trị của AI.                                                                                                            |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 40 phút thao tác + 8 giờ làm việc chờ/đầu việc

[Xác định điểm chưa rõ: 5'] → [Tìm người quyết định: 10']
→ [Gửi câu hỏi và ngữ cảnh: 10'] → [Chờ quyết định: 8 giờ] ← BOTTLENECK
→ [Đọc lại ngữ cảnh và tiếp tục: 15']
```

### Card muốn pitch nhất

- Card số: #1
- Vì sao: Công việc lặp lại mỗi tuần, đang mất khoảng 60 phút/developer và có phạm vi rõ. Dễ thử nghiệm, đo thời gian tiết kiệm và kiểm tra chất lượng báo cáo.
- Câu hỏi muốn nhóm phản biện: Liệu mẫu báo cáo cố định và Jira đã đủ giải quyết vấn đề chưa? Nếu dùng AI, thời gian kiểm tra và sửa bản nháp có khiến tổng thời gian không giảm đáng kể không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                                                  | Đồng ý? | Đã sửa gì                                                                                           |
| --------------------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------- |
| Chưa chứng minh mẫu báo cáo cố định và Jira chưa đủ giải quyết vấn đề. | Đồng ý  | Bổ sung thử nghiệm với mẫu cố định và Jira để làm mốc so sánh trước khi đánh giá AI. |
| Thời gian kiểm tra, sửa bản nháp có thể làm giảm lợi ích tiết kiệm.        | Đồng ý  | Đo tổng thời gian chuẩn bị dữ liệu, tạo nháp, kiểm tra và sửa đến khi sẵn sàng gửi.    |
| Tiết kiệm thời gian chưa đủ chứng minh báo cáo có chất lượng.              | Đồng ý  | Bổ sung tiêu chí: thông tin sai hoặc thiếu và số câu hỏi làm rõ từ quản lý không tăng. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                     | Tôi đã làm gì?           | Kết quả / ảnh hưởng tới bài nhóm |
| -------------------------------- | ----------------------------- | ---------------------------------------- |
| Pitch Problem Card               |                               |                                          |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:    |                                          |
| Nhận phản biện                | Câu hỏi tôi nhận được: | Tôi đã sửa gì:                      |
| Gom cluster / cây OST           |                               |                                          |
| Chọn candidate problem          |                               |                                          |
| Kiểm chứng / research          |                               |                                          |
| Quy trình nhóm                 |                               |                                          |
| Problem Statement                |                               |                                          |
| Mức can thiệp AI               |                               |                                          |
| Quyết định                    |                               |                                          |

---

## 5. Dùng AI

| Checkpoint                          | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
| ----------------------------------- | ---------------------------- | ---------------------- | -------------------------------- | -------------------------------------------- |
| CP1 Scan                            |                              |                        |                                  |                                              |
| CP2 Problem Card                    |                              |                        |                                  |                                              |
| CP4 Research                        |                              |                        |                                  |                                              |
| CP5 Quy trình                      |                              |                        |                                  |                                              |
| CP5–6 Problem Statement            |                              |                        |                                  |                                              |
| CP6 Mức can thiệp / quyết định |                              |                        |                                  |                                              |

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
