###### tags: `刪除`
# add-vote-items 新增投票項目
## /vote/add_items/
front to back

| 說明     | key       | value  |
| -------- | --------- | ------ |
| 帳號     | uid       | string |
| 投票編號 | voteNum   | int    |
| 投票項目 | voteItems | object |


| 投票項目{}   |              |        |
| ------------ | ------------ | ------ |
| 投票項目編號 | voteItemNum  | int    |
| 投票項目名稱 | voteItemName | string |

back to front

| 說明             | key     | value |
| ---------------- | ------- | ----- |
| 新增投票項目結果 | response | bool      |