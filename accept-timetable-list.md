###### tags: `timetable`
# accept-timetable-list 接受課表列表
## /accept-timetable-list
front to back

| 說明 | key        | value  |
| ---- | ---------- | ------ |
| 帳號 | id         | string |
| 學年 | schoolYear | string |
| 學期 | semester   | string |


back to front

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 好友姓名 | friendName  | string |
| 課表編號 | timetableId | string |

---
uid:
 >account>uid

schoolYear:
 >personal_timetable>semester

兩個會合起來存回資料庫

semester:
 >personal_timetable>semester

---
選取課表之後先使用get-timetable預覽課表