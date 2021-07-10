###### tags: `note`
# create-note 建立筆記
## /note/create_new/
front to back

| 說明 | key      | value  |
| ---- | -------- | ------ |
| 帳號 | uid      | string |
| 分類 | typeName | string |
| 標題 | title    | string |
| 內容 | content  | string |


back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 建立筆記結果 | response | bool  |

---
uid:
 >account>user_id

typeName:
 >note>type_name

title:
 >note>title

content:
 >note>content