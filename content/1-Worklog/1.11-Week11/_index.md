---
title: "Week 11 Worklog"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Topic: Automation with Lambda, EventBridge, and subtitle processing

### Week Objectives

* Automatically update episode status after MediaConvert completes.
* Convert `.srt` subtitles to `.vtt` for the video player.

### Work Completed

| Day | Work | Result | Reference |
| --- | --- | --- | --- |
| 1 | Created EventBridge rule for MediaConvert job state changes | Received COMPLETE/ERROR/CANCELED events | EventBridge Docs: <https://docs.aws.amazon.com/eventbridge/latest/userguide/> |
| 2 | Built Lambda `netflop-mediaconvert-notifier` to call backend webhook | Backend automatically updated episode status | Lambda Developer Guide: <https://docs.aws.amazon.com/lambda/latest/dg/welcome.html> |
| 3 | Tested webhook `/api/uploads/mediaconvert/events` | Episode status changed to ready after encoding | Express Routing: <https://expressjs.com/en/guide/routing.html> |
| 4 | Built subtitle converter Lambda from `.srt` to `.vtt` | Subtitles could be displayed in the player | WebVTT: <https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API> |

### Achievements

* Converted the media pipeline to an event-driven flow.
* Episode status was updated automatically after MediaConvert completed.
* SRT subtitles were converted to VTT for web playback.


