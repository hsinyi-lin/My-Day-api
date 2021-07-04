###### tags: `schedule`
# create-common-schedule 建立共同行程
## /create_common
front to back

| 說明     | key       | value    |
| -------- | --------- | -------- |
| 帳號     | uid        | string   |
| 群組編號 | groupNum   | int      |
| 標題     | title     | string   |
| 開始時間 | startTime | datetime |
| 結束時間 | endTime   | datetime |
| 類別編號 | typeId   | int      |
| 地點     | place  | string     |


back to front

| 說明             | key      | value |
| ---------------- | -------- | ----- |
| 建立共同行程結果 | response | bool      |

---
uid:
 >account>user_id

groupNum:
 >group>serial_no

title:
 >schedule>schedule_name

startTime:
 >schedule>schedule_start

endTime:
 >schedule>schedule_end  

typeId:
 >type>type_id  

location:
 >schedule>place

---
### <font color=red> **後端注意：**  </font>
需驗證此使用者是否在群組內  
&nbsp;  

* 透過群組編號建立行程(connect_group_no)，連接每位成員的personal_schedul