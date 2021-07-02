###### tags: `schedule`
# delete-schedule 刪除行程
## /schedule/delete/
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 行程編號 | scheduleNum | int    |

back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 刪除行程結果 | response | bool  |

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no

---
### <font color=red> **注意**  </font>
包含刪除行程和共同行程，但是共同行程只有管理者可以刪除