###### tags: `schedule`
# get-common-schedule 取得共同行程
## /get-common-schedule
front to back

| 說明     | key         | value  |
| -------- | ----------- | ------ |
| 帳號     | uid          | string |
| 行程編號 | scheduleNum | int    |


back to front

| 說明     | key       | value    |
| -------- | --------- | -------- |
| 標題     | title     | string   |
| 開始時間 | startTime | datetime |
| 結束時間 | endTime   | datetime |
| 類別名稱 | typeName | string   |
| 地點     | place     | string   |

**注意權限**

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no
 
---
### 用於
* 共同行程剛新增時成員點選收到的通知
* 詳細說明
    1. 共同行程建立
    2. 群組成員收到通知（顯示於群組通知列表）
    3. 成員可設定倒數和新增通知時間（此時用此api來取得資料）
    4. 生成一個personal_schedule來記錄以上資訊