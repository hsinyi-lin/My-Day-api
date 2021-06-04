###### tags: `studyplan`
# edit-studyplan 編輯讀書計畫
## /edit-studyplan
front to back

| 說明         | key                       | value    |
| ------------ | ------------------------- | -------- |
| 帳號         | uid                       | string   |
| 讀書計畫編號 | studyplanNum              | int      |
| 標題         | title(schedule_name)      | string   |
| 開始時間     | startTime(schedule_start) | datetime |
| 結束時間     | endTime(schedule_end)     | datetime |
| 科目         | subject(subjects)         | object   |

| 科目{}       |              |          |
| ------------ | ------------ | -------- |
| 科目名稱     | subjectName(subject)  | string   |
| 科目開始時間 | subjectStart(plan_start) | datetime |
| 科目結束時間 | subjectEnd(plan_end)   | datetime |
| 休息         | is_rest       | bool     |

back to front

| 說明             | key      | value |
| ---------------- | -------- | ----- |
| 編輯讀書計畫結果 | response | bool  |

---
uid:
 >account>user_id

studyplanNum:
 >study_plan>serial_no

title:
 >schedule>schedule_name

scheduleNum:
 >schedule>serial_no

date:
 >schedule>schedule_start

startTime:
 >schedule>schedule_start
 >
endTime
 >schedule>schedule_end

subjectName:
 >plan_content>subject

subjectStart:
 >plan_content>plan_start

subjectEnd:
 >plan_content>plan_end

rest:
 >plan_content>is_rest