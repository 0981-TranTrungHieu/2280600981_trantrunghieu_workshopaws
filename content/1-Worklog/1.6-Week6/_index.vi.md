---
title: "Worklog Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Chủ đề: Thiết kế S3 input/output cho video, ảnh và phụ đề

### Mục tiêu tuần 6

* Tách media khỏi EC2 bằng Amazon S3.
* Thiết kế cấu trúc bucket cho video gốc, HLS output, poster, avatar và phụ đề.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tạo bucket `netflop-input-source` cho video/phụ đề gốc | Có nơi lưu file upload ban đầu | S3 User Guide: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/> |
| 2 | Tạo bucket `netflop-output-source` cho HLS, ảnh, avatar, phụ đề VTT | Có nơi lưu output phục vụ website | S3 Bucket Overview: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingBucket.html> |
| 3 | Thiết kế key prefix `movies/{movieId}/episodes/{episodeId}/...` | Media được tổ chức theo phim/tập rõ ràng | S3 Object Keys: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-keys.html> |
| 4 | Tìm hiểu bucket policy, CORS và Block Public Access | Chuẩn bị cho upload từ backend/admin và phát qua CloudFront | S3 CORS: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html> |

### Kết quả đạt được

* Có thiết kế lưu trữ media rõ ràng cho Netflop.
* Hiểu vì sao không nên lưu video lớn trực tiếp trên EC2.
* Chuẩn bị được nền tảng cho upload video và HLS output.

