---
title: "Worklog Tuần 11"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Chủ đề: Tự động hóa bằng Lambda, EventBridge và xử lý phụ đề

### Mục tiêu tuần 11

* Tự động cập nhật trạng thái tập phim sau khi MediaConvert hoàn tất.
* Chuyển phụ đề `.srt` sang `.vtt` để hiển thị trên video player.

### Công việc đã thực hiện

| Ngày | Công việc | Kết quả | Nguồn tài liệu |
| --- | --- | --- | --- |
| 1 | Tạo EventBridge rule bắt sự kiện MediaConvert job state change | Nhận được event COMPLETE/ERROR/CANCELED | EventBridge Docs: <https://docs.aws.amazon.com/eventbridge/latest/userguide/> |
| 2 | Viết Lambda `netflop-mediaconvert-notifier` gọi webhook backend | Backend tự cập nhật trạng thái tập phim | Lambda Developer Guide: <https://docs.aws.amazon.com/lambda/latest/dg/welcome.html> |
| 3 | Kiểm thử webhook `/api/uploads/mediaconvert/events` | Tập phim chuyển sang ready khi encode xong | Express Routing: <https://expressjs.com/en/guide/routing.html> |
| 4 | Viết Lambda subtitle converter chuyển `.srt` sang `.vtt` | Phụ đề hiển thị được trên player | WebVTT: <https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API> |

### Kết quả đạt được

* Media pipeline chuyển sang hướng event-driven, không cần backend polling liên tục.
* Tập phim được tự động cập nhật trạng thái sau khi MediaConvert xử lý xong.
* Phụ đề SRT được chuyển sang VTT để dùng trên trình phát web.

