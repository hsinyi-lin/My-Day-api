###### tags: `studyplan`
# get-studyplan 取得讀書計畫
## /get-studyplan
front to back

| 說明         | key          | value  |
| ------------ | ------------ | ------ |
| 帳號         | uid          | string |
| 讀書計畫編號 | studyplanNum | int    |

back to front

| 說明         | key          | value    |
| ------------ | ------------ | -------- |
| 標題         | title        | string   |
| 日期         | date         | datetime |
| 開始時間     | startTime    | datetime |
| 結束時間     | endTime      | datetime |
| 科目         | subject      | object   |


| 科目{}       |              |          |
| ------------ | ------------ | -------- |
| 科目名稱     | subjectName  | string   |
| 科目開始時間 | subjectStart | datetime |
| 科目結束時間 | subjectEnd   | datetime |
| 休息         | rest         | bool     |

---
uid:
 >account>user_id

studyplanNum:
 >study_plan>serial_no


