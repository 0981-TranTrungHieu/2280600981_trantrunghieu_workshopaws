---
title: "Worklog Tuần 10"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Chủ đề: Phân phối video bằng CloudFront và bảo vệ stream

### Mục tiêu tuần 10

* Phát HLS ổn định thông qua CloudFront thay vì truy cập trực tiếp S3.
* Tìm hiểu cơ chế bảo vệ video bằng signed cookies/signed URL.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tạo CloudFront distribution trỏ đến S3 output | HLS có CDN endpoint để phát video | CloudFront Developer Guide: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 2 | Cấu hình HTTPS, cache behavior và path cho HLS segment | Player tải `m3u8` và `.ts` ổn định hơn | CloudFront Cache Behavior: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/DownloadDistValuesCacheBehavior.html> |
| 3 | Tích hợp VideoPlayer phát HLS từ CloudFront | Người dùng xem được phim trên web | hls.js Docs: <https://github.com/video-dev/hls.js/> |
| 4 | Tìm hiểu signed cookies qua endpoint `/api/stream/session` | Có hướng bảo vệ stream không public toàn bộ video | CloudFront Signed Cookies: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-signed-cookies.html> |

### Kết quả đạt được

* Video HLS được phát qua CloudFront.
* Hiểu lợi ích CDN cho website xem phim.
* Có cơ chế định hướng bảo vệ nội dung video bằng signed cookies.

