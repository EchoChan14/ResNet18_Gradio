# 🍱 AI 美食分類與中文說明系統

本專案使用 `ResNet18` 深度學習模型，搭配 `Gradio` 建立一個可互動的「美食分類 + 說明查詢」AI 系統，使用者可上傳食物圖片，即時獲得分類結果與對應的繁體中文解說。

## 📌 功能特色

- 🧠 使用 ResNet18 預訓練模型進行圖片分類（10 種食物）
- 🗂️ 自建 `food_info.csv` 中文食物說明資料表
- 🖼️ 上傳圖片即顯示 Top-3 預測結果
- 📘 對應說明顯示該食物的歷史與成分簡介
- 🌐 搭配 Gradio 建立 Web 介面，可即時互動

## 📦 資料集來源

本專案所使用之圖片資料集為：

- [📁 Kaggle - Food-101 Tiny Dataset](https://www.kaggle.com/datasets/kmader/food41)
- 精選 10 類常見食物，每類約 150 張圖片（train/valid/test）

若您使用此專案發表公開內容，請適度註明原始資料來源以尊重原作者。

資料圖片版權原始出處屬於 Food-101 作者 / Kaggle 資料集提供者。

## 👨‍🔬 專案作者

- 作者：Echo6514  
- 學校：國立臺北護理健康大學 資訊管理研究所  
- 聯絡方式：GitHub ➜ [EchoChan14](https://github.com/EchoChan14)  
- 特別感謝：ChatGPT 協助架構、Gradio 團隊、PyTorch 社群


## 📂 專案結構

| 檔案名稱                   | 說明                         |
|----------------------------|------------------------------|
| `Resnet_Gradio.ipynb`      | 主程式，執行 Gradio demo ✅ |
| `food_resnet_train.ipynb`  | ResNet18 模型訓練流程        |
| `food_resnet_predict.ipynb`| 圖片分類 + 說明測試程式     |
| `food_info.csv`            | 食物名稱與中文說明資料表    |
| `resnet18_food.pth`        | 訓練完成的模型參數檔         |

## 🚀 使用方式

```bash
# 安裝必要套件
pip install torch torchvision gradio pandas

MIT License
本專案開源，歡迎自由使用、修改、學習，僅需保留原始作者名稱與出處，禁止未經授權之商業行為。
