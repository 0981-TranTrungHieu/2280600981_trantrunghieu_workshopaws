---
title: "Worklog Tuần 5"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Chủ đề: Thiết kế database và triển khai Amazon RDS MySQL

### Mục tiêu tuần 5

* Chuyển database của Netflop sang Amazon RDS MySQL.
* Kết nối backend Node.js đến database và kiểm tra dữ liệu phim.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Phân tích schema database `web_xem_phim_final` | Nắm bảng phim, tập phim, tài khoản, bình luận, lịch sử xem | MySQL Docs: <https://dev.mysql.com/doc/> |
| 2 | Tạo RDS MySQL `netflop-db` và cấu hình storage/backup | Có database managed thay cho MySQL local | RDS MySQL Docs: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MySQL.html> |
| 3 | Import dữ liệu và kiểm tra kết nối từ EC2/backend | Backend đọc/ghi được dữ liệu từ RDS | RDS Connectivity: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ConnectToInstance.html> |
| 4 | Rà soát security group RDS và biến môi trường database | Giảm lỗi kết nối và tránh lộ thông tin DB | Node.js Environment Variables: <https://nodejs.org/en/learn/command-line/how-to-read-environment-variables-from-nodejs> |

### Kết quả đạt được

* RDS MySQL hoạt động và lưu dữ liệu chính của Netflop.
* Backend kết nối được đến database trên AWS.
* Hiểu cách quản lý cấu hình database bằng biến môi trường.

