###### tags: `account`
# login 登入
## /login
font to back

| 說明 | key | value  |
| ---- | --- | ------ |
| 密碼 | pw  | string |
| 帳號 | id  | string |

back to font

| 說明     | key             | value  |
| -------- | --------------- | ------ |
| 姓名     | name            | string |
| 課表     | schoolTimetable | object |
| 學習計畫 | studyPlan       | object |
| 設定     | setting         | object |


---

**使用者登入**  

使用者輸入帳號密碼後可取得個人資訊  
登入時會初始化課表、學習計畫、設定  
後端傳回初始化資料json  
加好友、飯局、群組等需要線上操作的功能無需在登入時載入，此功能在使用者需要時再透過網路來載入
