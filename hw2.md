## 題目
| 任務 |說明| 需時(天) | 前置任務|
|:----:|:-:|:-------:|:-------:|
|1|研擬計畫|1|-|
|2|任務分配|4|1|
|3|取得硬體|17|1|
|4|程式開發|70|2|
|5|安裝硬體|10|3|
|6|程式測試|30|4|
|7|撰寫使用手冊|25|5|
|8|轉換檔案|20|5|
|9|系統測試|25|6|
|10|使用者訓練|20|7,8|
|11|使用者測試|25|9,10|

## PERT/CPM圖
![CPM&PERT圖](CPM&PERT圖.png "程式碼github轉不過來QQ")  
### 關鍵路徑:1->2->4->6->9->11

## 甘特圖
```mermaid
gantt
    title A Gantt Diagram
    
    section Section
    研擬計畫 : a1, 2022-10-03, 1d
    任務分配 : a2, after a1, 4d
    取得硬體 : a3, after a1, 17d  
    程式開發 : a4, after a2, 70d
    安裝硬體 : a5, after a3, 10d
    程式測試 : a6, after a4, 30d
    撰寫使用手冊 :a7, after a5, 25d
    轉換檔案 : a8, after a5, 20d
    系統測試 : a9, after a6, 25d
    使用者訓練 : a10, after a7, 20d
    使用者測試 : after a9, 25d
```

