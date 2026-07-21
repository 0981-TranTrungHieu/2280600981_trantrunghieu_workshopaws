---
title: "Configure CloudFront HLS streaming"
date: 2026-07-13
weight: 3
chapter: false
pre: " <b> 5.4.3. </b> "
---

CloudFront distribution `d11jdx7259stge.cloudfront.net` delivers HLS streams from S3 output to the video player.

```text
Frontend -> Backend movie/episode info
Backend -> /api/stream/session signed cookies
Video Player -> CloudFront -> S3 output HLS
```

#### Checking steps

1. Open CloudFront console.
2. Check distribution `d11jdx7259stge.cloudfront.net` is Enabled.
3. Check origin points to S3 output.
4. Open a movie episode in Netflop.
5. Confirm the player streams HLS through CloudFront.

![CloudFront](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/5.4.3-cloudfront-hls/cloudfront1.png)
![CloudFront detail](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/5.4.3-cloudfront-hls/cf2.png)
![Player](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/5.4.3-cloudfront-hls/player1.png)

