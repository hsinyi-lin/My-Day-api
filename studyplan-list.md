###### tags: `studyplan`
# personal-studyplan-list 個人讀書計畫列表
## /personal-studyplan-list
front to back

| 說明 | key | value  |
| ---- | --- | ------ |
| 帳號 | uid  | string |

back to front

| 說明         | key          | value    |
| ------------ | ------------ | -------- |
| 讀書計畫編號 | studyplanNum | string   |
| 標題         | title        | string   |
| 日期         | date         | datetime |
| 開始時間     | startTime    | datetime |
| 結束時間     | endTime      | datetime |

---
uid:
 >account>user_id


----
### <font color=red> **注意**  </font>
這個是個人學習計畫列表+全部群組的共同學習計畫列表
需呼叫此API和group-studyplan-list的API