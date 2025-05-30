# 🍱 AI 美食分類與中文說明系統

本專案使用 `ResNet18` 深度學習模型，搭配 `Gradio` 建立一個可互動的「美食分類 + 說明查詢」AI 系統，使用者可上傳食物圖片，即時獲得分類結果與對應的繁體中文解說。

## 📌 功能特色

- 🧠 使用 ResNet18 預訓練模型進行圖片分類（10 種食物）
- 🗂️ 自建 `food_info.csv` 中文食物說明資料表
- 🖼️ 上傳圖片即顯示 Top-3 預測結果
- 📘 對應說明顯示該食物的歷史與成分簡介
- 🌐 搭配 Gradio 建立 Web 介面，可即時互動


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
