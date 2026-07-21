---
title: "Week 4 Worklog"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Topic: Deploy EC2, Nginx, Node.js API, and React frontend

### Week Objectives

* Run the Netflop application on EC2.
* Configure Nginx reverse proxy for frontend and backend.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Launched Linux EC2, connected by SSH, and updated packages | EC2 was ready for runtime installation | EC2 Getting Started: <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html> |
| 2 | Installed Node.js, npm, PM2, and cloned Netflop source code | Backend could run under PM2 | PM2 Docs: <https://pm2.keymetrics.io/docs/usage/quick-start/> |
| 3 | Built React frontend and configured Nginx to serve static files | Frontend was served through the web server | Nginx Docs: <https://nginx.org/en/docs/> |
| 4 | Configured reverse proxy from `/api` to the Node.js backend | Frontend could call backend APIs | Nginx Reverse Proxy: <https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/> |

### Achievements

* Ran the basic Netflop web application on EC2.
* Used PM2 to manage the Node.js backend.
* Configured Nginx for frontend hosting and API proxying.


