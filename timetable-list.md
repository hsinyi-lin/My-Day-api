###### tags: `timetable`
# main-timetable-list 課表列表
## /timetable-list
front to back

| 說明 | key | value  |
| ---- | --- | ------ |
| 帳號 | uid  | string |

back to front

| 說明     | key         | value    |
| -------- | ----------- | -------- |
| 課表編號 | timetableId | int   |
| 學年     | schoolYear  | string   |
| 學期     | semester    | string   |
| 開始日期 | startDate   | datetime |
| 結束日期 | endDate     | datetime |
| 課程     | subject     | object   |

&nbsp;
&nbsp;

| 課程內容{} |             |          |
| ---------- | ----------- | -------- |
| 課程名稱   | subjectName | string   |
| 課程開始   | startTime   | datetime |
| 課程結束   | endTime     | datetime |
| 星期       | week        | int      |

---
uid:
 >account>uid
