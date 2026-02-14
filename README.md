# n8n 自動化工作流教學資源庫 (n8n Teaching Resources)

歡迎來到本專案！這裡存放了 **n8n 自動化工作流** 教學相關的教材與程式碼檔案，旨在幫助學習者快速上手 Agentic AI 與工作流自動化。

---

## 📁 檔案目錄與說明

### 1. 核心教材 (Main Presentation)
* **`myn8n.pptx`**：**請先開啟此檔案**。這是本課程的主要教學簡報，涵蓋了自動化工作流的核心概念與架構說明。

### 2. n8n 工作流檔案 (Workflow JSONs)
所有的 `.json` 檔案都是 **n8n 的程式主體**。您可以將它們一個一個匯入 (Import) 到您的 n8n 環境中使用。

| 檔案名稱 | 說明 |
| :--- | :--- |
| `1First AI Agent.json` | 初探 AI 代理人工作流 |
| `2Chat_cal.json` | 日曆對話機器人基礎 |
| `3Chat_Cal_Webhook.json` | 透過 Webhook 觸發的日曆助手 |
| `4RAG004.json` | RAG (檢索增強生成) 實作範例 |
| `5ImageToFB.json` | 圖像生成並自動發佈至 Facebook |
| `6Financial Times RSS.json` | 金融時報 RSS 新聞抓取自動化 |
| `7iPhone Assistant.json` | iPhone 專用助手整合 |
| `8 11LabsVoiceAgent.json` | ElevenLabs 語音合成代理人 |
| `9nanoBanana.json` | 使用 Nano Banana 模型進行多模態應用 |
| `61Schedule...mes RSS.json` | 排程型新聞自動化工作流 |

### 3. 前端網頁介面 (Frontend HTMLs)
所有的 `.html` 檔案皆為**網頁版的前端介面**，用於模擬真實應用的前後端互動邏輯：
1. **輸入資料**：使用者在瀏覽器開啟 `.html` 檔案並輸入指令。
2. **資料傳輸**：前端透過 **Webhook** 將資料傳送給對應的 n8n 工作流（`.json` 檔案）。
3. **Webhook**：目前程式中的 Webhook 皆為虛構的，請一定要更新為你自己的 Webhook。
4. **執行與回傳**：n8n 執行邏輯後，將結果傳回前端網頁顯示。


*重點檔案：* `rag_frontend.html` / `rss_news.html` / `fb_post.html` / `nanoB_...html` 系列。

---

## 🚀 使用指南

1. **閱讀簡報**：開啟 `myn8n.pptx` 掌握整體教學脈絡。
2. **匯入 n8n**：
   * 開啟您的 n8n 介面。
   * 點選 **Workflows** -> **Import from File**，選擇本專案中的 `.json` 檔案。
3. **部署前端**：
   * 在瀏覽器中直接開啟 `.html` 檔案。
   * **注意**：請確保 HTML 檔案中的 `Webhook URL` 已修改為您在 n8n 產生的 Production URL。

---

## 🛠 系統需求
* [n8n](https://n8n.io/) 
* 現代化瀏覽器 (Chrome / Edge / Firefox)

** 欒老師 (Prof. Luarn)
```diff

- 目前程式中的 Webhook 皆為虛構的，請一定要更新為你自己的 Webhook才能正確執行。
