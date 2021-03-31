###### tags: `timetable`
# delete-accept-timetable 刪除接受課表
## /delete-accept-timetable
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 課表編號 | timetableId | string |



back to front

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 刪除接受課表 | response  | bool |

---
uid:
 >account>uid

timetableId:
 >personal_timetable>timetable_no