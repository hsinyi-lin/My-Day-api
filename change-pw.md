###### tags: `account`
# change-pw 變更密碼
## /change-pw
front to back

| 說明       | key      | value  |
| ---------- | -------- | ------ |
| 帳號       | uid       | string |
| 新密碼     | password | string |


back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 更改密碼結果 | response | bool  |

### <font color=red> **注意**  </font>
前端判斷新密碼以及確認新密碼

---
uid:
 >account>user_id

password:
 >account>password
---

**使用者更改密碼**  

確認為本人後，使用者可以輸入新的密碼以及確認新密碼，來更改舊密碼，之後回到登入畫面
