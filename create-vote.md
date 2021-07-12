###### tags: `vote`
# create-vote 建立投票
## /vote/create_new/
front to back

| 說明         | key                | value    |
| ------------ | ------------------ | -------- |
| 帳號         | uid                | string   |
| 群組編號     | groupNum           | int      |
| 投票類別     | optionTypeId       | int      |
| 標題         | title              | string   |
| 投票項目     | voteItems          | object   |
| 截止日       | deadline           | datetime |
| 允許新增     | isAddItemPermit    | bool     |
| 匿名         | isAnonymous        | bool     |
| 選擇投票數量 | chooseVoteQuantity | int      |



| 投票項目{}   |              |        |
| ------------ | ------------ | ------ |
| 投票項目編號 | voteItemNum  | int    |
| 投票項目名稱 | voteItemName | string |


back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 建立投票結果 | response | bool      |

---
uid:
 >account>user_id

groupNum:
 >group>serial_no

optionTypeId:
 >option_type>option_type_id

voteItemNum:
 >vote_option>option_num(vote_option資料表和vote_date_option資料表都是)

voteItemName:
 >vote_option>content

deadline:
 >vote>end_time

isAddItemPermit:
 >vote>is_add_item_permit

isAnonymous:
 >vote>is_anonymous

chooseVoteQuantity:
 >vote>mutiple_choice
---
### <font color=red> **注意**  </font>
至少一個選項，並且開放新增投票