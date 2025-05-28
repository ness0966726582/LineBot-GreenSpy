# LineBot-GreenSpy
LINE 間諜幫你看地球

# LineBot-GreenSpy 🌿📲

一個結合 Google Earth Engine（GEE）、LINE Messaging API 與遙測資料的綠地指標查詢系統。  
使用者只需在 LINE 上輸入行政區名稱（如「新北市」），即可即時獲得該區最新的綠地覆蓋率與 NDVI 地圖。

---

## 🚀 專案特色

- 查詢台灣任一行政區的綠地百分比
- 使用 GEE 自動計算 NDVI（植生指數）
- 自動產圖並回傳到 LINE
- 可搭配 Make 自動定時發送報表或通知

---

## 🛠 使用技術

- Google Earth Engine（遙測影像分析）
- LINE Messaging API（聊天機器人平台）
- Make（自動化流程）
- Google Sheets / Google Drive（資料儲存與共享）

---

## 📁 專案結構

```
green-index-taiwan/
├── gee_scripts/         # GEE NDVI 腳本
├── make_scenarios/      # Make 自動化流程設定圖 or 說明
├── linebot/             # LINE webhook 程式碼
├── images/              # 輸出圖像範例
├── data/                # 測試用 GeoJSON、行政區資料
├── README.md            # 本說明文件
├── LICENSE              # 授權條款（建議用 MIT）
└── .env.example         # 環境變數範例（不含機密資訊）
```

---

## 🖼 使用展示

> LINE 回覆範例：
> 
> 🟢 新北市 2024/05/27 綠地覆蓋率為 32.7%  
> ![NDVI Map Example](images/ndvi_newtaipei_sample.png)

---

## ⚙️ 如何啟用

1. 設定 Google Earth Engine 帳號
2. 將腳本上傳至 GEE，並設定區域與輸出方式
3. 設定 Make webhook 接收 LINE 訊息並呼叫 GEE
4. 設定 LINE Bot，啟用 Webhook
5. 測試訊息：「新北市」

---

## 🧠 延伸應用

- 自動每週生成 NDVI 趨勢報告
- 結合 IoT 感測資料
- 做成 ESG 綠地監控平台

---

## 📜 LICENSE

MIT License — Feel free to use, improve, and save the planet.

---

> 「桌子看了地球，地球也在看我們。」🌍
