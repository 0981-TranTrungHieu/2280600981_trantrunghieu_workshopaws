---
title: "Worklog Tuần 7"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Chủ đề: Phân tích chức năng Netflop và thiết kế luồng frontend/backend

### Mục tiêu tuần 7

* Phân tích code Netflop để xác định các API và màn hình cần triển khai.
* Thiết kế luồng người dùng và admin trước khi tích hợp media pipeline.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Đọc source React frontend và Node.js backend | Nắm module phim, tập phim, user, admin, upload | GitHub Netflop: <https://github.com/Danh0104/Web-xem-phim-Netflop.git> |
| 2 | Xác định luồng user: danh sách phim, tìm kiếm, chi tiết, xem phim, phụ đề | Có flow người dùng cuối | React Docs: <https://react.dev/learn> |
| 3 | Xác định luồng admin: upload phim, poster, tập phim, phụ đề | Có flow quản trị nội dung | Express Docs: <https://expressjs.com/> |
| 4 | Mapping frontend/backend với AWS: RDS, S3, MediaConvert, CloudFront | Có bản thiết kế tích hợp dịch vụ | AWS Architecture Center: <https://aws.amazon.com/architecture/> |

### Kết quả đạt được

* Hiểu cấu trúc ứng dụng Netflop ở mức code và chức năng.
* Xác định được điểm tích hợp giữa backend API và AWS services.
* Chuẩn bị được luồng triển khai upload media ở tuần tiếp theo.

