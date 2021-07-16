###### tags: `vote`
# vote-list 投票列表
## /vote/get_list/
front to back

| 說明     | key     | value |
| -------- | ------- | ----- |
| 帳號     | uid      | string |
| 群組編號 | groupNum | int   |


back to front

| 說明 | key  | value  |
| ---- | ---- | ------ |
| 投票 | vote | object |

| vote{}   |            |        |
| -------- | ---------- | ------ |
| 投票編號 | voteNum    | int    |
| 投票人數 | votersNum  | int    |
| 標題     | title      | string |
| 投票狀態 | isVoteTpye | bool   |

---
uid:
 >account>user_id

groupNum:
 >group>serial_no