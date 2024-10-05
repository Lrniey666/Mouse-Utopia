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
組員 B：數據分析與模型訓練

使用收集到的數據來訓練神經網絡，包括預測心率、皮膚溫度和行為姿態等模型。
利用 DeepLabCut 進行姿態估測，並結合 HRNet 和 Swin Transformer 增強精準度。
訓練生成模型，如 VideoGPT 和 MoCoGAN，來模擬和生成實驗鼠行為的短片，以構建數字雙胞胎。
組員 C：數據後處理與應用開發

使用自然語言處理技術（例如 BERT、GPT-3）分析鼠類表型資料庫（Mouse Phenome Database），為藥物效應預測提供支持。
開發與數據可視化相關的應用程式，設計演示數字雙胞胎的界面，並確保使用者可以輕鬆操作與互動。
使用圖神經網絡（GNN）進行藥物相關性的建模，以支援藥物發現與預測。
