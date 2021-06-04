###### tags: `account`
# register 註冊
## /register
front to back

| 說明 | key      | value  |
| ---- | -------- | ------ |
| 姓名 | userName | string |
| 帳號 | uid       | string |
| 密碼 | password | string |

back to front
| 說明     | key      | value |
| -------- | -------- | ----- |
| 註冊結果 | response | bool  |

---
userName:
 >account>name  

uid:
 >account>user_id

password:
 >account>password
---

**使用者註冊**  
使用者輸入姓名、帳號、密碼後即可使用帳號、密碼登入