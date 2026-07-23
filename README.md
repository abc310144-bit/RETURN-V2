# UrMart 退貨優化 V2

UrMart 後台退貨流程原型（Demo）V2 版本，在 V1 基礎上新增**自動派車**相關功能。本資料夾為獨立可執行的打包版本。

## 功能特色

- V1 全部退貨流程（建立退貨、退貨單檢視、退貨管理列表）
- 退貨單詳情頁**派車 / 編輯派車 / 取消派車**
- 派車設定（取件日期、溫層規格、收寄件人等）
- 16:30 鎖單、17:00 取件日規則與相關提示彈窗
- Demo 測試時間面板（左下角）

## 快速開始

1. 下載或 clone 本專案
2. 雙擊開啟 `退貨 V2 index.html`（需與同目錄的 `app.js` 放在一起）
3. 首次載入需網路連線（Tailwind CDN）

## 原始碼與打包

React 原始碼位於同層的 `退貨優化 V 1 新增退貨按鈕` 專案。V2 透過 `window.__RETURN_APP_VARIANT__ = 'v2'` 啟用 V2 功能。

在 V1 專案目錄執行：

```bash
npm install
npm run build:standalone
```

再將產出的 `app.js` 複製至本資料夾覆蓋即可更新 Demo。

## 專案結構

```
├── 退貨 V2 index.html    # V2 入口
├── app.js                # 打包後的獨立執行檔
└── README.md
```

## 授權

MIT License
