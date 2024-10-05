# Mouse Utopia: Non-Invasive Mouse Monitoring and Vital Sign Prediction Meets Video Generation 
## 組員<br>
+ 張聖坤 C111118124<br>
+ 張任沂 C111118128<br>
+ 李杰　C109143138<br>

## 專案介紹
https://docs.google.com/document/d/1I6LmDxumgGYgtsrIZVUO2RomxJ6OgTnBFnN7nqPlHHo/edit?pli=1

## 工作分配
### 張聖坤
>資料收集與設備操作
>>負責設置和操作非侵入性的資料收集設備，如玻璃箱、Duo len 相機、熱像儀和 mmWave 雷達。
確保收集到的數據涵蓋心率、皮膚溫度、骨架姿態和運動等關鍵生理數據。
統籌所有刺激裝置（如雷射、喇叭、LED 燈等）來模擬不同實驗條件。
>>
### 張任沂
>數據分析與模型訓練
>>使用收集到的數據來訓練神經網絡，包括預測心率、皮膚溫度和行為姿態等模型。
利用 DeepLabCut 進行姿態估測，並結合 HRNet 和 Swin Transformer 增強精準度。
訓練生成模型，如 VideoGPT 和 MoCoGAN，來模擬和生成實驗鼠行為的短片，以構建數字雙胞胎。
>>
### 李杰
>數據後處理與應用開發
>>使用自然語言處理技術（例如 BERT、GPT-3）分析鼠類表型資料庫（Mouse Phenome Database），為藥物效應預測提供支持。
開發與數據可視化相關的應用程式，設計演示數字雙胞胎的界面，並確保使用者可以輕鬆操作與互動。
使用圖神經網絡（GNN）進行藥物相關性的建模，以支援藥物發現與預測。
>>
# 工作分解結構清單

| 任務 | 任務名稱                | 需時（天） | 前置任務 | 主要負責人    |
| -------- | ----------------------- | ---------- | ------------ | ----------- |
| 1        | 設置玻璃箱              | 3          | -            | 組員 A      |
| 2        | Duo len 相機配置及安裝  | 5          | 1            | 組員 A      |
| 3        | 熱成像儀設置            | 3          | 1            | 組員 A      |
| 4        | 雷射與刺激裝置操作      | 4          | 1            | 組員 A      |
| 5        | mmWave 雷達設置         | 5          | 1            | 組員 A      |
| 6        | 數據收集設備組裝與測試  | 7          | 2, 3, 4, 5   | 組員 A      |
| 7        | 預測鼠類骨架姿態        | 10         | 6            | 組員 B, C   |
| 8        | DeepLabCut 姿態估測     | 7          | 7            | 組員 B, C   |
| 9        | 整合 HRNet 與 Swin Transformer | 10     | 8            | 組員 B, C   |
| 10       | 分析鼠類皮膚溫度        | 5          | 6            | 組員 B      |
| 11       | 分析鼠類心率和呼吸率    | 5          | 6            | 組員 B      |
| 12       | 使用 GAN 進行合成數據生成 | 10       | 9, 10, 11    | 組員 B, C   |
| 13       | 使用 GNN 進行藥物效應建模 | 12       | 12           | 組員 B, C   |
| 14       | 使用 VideoGPT 生成短視頻 | 10        | 12           | 組員 B, C   |
| 15       | 使用 MoCoGAN 生成視頻   | 10         | 14           | 組員 B, C   |
| 16       | 設計數據可視化演示      | 7          | 13, 15       | 組員 C      |
| 17       | 開發數字雙胞胎的界面    | 15         | 16           | 組員 A, C   |
| 18       | 使用 BERT 分析表型資料庫 | 10        | 13           | 組員 A, C   |
| 19       | 設計與開發數字雙胞胎模型 | 20        | 17, 18       | 組員 A, C   |
| 20       | 測試數字雙胞胎模擬結果  | 10         | 19           | 組員 A, C   |
| 21       | 項目計劃與時間表制定    | 5          | -            | 組員 C      |
| 22       | 項目進度跟蹤與調整      | 10         | 21           | 組員 C      |
| 23       | 制定預算計劃            | 5          | 21           | 組員 C      |
| 24       | 資金使用監控與報告      | 10         | 23           | 組員 C      |
| 25       | 數據收集設備性能測試    | 7          | 6            | 組員 A, B   |
| 26       | 神經網絡模型準確度測試  | 7          | 13           | 組員 A, B   |
| 27       | 編寫數據分析報告        | 10         | 26           | 組員 A, C   |
| 28       | 編寫模型驗證報告        | 10         | 26           | 組員 A, C   |
| 29       | 準備最終成果演示        | 7          | 27, 28       | 組員 A, C   |
| 30       | 向相關機構展示項目成果  | 5          | 29           | 組員 A, C   |

## 專題PERT/CPM圖

```mermaid
gantt
dateFormat  YYYY-MM-DD
section 設置與安裝
任務1: done, 2024-10-01, 3d
任務2: after task1, 5d
任務3: after task1, 3d
任務4: after task1, 4d
任務5: after task1, 5d
任務6: after task2, task3, task4, task5, 7d

section 數據分析與模型開發
任務7: after task6, 10d
任務8: after task7, 7d
任務9: after task8, 10d
任務10: after task6, 5d
任務11: after task6, 5d
任務12: after task9, task10, task11, 10d
任務13: after task12, 12d
任務14: after task12, 10d
任務15: after task14, 10d

section 數據可視化與應用開發
任務16: after task13, task15, 7d
任務17: after task16, 15d
任務18: after task13, 10d
任務19: after task17, task18, 20d
任務20: after task19, 10d

section 項目管理與測試
任務21: 2024-10-01, 5d
任務22: after task21, 10d
任務23: after task21, 5d
任務24: after task23, 10d
任務25: after task6, 7d
任務26: after task13, 7d
任務27: after task26, 10d
任務28: after task26, 10d
任務29: after task27, task28, 7d
任務30: after task29, 5d

``````


