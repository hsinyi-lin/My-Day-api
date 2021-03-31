###### tags: `timetable`
# accept-timetable 接受課表
## /accept-timetable
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 課表編號 | timetableId | string |


back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 接受課表結果 | response | bool   |

---
uid:
 >account>uid

timetableId:
 >personal_timetable>timetable_no

---
預覽後可以接受課表