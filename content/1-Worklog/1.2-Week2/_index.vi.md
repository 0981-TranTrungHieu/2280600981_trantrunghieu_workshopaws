---
title: "Worklog Tuần 2"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Chủ đề: IAM, AWS CLI, bảo mật tài khoản và kiểm soát chi phí

### Mục tiêu tuần 2

* Thiết lập quyền truy cập AWS an toàn cho quá trình triển khai.
* Biết sử dụng AWS CLI để kiểm tra tài nguyên và hỗ trợ deploy.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tìm hiểu IAM user, group, role, policy và nguyên tắc least privilege | Hiểu cách cấp quyền cho EC2, S3, Lambda, MediaConvert | IAM User Guide: <https://docs.aws.amazon.com/IAM/latest/UserGuide/> |
| 2 | Cài đặt và cấu hình AWS CLI trên máy local | Có thể gọi lệnh AWS CLI để kiểm tra account/region/service | AWS CLI Docs: <https://docs.aws.amazon.com/cli/latest/userguide/> |
| 3 | Bật MFA, rà soát access key và quyền admin/deploy | Giảm rủi ro lộ thông tin truy cập | IAM Security Best Practices: <https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html> |
| 4 | Tìm hiểu Billing Dashboard, AWS Budgets và cảnh báo chi phí | Có kế hoạch kiểm soát chi phí khi dùng EC2, RDS, S3, MediaConvert | AWS Budgets: <https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html> |

### Kết quả đạt được

* Biết cách cấu hình quyền và profile AWS CLI cho dự án.
* Nắm được các rủi ro bảo mật khi dùng access key.
* Chuẩn bị được nền tảng bảo mật và chi phí trước khi tạo tài nguyên thật.

