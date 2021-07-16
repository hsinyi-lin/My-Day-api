###### tags: `vote`
# vote 投票
## /vote
front to back

| 說明         | key         | value  |
| ------------ | ----------- | ------ |
| 投票編號     | voteNum     | int    |
| 投票項目編號 | voteItemNum | int list  |
| 帳號(投票者) | uid          | string |

back to front

| 說明     | key      | value |
| -------- | -------- | ----- |
| 投票結果 | response | bool  |

---
voteNum:
 >vote>serial_no
 
voteItemNum:
 >vote_option>option_num(vote_option資料表和vote_date_option資料表都是)

uid:
 >account>user_id

voteType>
 >判斷vote_record裡有沒有