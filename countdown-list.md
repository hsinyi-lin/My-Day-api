###### tags: `schedule`
# countdown-list 倒數列表
## /countdown-list
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 行程編號 | scheduleNum | int    |

back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 行程 | scheduleNum | object  |


| 行程{}   |               |        |
| -------- | ------------- | ------ |
| 標題     | title         | string |
| 倒數天數 | countdownDate | int    |

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no
