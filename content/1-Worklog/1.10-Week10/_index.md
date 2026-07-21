---
title: "Week 10 Worklog"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Topic: Deliver video with CloudFront and protect streams

### Week Objectives

* Stream HLS through CloudFront instead of direct S3 access.
* Study stream protection using signed cookies or signed URLs.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Created CloudFront distribution with S3 output as origin | HLS had a CDN endpoint for video playback | CloudFront Developer Guide: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| 2 | Configured HTTPS, cache behavior, and HLS paths | Player loaded `m3u8` and `.ts` segments more reliably | CloudFront Cache Behavior: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/DownloadDistValuesCacheBehavior.html> |
| 3 | Integrated VideoPlayer to play HLS from CloudFront | Users could watch movies on the website | hls.js Docs: <https://github.com/video-dev/hls.js/> |
| 4 | Studied signed cookies through `/api/stream/session` | Prepared a direction for protecting non-public video streams | CloudFront Signed Cookies: <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-signed-cookies.html> |

### Achievements

* Delivered HLS video through CloudFront.
* Understood CDN benefits for a movie streaming website.
* Prepared a stream protection approach using signed cookies.


