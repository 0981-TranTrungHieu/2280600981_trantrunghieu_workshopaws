---
title: "Week 9 Worklog"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Topic: Integrate AWS Elemental MediaConvert for HLS video processing

### Week Objectives

* Automatically convert MP4/MKV videos from S3 input to multi-quality HLS in S3 output.
* Store video processing status for frontend/admin tracking.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Studied MediaConvert jobs, inputs, output groups, and endpoints | Understood video encoding job structure | MediaConvert User Guide: <https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html> |
| 2 | Created IAM role for MediaConvert to access S3 input/output | MediaConvert could read source videos and write HLS output | MediaConvert IAM: <https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html> |
| 3 | Created backend job for HLS 360p/480p/720p/1080p | Videos were converted to HLS | MediaConvert HLS: <https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html> |
| 4 | Saved `jobId`, `hls_url`, `cloudfront_url`, and `upload_status` to database | Admin could track episode processing status | AWS SDK MediaConvert: <https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/client/mediaconvert/> |

### Achievements

* Built a media pipeline from S3 input to HLS output.
* Understood why MediaConvert was selected instead of running FFmpeg on EC2.
* Prepared HLS data for CloudFront streaming.


