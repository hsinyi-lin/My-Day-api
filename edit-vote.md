###### tags: `vote`
# edit-vote 編輯投票
## /vote/edit/
front to back

| 說明         | key                | value    |
| ------------ | ------------------ | -------- |
| 帳號         | uid                 | string   |
| 投票編號     | voteNum            | int      |
| 標題         | title              | string   |
| 投票項目     | voteItems          | object   |
| 截止日       | deadline           | datetime |
| 允許新增     | isAddItemPermit      | bool     |
| 匿名         | isAnonymous          | bool     |
| 選擇投票數量 | chooseVoteQuantity | int      |


| 投票項目{}   |              |        |
| ------------ | ------------ | ------ |
| 投票項目編號 | voteItemNum  | int    |
| 投票項目名稱 | voteItemName | string |


back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 編輯投票結果 | response | bool      |

---
uid:
 >account>user_id

voteNum:
 >vote>serial_no

title:
 >vote>title

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

### <font color=red> **注意**  </font>
沒人投票才可以用  
請將全部投票項目傳入，否則會被刪除