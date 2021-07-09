###### tags: `schedule`
# get-schedule 取得行程
## /schedule/get/
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 行程編號 | scheduleNum | int    |

back to front

| 說明     | key       | value    |
| -------- | --------- | -------- |
| 標題     | title     | string   |
| 開始時間 | startTime | datetime |
| 結束時間 | endTime   | datetime |
| **提醒** | remind    | object   |
| 類別編號 | typeId   | int      |
| 倒數     | isCountdown | bool     |
| 地點     | place  | string   |
| 備註     | remark    | string   |

&nbsp;

| 提醒{}   |            |          |
| -------- | ---------- | -------- |
| 是否開啟 | isRemind   | bool     |
| 提醒時間 | remindTime | datetime |

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no
---
### 用於
* 使用者取得行程  
在行程列表中點選
