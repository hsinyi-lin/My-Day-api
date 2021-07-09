###### tags: `schedule`
# common-schedule-hidden 隱藏共同行程設定
## /schedule/common_hidden/
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid         | string |
| 行程編號 | scheduleNum | int    |
| 狀態     | isHidden    | bool   |

back to front
| 說明         | key      | value |
| ------------ | -------- | ----- |
| 隱藏共同行程結果 | response | bool  |

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no

isHidden:
 >personal_schedule>is_hidden