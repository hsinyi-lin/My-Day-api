###### tags: `vote`
# get-vote 取得投票
## /vote/get/
front to back

| 說明     | key     | value  |
| -------- | ------- | ------ |
| 帳號     | uid      | string |
| 投票編號 | voteNum | int    |


back to front

| 說明         | key                | value    |
| ------------ | ------------------ | -------- |
| 標題         | title              | string   |
| 投票項目     | voteItems          | object   |
| 允許新增     | addItemPermit      | bool     |
| 截止日       | deadline           | datetime |
| 匿名         | anonymous          | bool     |
| 選擇投票數量 | chooseVoteQuantity | int       |
| 投票次數     | voteCount          |  int    |

| 投票項目{}   |              |        |
| ------------ | ------------ | ------ |
| 投票項目編號 | voteItemNum  | int    |
| 投票項目名稱 | voteItemName | string |

---
uid:
 >account>user_id

voteNum:
 >vote>serial_no