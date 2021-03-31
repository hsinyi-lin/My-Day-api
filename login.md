###### tags: `account`
# login 登入
## /login
front to back

| 說明 | key      | value  |
| ---- | -------- | ------ |
| 帳號 | uid       | string |
| 密碼 | password | string |


back to front

| 說明 | key      | value  |
| ---- | -------- | ------ |
| 姓名 | userName | string |


### <font color=red> **注意**  </font>
login 呼叫 行程、課表、學習計畫、設定

---
uid:
 >account>user_id

password:
 >account>password  

---

**使用者登入**  

使用者輸入帳號密碼後可取得個人資訊  
登入時會初始化課表、學習計畫、設定  
後端傳回初始化資料json  
加好友、飯局、群組等需要線上操作的功能無需在登入時載入，此功能在使用者需要時再透過網路來載入