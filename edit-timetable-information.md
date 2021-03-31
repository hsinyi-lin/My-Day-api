###### tags: `timetable`
# edit-timetable-information 編輯課表資訊
## /edit-timetable-information
front to back

| 說明         | key        | value    |
| ------------ | ---------- | -------- |
| 帳號         | uid         | string   |
| 學校         | school     | string   |
| 學年         | schoolYear | string   |
| 學期         | semester   | string   |
| 學期開始日期 | startTime  | datetime |
| 學期結束日期 | endTime    | datetime |

back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 編輯課表資訊結果 | response |  bool     |

---
uid:
 >account>uid

school:
 >school>school_name

schoolYear:
 >personal_timetable>semester

兩個會合起來存回資料庫

semester:
 >personal_timetable>semester

startTime:
 >personal_timetable>semester_start

endTime
 >personal_timetable>semester_end
---
### <font color=red> **注意**  </font>
只傳要編輯的內容其他回傳空值即可