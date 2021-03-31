###### tags: `timetable`
# edit-timetable 編輯課表
## /edit-timetable
front to back

| 說明 | key        | value  |
| ---- | ---------- | ------ |
| 帳號 | uid         | string |
| 學年 | schoolYear | string |
| 學期 | semester   | string |
| 課程 | subject    | object |

&nbsp;
&nbsp;

| 課程{} |             |          |
| ---------- | ----------- | -------- |
| 課程名稱   | subjectName | string   |
| 課程開始   | startTime   | datetime |
| 課程結束   | endTime     | datetime |
| 星期       | week        | int      |

back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 編輯課表結果 | response |  bool     |

---
uid:
 >account>uid

schoolYear:
 >personal_timetable>semester

兩個會合起來存回資料庫

semester:
 >personal_timetable>semester

subjectName:
 >subject>subject_name

startTime:
 >class_time>start

endTime:
 >class_time>end
 
week:
 >section>weekday
---
* 星期要自己算資料庫沒有存(課程結束-課程開始)
