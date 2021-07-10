###### tags: `note`
# edit-note 編輯筆記
## /note/edit/
front to back

| 說明     | key      | value  |
| -------- | -------- | ------ |
| 帳號     | uid      | string |
| 筆記編號 | noteNum  | int    |
| 分類     | typeName | string |
| 標題     | title    | string |
| 內容     | content  | string |



back to front

| 說明     | key      | value |
| -------- | -------- | ----- |
| 編輯筆記結果 | response | bool  |

---
uid:
 >account>user_id

noteNum:
 >note>serial_no

typeName:
 >note>type_name

title:
 >note>title

content:
 >note>content