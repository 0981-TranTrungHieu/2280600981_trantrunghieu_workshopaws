---
title: "Worklog Tuần 3"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Chủ đề: Thiết kế mạng VPC, Security Group và EC2

### Mục tiêu tuần 3

* Thiết kế lớp network cho Netflop để EC2 public phục vụ web và RDS được kiểm soát truy cập.
* Hiểu cách Security Group ảnh hưởng đến SSH, HTTP/HTTPS và MySQL.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tìm hiểu VPC, subnet, route table, Internet Gateway | Hiểu luồng truy cập từ internet vào EC2 | VPC User Guide: <https://docs.aws.amazon.com/vpc/latest/userguide/> |
| 2 | Thiết kế Security Group cho EC2: SSH, HTTP, HTTPS | Có rule phục vụ deploy và truy cập website | EC2 Security Groups: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html> |
| 3 | Thiết kế Security Group cho RDS chỉ cho EC2/backend truy cập MySQL | Giảm rủi ro mở database public | RDS Security: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.html> |
| 4 | Lên cấu hình EC2 `t3.micro`, key pair, EBS và Elastic IP/domain | Chuẩn bị hạ tầng chạy web Netflop | EC2 User Guide: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/> |

### Kết quả đạt được

* Xác định được network baseline cho Netflop.
* Hiểu cách mở port đúng nhu cầu thay vì mở rộng toàn bộ.
* Chuẩn bị được cấu hình EC2 và security group để triển khai ứng dụng.

