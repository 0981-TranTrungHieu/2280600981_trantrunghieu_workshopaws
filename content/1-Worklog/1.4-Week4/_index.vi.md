---
title: "Worklog Tuần 4"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Chủ đề: Triển khai EC2, Nginx, Node.js API và React frontend

### Mục tiêu tuần 4

* Đưa ứng dụng Netflop chạy được trên EC2.
* Cấu hình Nginx reverse proxy cho frontend/backend.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Khởi tạo EC2 Linux, SSH vào server và cập nhật package | EC2 sẵn sàng cài runtime | EC2 Getting Started: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html> |
| 2 | Cài Node.js, npm, PM2 và clone source Netflop | Backend có thể chạy bằng PM2 | PM2 Docs: <https://pm2.keymetrics.io/docs/usage/quick-start/> |
| 3 | Build React frontend và cấu hình Nginx serve static files | Frontend hiển thị qua web server | Nginx Docs: <https://nginx.org/en/docs/> |
| 4 | Cấu hình reverse proxy `/api` về Node.js backend | Frontend gọi được API backend | Nginx Reverse Proxy: <https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/> |

### Kết quả đạt được

* Netflop chạy được ở mức ứng dụng web cơ bản trên EC2.
* Biết cách dùng PM2 để quản lý Node.js backend.
* Cấu hình được Nginx phục vụ frontend và proxy API.

