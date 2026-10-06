# AI Support Log — Day 20

| Thông tin | Nội dung |
|---|---|
| Người nộp | Hoàng Quốc Dũng |
| Mã học viên | 2A202602523 |
| Ngày | 06/10/2026 |
| Công cụ | Codex |
| Dự án | Campus 24/7 — EDU-14 / P-120 |
| Persona do người nộp chọn | Cán bộ học vụ tiếp nhận và xử lý yêu cầu sinh viên |
| Đầu ra | [README.md — Metrics Pack](README.md#metrics-pack) |

## 1. Các yêu cầu và phản hồi trong phiên

| Lượt | Yêu cầu / phản hồi | AI hỗ trợ |
|---|---|---|
| 1 | Cung cấp brief Day 20, hỏi áp dụng thế nào cho dự án khiếu nại/xin giấy tờ. | Giải thích các phase và hồ sơ nộp. |
| 2 | Yêu cầu đọc bản sao `P-120` để nắm dự án, phân biệt với bài lab cá nhân. | Đọc tài liệu nghiệp vụ và mã nguồn, xem năm wireframe; xác định Campus 24/7. |
| 3 | Hoàn thiện README và AI log; cấm sửa `P-120`, không nộp thư mục đó. | Soạn bản đề xuất đầu tiên ở root; đã chọn persona sinh viên chưa đúng ý người nộp. |
| 4 | Người nộp muốn tự làm từng phase và yêu cầu câu trả lời ngắn. | Gợi ý Phase 0, ban đầu vẫn chọn sai persona. |
| 5 | Người nộp xác định cán bộ là người dùng chính của use case. | Sửa persona và core job đề xuất sang cán bộ học vụ. |
| 6 | Người nộp giải thích: sinh viên xin giấy có mẫu sẵn; AI điền để cán bộ chỉ đọc lại. | Làm rõ hướng sản phẩm: giảm nhập liệu, cán bộ kiểm tra/duyệt bản giấy điền sẵn. |
| 7 | “oke sửa lại hết 2 file kia đi, xong rồi hướng dẫn làm phase 1”. | Viết lại toàn bộ Metrics Pack theo cán bộ; cập nhật log và hướng dẫn Phase 1. |

## 2. Quyết định và thông tin do người nộp cung cấp

- Dự án: Campus 24/7, trợ lý hỗ trợ xử lý yêu cầu học vụ.
- Persona chính của bài lab: cán bộ học vụ tiếp nhận và xử lý yêu cầu sinh viên.
- Luồng sản phẩm được làm rõ: sinh viên xin giấy; có format/mẫu; AI điền sẵn; cán bộ đọc lại.
- Người nộp đồng ý phần diễn đạt Phase 0: cán bộ muốn duyệt giấy nhanh, đúng thông tin, giảm nhập liệu thủ công.
- Người nộp muốn tự hoàn thiện từng phase.
- Giới hạn: chỉ sửa README và AI log; `P-120` chỉ để đọc, không nộp.

`File_tu_viet.md` do người nộp đang viết xác nhận tên dự án và persona cán bộ. AI chỉ đọc để đối chiếu, không chỉnh sửa tệp này.

## 3. AI đã đề xuất gì ở bản sửa

- Giới hạn use case giấy xác nhận sinh viên; không gộp khiếu nại/đặt phòng.
- Ứng viên core action: cán bộ kiểm tra, chỉnh sửa nếu cần và xác nhận bản giấy AI điền đúng, đủ.
- Core Action Card, bảng bốn khái niệm và tự kiểm năm tiêu chí.
- Cadence theo ca có hồ sơ; retention cán bộ ở ca có công việc tiếp theo.
- Activation lần duyệt đầu; engagement sản lượng theo workload và tỷ lệ không sửa tay.
- NSM giấy được duyệt theo checklist, có theo dõi lỗi sau duyệt; leading thời gian thao tác và counter công sửa/lỗi.
- Loop workflow hai chu kỳ; metric hypothesis; bảy event và tiêu chí nghiệm thu.
- Cách đo ca có cơ hội xử lý từ lịch/phân công; phân biệt thời gian chờ với thao tác chủ động.

Các mốc 7 ngày theo dõi lỗi, 30 ngày theo dõi quay lại, cửa sổ activation theo ca và quality threshold là đề xuất đo lường. Chưa được kiểm chứng bằng dữ liệu, không phải SLA đã cam kết.

## 4. Kiểm chứng và chỉnh sửa có bằng chứng

| Nội dung | Bằng chứng / nguồn | Kết quả |
|---|---|---|
| AI hiểu sai persona | Người nộp phản hồi cán bộ là người dùng chính. | Bỏ góc nhìn sinh viên của bản đầu; viết lại toàn bộ chuỗi metric theo cán bộ. |
| AI chưa hiểu đúng lợi ích | Người nộp giải thích AI điền sẵn giấy theo mẫu. | Chuyển trọng tâm sang giảm nhập liệu và kiểm tra bản giấy. |
| Tránh coi output AI là value đã xảy ra | Framework của brief Day 20. | Bản nháp điền sẵn là đầu vào; event value đề xuất cần hành vi kiểm tra/xác nhận của cán bộ. |
| Không suy ra tính năng đã triển khai | Mã nguồn hiện có còn khung mẫu; mô tả mới do người nộp cung cấp. | Ghi rõ hướng sản phẩm và hợp đồng tracking đề xuất, chưa tuyên bố chạy được. |
| Phân biệt duyệt với cấp giấy | Tài liệu nghiệp vụ và giới hạn chưa xác nhận phát hành. | Duyệt là xác nhận nội dung cho bước tiếp theo; không coi là đã ký/phát hành/nhận giấy. |
| Giới hạn chỉnh sửa | Người nộp cấm sửa `P-120`. | Chỉ cập nhật hai file bài lab; không sửa dự án nhóm hoặc file người nộp tự viết. |

Chưa có khảo sát cán bộ, baseline điền tay, số liệu tiết kiệm thời gian, kết quả thử loop hoặc nghiệm thu tracking trong phiên.

## 5. Quy định sử dụng AI và trạng thái quyết định

Brief cho phép AI brainstorm ứng viên core action, phản biện retention và gợi ý event. Người học phải tự chọn core action, kết luận cadence và metric hypothesis.

AI đã hỗ trợ viết một bản đề xuất đầy đủ, gồm cả phương án cho các quyết định lõi. Phạm vi này được khai báo; không ghi các đề xuất như quyết định cá nhân đã chốt.

| Quyết định | Trạng thái |
|---|---|
| Persona cán bộ | Người nộp đã xác định trực tiếp. |
| Luồng AI điền mẫu để cán bộ đọc lại | Người nộp đã giải thích trực tiếp. |
| Diễn đạt Phase 0 | Người nộp đã đồng ý trước khi yêu cầu sửa tài liệu. |
| Core action và completion rule | AI đề xuất; người nộp đang tự làm Phase 1, chưa chốt. |
| Kết luận cadence | AI đề xuất; người nộp cần tự chốt Phase 2. |
| Metric hypothesis | AI đề xuất; người nộp cần tự chốt Phase 4. |
| Ngưỡng và định nghĩa metric | Bản thiết kế thử nghiệm, cần rà soát và đo thực tế. |

Khi người nộp chọn/sửa một phương án, cập nhật lựa chọn và lý do thực tế vào log; không tự ghi đã kiểm chứng hoặc đã duyệt khi chưa xảy ra.

## 6. Nguồn và bàn giao

- Nguồn: brief Day 20 do người dùng cung cấp; tài liệu Campus 24/7 trong bản sao `P-120`; phản hồi làm rõ của người nộp và Phase 0 đang viết.
- Đầu ra cập nhật: `README.md`, `ai-support-log.md` ở root repository cá nhân.
- `P-120` giữ nguyên, chỉ dùng tham khảo và không thuộc bộ hồ sơ nộp.
- Không chạy thử sản phẩm, triển khai tracking, gửi khảo sát, commit hoặc push trong lượt sửa này.
- Link GitHub và quyền xem chưa được kiểm chứng.
