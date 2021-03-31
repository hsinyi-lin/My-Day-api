###### tags: `schedule`
# schedule-list 行程列表
## /schedule-list
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |

back to front

| 說明     | key         | value    |
| -------- | ----------- | -------- |
| 行程   | schedule    | object   |


| 行程{} |             |          |
| ---------- | ----------- | -------- |
| 行程編號 | scheduleNum | int      |
| 標題     | title       | string   |
| 開始時間 | startTime   | datetime |
| 結束時間 | endTime     | datetime |
| 類別編號 | typeId     | int      |

---
uid:
 >account>user_id