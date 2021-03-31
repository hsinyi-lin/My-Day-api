###### tags: `timetable`
# get-timetable 取得課表
## /get-timetable
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid         | string |
| 課表編號 | timetableId | int    |

back to front

| 說明     | key        | value    |
| -------- | ---------- | -------- |
| 學校     | school     | string   |
| 學年     | schoolYear | string   |
| 學期     | semester   | string   |
| 開始日期 | startDate  | datetime |
| 結束日期 | endDate    | datetime |
| 課程     | subject    | object   |
&nbsp;
&nbsp;

| 課程{} |             |          |
| ---------- | ----------- | -------- |
| 課程名稱   | subjectName | string   |
| 課程開始   | startTime   | datetime |
| 課程結束   | endTime     | datetime |
| 星期       | week        | int      |

---
uid:
 >account>uid

timetableId:
 >personal_timetable>timetable_no