# YOLOv11 Toyota Logo Detection 專案

本專案為【深度學習課程期末專案】，以 YOLOv11 模型實作 Toyota 車標自動偵測，涵蓋資料蒐集、標註、訓練、成果展示等完整流程。

---

## 🎥 專案成果影片

[![Yt連結](https://www.youtube.com/watch?v=JRGKaWM_o38)

👉 點擊上方影片可觀看專案成果展示！

---

## 📁 專案結構
yolov11/
├── 412777095_Toyota.ipynb # 專案 Jupyter 筆記本
├── data.yaml # YOLO 設定
├── toyota_dataset/ # 訓練/驗證資料集與標註
│ ├── images/train/
│ ├── images/val/
│ ├── labels/train/
│ ├── labels/val/
├── toyota_logo_project/ # 訓練成果圖表、模型檔
├── runs/ # YOLO 自動產生推論結果
├── yolo11n.pt # YOLOv11 預訓練權重

---

## 🧰 執行環境

- Python 3.8+
- Ultralytics
- YOLOv11
- torch, torchvision
- numpy, opencv, matplotlib, tqdm, jupyter


## 🚀 使用方式

1. **準備資料集**
    - 圖片與標註請依 YOLO 格式放在 `toyota_dataset/` 下。

2. **訓練模型**
    - 於 Jupyter Notebook 執行 `412777095_Toyota.ipynb`，依內部說明調整訓練參數。

3. **推論展示**
    - 成果圖表與推論影像可於 `toyota_logo_project/` 或 `runs/` 目錄中查看。

4. **成果影片**
    - 可點擊 README 頂部的 YouTube 連結觀看偵測實際效果。

---

## 📊 專案亮點

- 自建 Toyota logo 資料集並標註
- YOLOv11 物件偵測流程完整實作
- 成果圖表齊全：混淆矩陣、PR 曲線、推論影像
- YouTube 影片直觀展示專案實力

---

## 💡 學習心得 / 經驗

- 實作深度學習物件偵測的完整 pipeline
- 了解資料標註對訓練結果的重要性
- 學習自動化訓練與結果評估流程

---
## 💡 專案反思

- 雖然最終的預測成果在部分影片段落能準確辨識 Toyota logo 並持續追蹤超過五秒，但整段影片的偵測表現還有明顯進步空間。
- 主要原因包含：
    - 資料集規模有限，圖片多樣性與標註數量不足，導致模型泛化能力不佳。
    - 訓練時尚未進行更多模型優化（如更換 backbone、超參數調整、資料增強等）。
    - 尚未嘗試進階後處理（如追蹤演算法、閾值微調）提升影片偵測連續性。
- 若有機會繼續優化，會考慮蒐集更多樣本、實作數據增強與模型調參，並結合影片物件追蹤技術，提升整體表現。







