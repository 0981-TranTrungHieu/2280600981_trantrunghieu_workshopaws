---
title: "Week 5 Worklog"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Topic: Database design and Amazon RDS MySQL deployment

### Week Objectives

* Move the Netflop database to Amazon RDS MySQL.
* Connect the Node.js backend to RDS and verify movie data.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Analyzed the `web_xem_phim_final` database schema | Understood movie, episode, account, comment, and watch history tables | MySQL Docs: <https://dev.mysql.com/doc/> |
| 2 | Created RDS MySQL `netflop-db` and configured storage/backup | Had a managed database instead of local MySQL | RDS MySQL Docs: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MySQL.html> |
| 3 | Imported data and tested EC2/backend connectivity to RDS | Backend could read/write data from RDS | RDS Connectivity: <https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ConnectToInstance.html> |
| 4 | Reviewed RDS Security Group and database environment variables | Reduced connection issues and avoided exposing DB credentials | Node.js Environment Variables: <https://nodejs.org/en/learn/command-line/how-to-read-environment-variables-from-nodejs> |

### Achievements

* RDS MySQL stored the main Netflop data.
* Backend connected successfully to the AWS database.
* Managed database configuration through environment variables.


