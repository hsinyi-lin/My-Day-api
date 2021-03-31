###### tags: `timetable`
# delete-timetable 刪除課表
## /delete-timetable
front to back

| 說明 | key        | value  |
| ---- | ---------- | ------ |
| 帳號 | uid         | string |
| 學年 | schoolYear | string |
| 學期 | semester   | string |

---
uid:
 >account>uid

schoolYear:
 >personal_timetable>semester

兩個會合起來存回資料庫

semester:
 >personal_timetable>semester


back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 刪除課表結果 | response |  bool  |
