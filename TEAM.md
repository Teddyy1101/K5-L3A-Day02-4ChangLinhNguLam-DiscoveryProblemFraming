# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: 4ChangLinhNguLam
- Candidate problem nhóm chọn (1 câu): Khi khách đổi một logic đã chốt từ 3–4 tháng trước, team BA/PO + dev không tìm lại được lý do và ràng buộc ngầm của quyết định cũ, dẫn tới mất thời gian tra cứu và rủi ro sửa sai gây hồi quy.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Huy Thứ | 2A202603356 | Phụ trách kiểm chứng, research | Teddyy1101 |
| 2 | Khuất Duy Hiếu | 2A202603383 | Điều phối thời gian, Người phản biện chính, Phụ trách research, Phân tích | KhuatHieu |
| 3 | Nguyễn Ngọc Minh Đức | 2A202603421 | Viết problem statement | MinhDuck512 |
| 4 | Nguyễn Hữu Đức | 2A202603429 | Vẽ quy trình | ducnguyen2112 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Khuất Duy Hiếu | Nguyễn Huy Thứ | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Huy Thứ | Khuất Duy Hiếu | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Huy Thứ | Khuất Duy Hiếu | Bảng research có link |
| CP5 — Quy trình trước/sau | Nguyễn Hữu Đức | Khuất Duy Hiếu | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Nguyễn Hữu Đức | Khuất Duy Hiếu | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Ngọc Minh Đức | Khuất Duy Hiếu | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Nguyễn Ngọc Minh Đức | Nguyễn Huy Thứ | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### Nguyễn Huy Thứ - 2A202603356

**Phần việc phụ trách:**

- Điều phối thời gian và theo dõi tiến độ công việc của nhóm
- Phụ trách CP4: xây dựng Assumption Map, kiểm chứng các giả định và research giải pháp hiện có

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Xác định các giả định quan trọng liên quan đến vấn đề nhóm lựa chọn
- Tìm hiểu các công cụ như Jira/Confluence Decision Log, Atlassian Rovo và Slack AI
- Tổng hợp ưu điểm, hạn chế và khả năng áp dụng của từng công cụ
- Đề xuất cần kiểm chứng bằng dữ liệu thực tế trước khi quyết định xây dựng giải pháp AI riêng

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Phần CP3 - Đóng góp ý kiến thảo luận chọn pitch
- Phần CP4 – Assumption Map
- Phần CP4 – Kiểm chứng và Research giải pháp hiện có trong `group_report.md`
- Commit: 261eec32936fe09cd39e2d4edd3d8f5c21b87f00

**Điều mình học được từ phần nhóm:**

- Biết cách phân biệt giả định và thông tin đã được kiểm chứng
- Hiểu rằng cần tìm hiểu các giải pháp hiện có trước khi đề xuất xây dựng một hệ thống mới
- Nhận ra AI không phải lúc nào cũng là lựa chọn tốt nhất, cần đánh giá hiệu quả thực tế và tính cần thiết trước khi áp dụng

### Khuất Duy Hiếu - 2A202603383

**Phần việc phụ trách:**

- Người chính CP3 (hội tụ nhóm), hỗ trợ CP4, CP5, CP6 theo bảng phân công ở trên
- Người phản biện chính khi pitch; cung cấp candidate #1 (nguồn từ team thật của mình) mà nhóm đã chọn

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hoàn thành CP1 (5 problem dạng Job Story) và CP2 (3 Problem Card kèm quy trình nháp) trong báo cáo cá nhân
- Pitch 3 candidate (#1, #2, #3) trong CP3; candidate #1 được nhóm chọn
- Đặt câu hỏi phản biện cho candidate #4, #6, #8, #9 của các bạn trong bảng pitch
- Làm file pitch card HTML cho Card #1 (`report/assets/pitch_card1_KhuatDuyHieu.html`)
- Merge các nhánh của thành viên vào nhánh chung
- Là 1 dev trong team dự án app ERP: phỏng vấn thực tế 5 thành viên (3 dev, 2 BA/PO); ghi nhận cú call Slack 45 phút từng dẫn đến 3 ca rework và năm nay tình trạng này đã xảy ra 2 lần.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (pitch và câu hỏi phản biện), mục 2.4 (candidate được chọn)
- `report/individual/2A202603383_KhuatDuyHieu.md` mục 2–3
- `report/assets/pitch_card1_KhuatDuyHieu.html`
- Commit: 59fcac4, 1cfa963, 359f736, b22839a, 376caf6
- Ca Slack chỉ ghi ở báo cáo cá nhân mục 4, không ghi thành snapshot trong `group_report.md` mục 3.2

**Điều mình học được từ phần nhóm:**

- #1 hòa điểm với cụm B nhưng được chọn vì hậu quả nặng hơn; dù team app ERP từng trải qua 3 ca rework sau cú call Slack 45 phút (năm nay lặp lại 2 lần), nhưng việc chuẩn hóa quy trình ghi chép thủ công (No AI) vẫn là ưu tiên số một trước khi tính đến AI.
- Gom cluster cho thấy #2 và #3 của mình cùng một pain mất ngữ cảnh với #1. Chatbot, glossary, script là solution; nếu không gạch khỏi cây OST thì nhóm đang chọn công cụ trước khi hiểu pain.
- Research của Thứ (Decision Log, Rovo, Slack AI) và ca Slack mình chứng kiến cùng chỉ về một chỗ: chưa đủ bằng chứng để xây AI. Not Yet là quyết định đúng với dữ liệu đang có, không phải bước lùi.
