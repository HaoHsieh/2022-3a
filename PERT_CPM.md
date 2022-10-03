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

