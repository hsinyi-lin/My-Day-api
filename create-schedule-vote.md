###### tags: `vote`
# create-schedule-vote 建立行程的投票
## /create-schedule-vote
front to back

| 說明         | key                | value  |
| ------------ | ------------------ | ------ |
| 帳號         | id                 | string |
| 群組編號     | groupId            |        |
| 標題         | title              |        |
| 投票日期     | voteDate          |        |
| 截止日       | deadline           |        |
| 允許新增     | addItemPermit      |        |
| 匿名         | anonymous          |        |
| 選擇投票數量 | chooseVoteQuantity |        |


back to front

| 說明         | key     | value |
| ------------ | ------- | ----- |
| 建立投票結果 | request |       |