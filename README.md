# AWS Rekognition Application
## 安全防護系統的功能介紹
1. 可疑人物: 當店內出現穿著可疑的人，系統進行影像分析後認為是可疑人物，會傳送警示給員工和老闆。
>* 使用 `PPE detection` 偵測遮掩穿著: 鼻子是否有口罩覆蓋、頭上是否有安全帽覆蓋，以及手上是否有手套覆蓋。

2. 現行犯: 如果店內可疑人物亮出`槍、刀子等危險器械`進行搶劫，就會觸發系統傳送案發現場影像，到勤務指揮中心的接收平台來自動報案， 最後，系統會上傳歹徒的影像到黑名單資料庫。
>* 使用 `Label detection` 偵測危險物品標籤: 偵測標籤出現 "Gun" or "Knife" or "Axe" or "Sword" 即成立條件
>* Moderating content 偵測部不當內容: 偵測標籤出現 Violence" or "Graphic Violence Or Gore" or "Physical Violence" or "Weapon Violence" 即成立條件

3.通緝犯: 當店內出現通緝犯時，防護系統會將拍到的臉孔與資料庫進行比對，確認是通緝犯就會自動視訊報案，並發送警示給店家。
>* Face comparison 比對偵測目標與黑名單資料

4.奧客: 當奧客出現時，因為有黑名單資料的紀錄，一出現就會發出警示，如有不良意圖及舉動，自動視訊報案。
>* Face comparison 比對偵測目標與黑名單資料
>* Moderating content 偵測部不當內容: Violence" or "Graphic Violence Or Gore" or "Physical Violence" or "Weapon Violence"

[智慧防護系統](./智慧防護系統_第 9 組_20210907.pdf)



