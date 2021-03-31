###### tags: `studyplan`
# delete-studyplan 刪除個人讀書計畫
## /delete-studyplan
front to back

| 說明         | key         | value  |
| ------------ | ----------- | ------ |
| 帳號         | uid         | string |
| 讀書計畫編號 | studyplanNum | int    |


back to front

| 說明             | key      | value |
| ---------------- | -------- | ----- |
| 刪除學習計畫結果 | response | bool  |

---
uid:
 >account>user_id

studyplanNum:
 >study_plan>serial_no
