---
title: "Week 6 Worklog"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Topic: S3 input/output design for videos, images, and subtitles

### Week Objectives

* Move media storage away from EC2 using Amazon S3.
* Design bucket structure for source videos, HLS output, posters, avatars, and subtitles.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Created `netflop-input-source` for original videos and subtitle input | Prepared storage for raw uploads | S3 User Guide: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/> |
| 2 | Created `netflop-output-source` for HLS, images, avatars, and VTT subtitles | Prepared storage for website-ready outputs | S3 Bucket Overview: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingBucket.html> |
| 3 | Designed key prefix `movies/{movieId}/episodes/{episodeId}/...` | Organized media clearly by movie and episode | S3 Object Keys: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-keys.html> |
| 4 | Studied bucket policy, CORS, and Block Public Access | Prepared upload and CloudFront delivery configuration | S3 CORS: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html> |

### Achievements

* Designed clear media storage for Netflop.
* Understood why large videos should not be stored directly on EC2.
* Prepared the base for video upload and HLS output.


