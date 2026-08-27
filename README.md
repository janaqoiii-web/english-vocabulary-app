# 📚 SRS Vocab Master - 漸進式間隔重複單字卡 App

![PWA Ready](https://img.shields.io/badge/PWA-Ready-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

**SRS Vocab Master** 是一款結合 **萊特納間隔重複系統（Spaced Repetition System, SRS）** 與 **AI 語音辨識/發音** 的高效英語單字記憶應用程式。支援跨平台（iOS, Android, Desktop）作為 PWA 離線使用，或打包為原生 APP。

---

## ✨ 核心功能亮點

* 🧠 **科學間隔重複記憶 (SRS)**：自動規劃單字複習週期（S-1 至 S-5 記憶階段），根據記憶品質自動升級或重置階段。
* 🎧 **聽力與拼字測驗**：
  * 提供「今日重溫」、「已學單字」、「全部單字」及「自選範圍」等靈活測驗模式。
* 🗣️ **口說朗讀評分**：
  * 支援瀏覽器原生 WebSpeech API 語音辨識。
  * 支援免麥克風「🧪 模擬試讀」測試模式。
  * 可擴充整合 **OpenAI Whisper API / 雲端 STT**，徹底解決行動裝置 WebView 語音權限限制。
* 💾 **單字庫管理與資料轉移**：
  * 支援手動新增/編輯單字，自動比對重複單字與防誤覆蓋提醒。
  * 支援 **JSON**（完整學習紀錄備份）與 **CSV**（試算表編修）匯入/匯出。
* 🔔 **每日定時溫習提醒**：內建 Web Audio 提示音效（水晶和弦、溫和木琴等）與系統推播通知。
* 📱 **PWA 與離線支援**：完全支援離線使用、加至桌面全螢幕運作，並可無縫打包上架 Store。

---

## 📂 專案檔案結構

```text
├── index.html        # 主程式 (UI 介面與完整應用邏輯)
├── manifest.json     # PWA 設定檔
├── sw.js             # Service Worker 離線快取引擎
├── SRS-192.png       # 192x192 應用程式圖示
└── SRS.png           # 512x512 高解析度啟動圖示
