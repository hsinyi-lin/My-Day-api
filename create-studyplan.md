###### tags: `studyplan`
# create-studyplan 建立讀書計畫
## /create-studyplan
front to back

| 說明     | key                       | value    |
| -------- | ------------------------- | -------- |
| 帳號     | uid                       | string   |
| 標題     | title(schedule_name)      | string   |
| 行程編號 | scheduleNum               | int      |
| 開始時間 | startTime(schedule_start) | datetime |
| 結束時間 | endTime(schedule_end)     | datetime |
| 科目     | subject(subjects)         | object   |

| 科目{}       |              |          |
| ------------ | ------------ | -------- |
| 科目名稱     | subjectName(subject)  | string   |
| 科目開始時間 | subjectStart(plan_start) | datetime |
| 科目結束時間 | subjectEnd(plan_end)   | datetime |
| 休息         | rest(is_rest)         | bool     |


back to front

| 說明             | key      | value |
| ---------------- | -------- | ----- |
| 建立讀書計畫結果 | response | bool  |

---
uid:
 >account>user_id

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

---
**scheduleNum**  

兩種情況：  
1.在現有行程建立讀書計畫  
(行程編號的類型是學習才能建立，行程名稱不變)  
2.在讀書計畫建立讀書計畫  
行程新增一個學習行程

---
前端限制開始結束時間