---
title: "Week 8 Worklog"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Topic: Integrate admin media upload to S3

### Week Objectives

* Allow admin to upload videos, images, and subtitles to S3 instead of EC2.
* Prepare metadata for backend MediaConvert jobs.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Studied AWS SDK for JavaScript v3 with S3 client | Backend could call S3 APIs | AWS SDK JS v3 S3: <https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/javascript_s3_code_examples.html> |
| 2 | Integrated poster, avatar, and banner uploads to S3 output | Images were stored on S3 and URLs saved in database | S3 PutObject: <https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html> |
| 3 | Designed multipart upload for large videos | Avoided timeout issues for large video uploads | S3 Multipart Upload: <https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html> |
| 4 | Saved episode metadata: S3 input path, upload status, movieId, episodeId | Prepared input for MediaConvert | Express Middleware: <https://expressjs.com/en/resources/middleware.html> |

### Achievements

* Built the admin media upload flow to S3.
* Backend stored file information and processing status.
* Reduced dependency on EC2 disk for large videos.


