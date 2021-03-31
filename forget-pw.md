###### tags: `account`
# forget-pw 忘記密碼
## /forget-pw
front to back

| 說明   | key              | value  |
| ------ | ---------------- | ------ |
| 帳號   | uid               | string |
| 驗證碼 | verificationCode | string |


back to front

| 說明     | key      | value |
| -------- | -------- | ----- |
| 驗證結果 | response | bool  |

---
uid:
 >account>user_id

verificationCode:
 >account>password
---

**使用者忘記密碼**  
接收到新密碼後，使用者再輸入一次新密碼即可登入