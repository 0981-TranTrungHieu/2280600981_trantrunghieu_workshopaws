---
title: "Test admin video upload"
date: 2026-07-14
weight: 3
chapter: false
pre: " <b> 5.5.3. </b> "
---

#### Upload flow

1. Admin signs in to the admin page.
2. Admin selects a movie/episode.
3. Admin selects an MP4/MKV video file.
4. Backend receives multipart upload request.
5. Video is uploaded to `netflop-input-source`.
6. Backend creates a MediaConvert job.
7. MediaConvert writes HLS output to `netflop-output-source`.
8. EventBridge receives COMPLETE.
9. Lambda `netflop-mediaconvert-notifier` calls backend webhook.
10. Backend updates episode `upload_status` to ready.

#### Backend values to check

* `jobId`
* `hls_url`
* `cloudfront_url`
* `upload_status`

![Admin input](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.3-admin-upload-video/adminin1.png)
![Admin upload](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.3-admin-upload-video/adminput1.png)
![Upload progress](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.3-admin-upload-video/adminup1.png)
![Upload processing](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.3-admin-upload-video/adminup2.png)
![Upload complete](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.3-admin-upload-video/adminup3.png)

