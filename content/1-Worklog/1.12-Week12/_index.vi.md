---
title: "Worklog Tuần 12"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Chủ đề: Monitoring, kiểm thử, cleanup và hoàn thiện báo cáo

### Mục tiêu tuần 12

* Kiểm thử toàn bộ luồng Netflop từ truy cập web đến upload, convert và phát video.
* Hoàn thiện báo cáo workshop, blog, event và worklog.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Cấu hình CloudWatch Logs/Metrics cho EC2, RDS, Lambda | Theo dõi được log và chỉ số vận hành | CloudWatch Docs: <https://docs.aws.amazon.com/cloudwatch/> |
| 2 | Tạo SNS topic/alarm cho lỗi hoặc tài nguyên quan trọng | Có hướng cảnh báo khi hệ thống bất thường | SNS Docs: <https://docs.aws.amazon.com/sns/> |
| 3 | Kiểm thử end-to-end: admin upload video, MediaConvert xử lý, CloudFront phát HLS | Xác nhận luồng chính hoạt động | AWS Well-Architected Reliability: <https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/> |
| 4 | Rà soát cleanup, chi phí, hình ảnh minh họa và nội dung báo cáo | Báo cáo hoàn thiện và giảm rủi ro phát sinh phí | AWS Cost Management: <https://docs.aws.amazon.com/cost-management/> |

### Kết quả đạt được

* Hoàn thiện luồng demo chính của website Netflop trên AWS.
* Có monitoring/cảnh báo cơ bản cho EC2, RDS, Lambda và chi phí.
* Hoàn thiện nội dung worklog, workshop và báo cáo cuối kỳ.

