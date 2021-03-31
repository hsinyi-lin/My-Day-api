###### tags: `studyplan`
# sharing-studyplan 共享讀書計畫
## /sharing-studyplan
front to back

| 說明         | key          | value  |
| ------------ | ------------ | ------ |
| 帳號         | id           | string |
| 讀書計畫編號 | studyplanNum | int    |
| 群組編號     | groupNum     | int    |


back to front

| 說明             | key      | value |
| ---------------- | -------- | ----- |
| 共享讀書計畫結果 | response | bool      |

---
uid:
 >account>user_id

studyplanNum:
 >study_plan>serial_no

groupNum:
 >group>serial_no



---
### <font color=red> **注意**  </font>
讀書計畫只能分享給一個群組
```
一個人無法同時出現在兩個群組跟兩群人讀書
```