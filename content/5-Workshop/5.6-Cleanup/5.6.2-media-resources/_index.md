---
title: "Clean up media and automation resources"
date: 2026-07-15
weight: 2
chapter: false
pre: " <b> 5.6.2. </b> "
---

#### Resources to check

* S3 bucket `netflop-input-source`
* S3 bucket `netflop-output-source`
* Unused CloudFront distributions
* Unused MediaConvert jobs/templates
* Lambda `netflop-mediaconvert-notifier`
* Lambda `netflop-subtitle-converter`
* EventBridge rule `netflop-mediaconvert-job-state-change`
* IAM roles/policies for MediaConvert and Lambda

#### Cleanup steps

1. Back up videos/HLS/subtitles if needed.
2. Empty S3 buckets before deletion.
3. Disable/delete unused CloudFront distributions.
4. Delete unused Lambda functions.
5. Delete unused EventBridge rules.
6. Review IAM roles and policies.

![CloudFront](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/5.4.3-cloudfront-hls/cloudfront1.png)
![MediaConvert](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/5.4.2-mediaconvert/mediaconvert.png)

