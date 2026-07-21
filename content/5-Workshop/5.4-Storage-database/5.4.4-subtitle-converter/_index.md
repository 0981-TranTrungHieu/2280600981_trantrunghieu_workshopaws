---
title: "Configure subtitle converter Lambda"
date: 2026-07-13
weight: 4
chapter: false
pre: " <b> 5.4.4. </b> "
---

Lambda `netflop-subtitle-converter` converts `.srt` subtitles into `.vtt`.

```text
Admin upload .srt -> S3 input subtitle-input/ -> Lambda -> S3 output subtitles/*.vtt -> Player
```

#### Checking steps

1. Upload `.srt` from admin page.
2. Confirm file appears in `netflop-input-source/subtitle-input/`.
3. Check Lambda logs.
4. Confirm `.vtt` file appears in S3 output.
5. Open video player and enable subtitles.

![Input subtitle](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/inputsub.png)
![Lambda subtitle](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/lamda.png)
![Output subtitle](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.4-Storage-database/outputsub.png)

