###### tags: `schedule`
# common-schedule-list 共同行程列表
## /common-schedule-list
front to back

| 說明     | key     | value  |
| -------- | ------- | ------ |
| 帳號     | uid     | string |
| 群組編號 | groupNum | int    |

back to front

| 說明     | key         | value    |
| -------- | ----------- | -------- |
| 行程編號 | scheduleNum | int      |
| 標題     | title       | string   |
| 開始時間 | startTime   | datetime |
| 結束時間 | endTime     | datetime |
| 類別名稱 | typeName   | string   |

---
uid:
 >account>user_id

groupNum:
 >serial_no

___
* 取得該群組的所有行程

* **與臨時群組共用**