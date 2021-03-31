###### tags: `account`
# send-code 驗證碼
## /send-code
front to back

| 說明 | key | value  |
| ---- | --- | ------ |
| 帳號 | uid  | string |

back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 驗證帳號結果 | response | bool  |

---
uid:
 >account>user_id
---

**傳送驗證碼**  

當使用者忘記密碼時可以使用忘記密碼，系統會傳送驗證碼到使用者信箱確認是否為本人