|任務|說明|需時(天)|前置任務|
|:---:|:---:|:---:|:---:|
|1|研擬計畫|1|-|
|2|任務分配|4|1|
|3|取得硬體|17|1|
|4|格式開發|70|2|
|5|安裝硬體|10|3|
|6|程式測試|30|4|
|7|撰寫使用手冊|25|5|
|8|轉換檔案|20|5|
|9|系統測試|25|6|
|10|使用者訓練|20|7,8|
|11|使用者測試|25|9,10|

```mermaid
gantt
    title 甘特圖

    section 研擬計畫
    研擬計畫             : a1, 2022-10-03, 1d
    section 任務分配
    任務分配             : a2, after a1, 4d
    section 取得硬體
    取得硬體             : a3, after a1, 17d
    section 格式開發
    格式開發             : a4, after a2, 70d
    section 安裝硬體
    安裝硬體             : a5, after a3, 10d
    section 程式測試
    程式測試             : a6, after a4, 30d
    section 撰寫使用手冊
    撰寫使用手冊          : a7, after a5, 25d
    section 轉換檔案
    轉換檔案             : a8, after a5, 20d
    section 系統測試
    系統測試             : a9, after a6, 25d
    section 使用者訓練
    使用者訓練           : a10, after a7, 20d
    section 使用者測試
    使用者測試           : a11, after a9, 25d
```

```mermaid
classDiagram
    研擬計畫 --|> 任務分配:1d
    研擬計畫 --> 取得硬體:1d
    取得硬體 --> 安裝硬體:17d
    安裝硬體 --> 撰寫使用手冊:10d
    安裝硬體 --> 轉換檔案:10d
    撰寫使用手冊 --> 使用者訓練:25d
    轉換檔案 --> 使用者訓練:20d
    使用者訓練 --> 使用者測試:20d
    
    任務分配 --|> 格式開發:4d
    格式開發 --|> 程式測試:70d
    程式測試 --|> 系統測試:30d
    系統測試 --|> 使用者測試:25d
    
    研擬計畫 : 開始：第1天
    研擬計畫 : 結束：第1天
    研擬計畫 : 需時：第1天
    
    任務分配 : 開始：第2天
    任務分配 : 結束：第5天
    任務分配 : 需時：第4天
    
    取得硬體 : 開始：第2天
    取得硬體 : 結束：第18天
    取得硬體 : 需時：第17天
    
    安裝硬體 : 開始：第19天
    安裝硬體 : 結束：第28天
    安裝硬體 : 需時：第10天
    
    撰寫使用手冊 : 開始：第29天
    撰寫使用手冊 : 結束：第53天
    撰寫使用手冊 : 需時：第25天
    
    轉換檔案 : 開始：第29天
    轉換檔案 : 結束：第49天
    轉換檔案 : 需時：第20天
    
    使用者訓練 : 開始：第54天
    使用者訓練 : 結束：第73天
    使用者訓練 : 需時：第20天
    
    格式開發 : 開始：第6天
    格式開發 : 結束：第75天
    格式開發 : 需時：第70天
    
    程式測試 : 開始：第76天
    程式測試 : 結束：第105天
    程式測試 : 需時：第30天
    
    系統測試 : 開始：第106天
    系統測試 : 結束：第130天
    系統測試 : 需時：第25天
    
    使用者測試 : 開始：第131天
    使用者測試 : 結束：第155天
    使用者測試 : 需時：第25天
    
    
    
```

