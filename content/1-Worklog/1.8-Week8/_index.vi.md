---
title: "Worklog Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Chủ đề: Tích hợp upload media từ admin lên S3

### Mục tiêu tuần 8

* Cho phép admin upload video, ảnh và phụ đề lên S3 thay vì lưu trên EC2.
* Chuẩn bị metadata để backend tạo MediaConvert job.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tìm hiểu AWS SDK for JavaScript v3 với S3 client | Backend có thể gọi S3 API | AWS SDK JS v3 S3: <https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/javascript_s3_code_examples.html> |
| 2 | Tích hợp upload poster, avatar và banner lên S3 output | File ảnh lưu trên S3, database lưu URL | S3 PutObject: <https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html> |
| 3 | Thiết kế multipart upload cho video lớn | Tránh lỗi timeout khi upload video dung lượng cao | S3 Multipart Upload: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html> |
| 4 | Lưu metadata tập phim: S3 input path, trạng thái upload, movieId, episodeId | Chuẩn bị input cho MediaConvert | Express File Upload Patterns: <https://expressjs.com/en/resources/middleware.html> |

### Kết quả đạt được

* Admin có luồng upload media lên S3.
* Backend lưu được thông tin file và trạng thái xử lý.
* Giảm phụ thuộc vào ổ đĩa EC2 khi xử lý video lớn.

