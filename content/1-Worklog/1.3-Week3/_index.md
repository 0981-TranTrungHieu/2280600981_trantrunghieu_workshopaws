---
title: "Week 3 Worklog"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Topic: VPC, Security Groups, and EC2 network design

### Week Objectives

* Design the network layer for Netflop with public EC2 and controlled RDS access.
* Understand how Security Groups affect SSH, HTTP/HTTPS, and MySQL access.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Studied VPC, subnets, route tables, and Internet Gateway | Understood traffic flow from the internet to EC2 | VPC User Guide: <https://docs.aws.amazon.com/vpc/latest/userguide/> |
| 2 | Designed EC2 Security Group rules for SSH, HTTP, and HTTPS | Prepared rules for deployment and website access | EC2 Security Groups: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html> |
| 3 | Designed RDS Security Group to allow MySQL access only from EC2/backend | Reduced database public exposure risk | RDS Security: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.html> |
| 4 | Planned EC2 t3.micro, key pair, EBS, and Elastic IP/domain setup | Prepared infrastructure for running Netflop | EC2 User Guide: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/> |

### Achievements

* Defined the network baseline for Netflop.
* Understood how to open only required ports.
* Prepared EC2 and Security Group configuration for deployment.


