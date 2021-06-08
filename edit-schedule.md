###### tags: `schedule`
# edit-schedule 編輯行程
## /edit-schedule
front to back

| 說明     | key         | value    |
| -------- | ----------- | -------- |
| 帳號     | uid         | string   |
| 行程編號 | scheduleNum | int      |
| 標題     | title       | string   |
| 開始時間 | startTime   | datetime |
| 結束時間 | endTime     | datetime |
| 提醒     | remind    | object   |
| 類別     | typeId      | int      |
| 倒數     | isCountdown | bool     |
| 地點     | place       | string   |
| 備註     | remark      | string   |

&nbsp;

| 提醒{}   |            |          |
| -------- | ---------- | -------- |
| 是否開啟 | isRemind   | bool     |
| 提醒時間 | remindTime | datetime |

back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 編輯行程結果 | response | bool  |

---
uid:
 >account>user_id

scheduleNum:
 >schedule>serial_no

title:
 >schedule>schedule_name

startTime:
 >schedule>schedule_start

endTime:
 >schedule>schedule_end  

* **isRemind**  
	* isRemind:
	 	>personal schedule>is_notice
 
	* isRemind:
	 	>personal schedule>notice_time

typeId:
 >type>type_id  

isCountdown:
 >personal schedule>is_countdown

place:
 >schedule>place

remark:
 >personal schedule>remark
---
### 用於
* 編輯個人行程
* 編輯共同行程
* 編輯臨時群組行程  

<font color=red>注意：</font>
將有所變更的欄位存入資料庫，若沒有變更的欄位則可以不用傳至後端（可由後端自行更改規則）  
**提醒時間無論有無修改需全部傳至後端**