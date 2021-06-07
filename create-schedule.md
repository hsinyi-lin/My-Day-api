###### tags: `schedule`
# create-schedule 建立行程
## /schedule/create_new/
front to back

| 說明     | key       | value    |
| -------- | --------- | -------- |
| 帳號     | uid        | string   |
| 標題     | title     | string   |
| 開始時間 | startTime | datetime |
| 結束時間 | endTime   | datetime |
| 提醒     | remind    | object   |
| 類別編號 | typeId   | int      |
| 倒數     | isCountdown | bool     |
| 地點     | place  | string     |
| 備註     | remark    | string   |

&nbsp;

| 提醒{}   |            |          |
| -------- | ---------- | -------- |
| 是否開啟 | isRemind   | bool     |
| 提醒時間 | remindTime[] | datetime |

back to front

| 說明         | key      | value |
| ------------ | -------- | ----- |
| 建立課表結果 | response | bool  |


---
uid:
 >account>user_id

title:
 >schedule>schedule_name

startTime:
 >schedule>schedule_start

endTime:
 >schedule>schedule_end  

* **Remind**  
	* isRemind:
	 	>personal_schedule>is_notice
 
	* isRemind:
	 	>schedule_notice>notice_time

typeId:
 >type>type_id  

countdown:
 >personal_schedule>is_countdown

place:
 >schedule>place

remark:
 >personal_schedule>remark

---
* **提醒：**  
    * 可同時傳回多個提醒時間 

**使用者建立行程**  
* 個人建立行程時會在schedule資料表中新增一筆資料，並且在personal_schedule新增多筆資料
* 群組建立行程時會新增一個schedule並新增多個personal_schedule
* 個人行程的connect_group_no可為空

```
EX:

{{
    "uid":"amy123",
    "title":"開會",
    "startTime":"2021-06-07 21:00:00",
    "endTime":"2021-06-07 22:00:00",
    "remind":{
        "isRemind":true,
        "remindTime":["2021-06-07 21:10:00","2021-06-07 21:20:00"]
    },
    "typeId":1,
    "isCountdown":false,
    "place":null,
    "remark":"test"
}
```