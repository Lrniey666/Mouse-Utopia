
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
## 專案工作分解結構清單

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

## 專案PERT/CPM圖

```mermaid
graph TD
    A1[任務1: 設置玻璃箱] --> A2[任務2: Duo len 相機配置及安裝]
    A1 --> A3[任務3: 熱成像儀設置]
    A1 --> A4[任務4: 雷射與刺激裝置操作]
    A1 --> A5[任務5: mmWave 雷達設置]
    A2 --> A6[任務6: 數據收集設備組裝與測試]
    A3 --> A6
    A4 --> A6
    A5 --> A6
    A6 --> A7[任務7: 預測鼠類骨架姿態]
    A7 --> A8[任務8: DeepLabCut 姿態估測]
    A8 --> A9[任務9: 整合 HRNet 與 Swin Transformer]
    A6 --> A10[任務10: 分析鼠類皮膚溫度]
    A6 --> A11[任務11: 分析鼠類心率和呼吸率]
    A9 --> A12[任務12: 使用 GAN 進行合成數據生成]
    A10 --> A12
    A11 --> A12
    A12 --> A13[任務13: 使用 GNN 進行藥物效應建模]
    A12 --> A14[任務14: 使用 VideoGPT 生成短視頻]
    A14 --> A15[任務15: 使用 MoCoGAN 生成視頻]
    A13 --> A16[任務16: 設計數據可視化演示]
    A15 --> A16
    A16 --> A17[任務17: 開發數字雙胞胎的界面]
    A13 --> A18[任務18: 使用 BERT 分析表型資料庫]
    A17 --> A19[任務19: 設計與開發數字雙胞胎模型]
    A18 --> A19
    A19 --> A20[任務20: 測試數字雙胞胎模擬結果]
    A21[任務21: 項目計劃與時間表制定] --> A22[任務22: 項目進度跟蹤與調整]
    A21 --> A23[任務23: 制定預算計劃]
    A23 --> A24[任務24: 資金使用監控與報告]
    A6 --> A25[任務25: 數據收集設備性能測試]
    A13 --> A26[任務26: 神經網絡模型準確度測試]
    A26 --> A27[任務27: 編寫數據分析報告]
    A26 --> A28[任務28: 編寫模型驗證報告]
    A27 --> A29[任務29: 準備最終成果演示]
    A28 --> A29
    A29 --> A30[任務30: 向相關機構展示項目成果]
``````
## 專案甘特圖

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Mouse Utopia Project Plan
    excludes weekends

    section 設置與安裝
    設置玻璃箱: a1, 2024-10-03, 3d
    Duo len 相機配置及安裝: a2, after a1, 5d
    熱成像儀設置: a3, after a1, 3d
    雷射與刺激裝置操作: a4, after a1, 4d
    mmWave 雷達設置: a5, after a1, 5d
    數據收集設備組裝與測試: a6, after a2 a3 a4 a5, 7d

    section 數據分析與模型開發
    預測鼠類骨架姿態: b1, after a6, 10d
    DeepLabCut 姿態估測: b2, after b1, 7d
    整合 HRNet 與 Swin Transformer: b3, after b2, 10d
    分析鼠類皮膚溫度: b4, after a6, 5d
    分析鼠類心率和呼吸率: b5, after a6, 5d
    使用 GAN 進行合成數據生成: b6, after b3 b4 b5, 10d
    使用 GNN 進行藥物效應建模: b7, after b6, 12d
    使用 VideoGPT 生成短視頻: b8, after b6, 10d
    使用 MoCoGAN 生成視頻: b9, after b8, 10d

    section 數據可視化與應用開發
    設計數據可視化演示: c1, after b7 b9, 7d
    開發數字雙胞胎的界面: c2, after c1, 15d
    使用 BERT 分析表型資料庫: c3, after b7, 10d
    設計與開發數字雙胞胎模型: c4, after c2 c3, 20d
    測試數字雙胞胎模擬結果: c5, after c4, 10d

    section 項目管理與測試
    項目計劃與時間表制定: d1, 2024-10-03, 5d
    項目進度跟蹤與調整: d2, after d1, 10d
    制定預算計劃: d3, after d1, 5d
    資金使用監控與報告: d4, after d3, 10d
    數據收集設備性能測試: d5, after a6, 7d
    神經網絡模型準確度測試: d6, after b7, 7d
    編寫數據分析報告: d7, after d6, 10d
    編寫模型驗證報告: d8, after d6, 10d
    準備最終成果演示: d9, after d7 d8, 7d
    向相關機構展示項目成果: d10, after d9, 5d
``````

