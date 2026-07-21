---
title: "Worklog Tuần 9"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Chủ đề: Tích hợp AWS Elemental MediaConvert để chuyển video sang HLS

### Mục tiêu tuần 9

* Tự động chuyển video MP4/MKV từ S3 input sang HLS nhiều chất lượng trong S3 output.
* Lưu trạng thái xử lý video để frontend/admin theo dõi.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tìm hiểu MediaConvert job, input, output group và endpoint | Hiểu cấu trúc job encode video | MediaConvert User Guide: <https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html> |
| 2 | Tạo IAM role cho MediaConvert truy cập S3 input/output | MediaConvert có quyền đọc video gốc và ghi HLS | MediaConvert IAM: <https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html> |
| 3 | Backend tạo job HLS 360p/480p/720p/1080p | Video được chuyển sang HLS | MediaConvert HLS: <https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html> |
| 4 | Lưu `jobId`, `hls_url`, `cloudfront_url`, `upload_status` vào database | Admin theo dõi được trạng thái tập phim | AWS SDK MediaConvert: <https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/client/mediaconvert/> |

### Kết quả đạt được

* Tạo được media pipeline từ S3 input sang HLS output.
* Hiểu lý do chọn MediaConvert thay vì tự chạy FFmpeg trên EC2.
* Chuẩn bị được dữ liệu để phát video qua CloudFront.

