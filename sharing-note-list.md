###### tags: `note`
# group-note-list 群組筆記列表
## /note/group_list/
front to back

| 說明     | key     | value  |
| -------- | ------- | ------ |
| 帳號     | uid     | string |
| 群組編號 | groupNum | int    |


back to front

| 說明 | key  | value  |
| ---- | ---- | ------ |
| 筆記 | note | object |

| note{}   |          |        |
| -------- | -------- | ------ |
| 筆記編號 | noteNum  | int    |
| 分類     | typeName | string |
| 標題     | title    | string |

---
uid:
 >account>user_id

groupNum:
 >group>serial_no

### <font color=red> **注意**  </font>
這個是某個群組的共同筆記列表
