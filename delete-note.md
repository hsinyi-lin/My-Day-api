###### tags: `note`
# delete-note 刪除筆記
## /note/delete/
front to back

| 說明     | key     | value  |
| -------- | ------- | ------ |
| 帳號     | uid     | string |
| 筆記編號 | noteNum | int    |


back to front

| 說明     | key      | value |
| -------- | -------- | ----- |
| 刪除筆記結果 | response | bool  |

---
uid:
 >account>user_id

noteNum:
 >note>serial_no