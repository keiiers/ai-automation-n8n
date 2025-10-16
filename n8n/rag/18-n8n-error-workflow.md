> 🌍 **Language / 语言 / 語言**: [🇺🇸 English](./readme-en.md) | [🇨🇳 简体中文](./readme-cn.md) | [🇹🇼 繁体中文](./readme.md)
# 8 分鐘學會 n8n 錯誤處理工作流 Error Workflow！3大通知方法 LINE、Email、Google Sheet 即時掌握 99% 的錯誤｜🧠 省力知識庫[![YouTube](https://img.shields.io/badge/Watch%20on-YouTube-red?logo=youtube)](https://youtu.be/Yt0gVZX_OGQ)

![n8n 錯誤處理工作流](https://github.com/qwedsazxc78/ai-automation-n8n/blob/main/n8n/18-n8n-error-workflow/cover.png?raw=true)

## 作者資訊

* **作者：** Alexhsieh
* **平台：** n8n（您可以將 `.json` 檔導入自己的 n8n 環境，查看完整流程與設定）
* **注意事項：** 範例檔案已移除所有 API 金鑰與個資，使用時請自行填寫

---

## 📌 功能介紹

此 n8n 錯誤處理工作流（Error Workflow）適用於任何 n8n 自動化腳本與流程中，幫助您即時監控並掌握 99% 工作流異常！

* ✅ **Email（HTML郵件）即時通知**：自動發送包含錯誤類型與詳細訊息的 HTML 郵件，快速鎖定問題來源。
* ✅ **Google Sheet 完整紀錄**：將每一次錯誤發生的所有執行細節記錄於 Google Sheet，便於長期追蹤、報表統計與問題歸檔。
* ✅ **LINE Messenger 即時推播**：當重大錯誤發生時，馬上推播至 LINE，讓你隨時隨地掌握系統狀態，迅速反應！

---

## 🔧 運作方式

1. **工作流設定錯誤處理**：工作流必須切換為 Active，並設定 Error Workflow 工作流。只有在正式啟用下，錯誤通知才能自動觸發。
2. **模擬錯誤產生**：藉由 Schedule Trigger 每 30 秒發送一個故意設成無效網址的 HTTP Request，模擬真實錯誤情境。
3. **多元通知流程**：
   - **Email 通知**：錯誤發生，自動寄出 HTML 郵件，主旨自訂、內容清楚標示所有錯誤細節。
   - **Google Sheet 紀錄**：利用 Google Sheet 同步記錄錯誤出現的時間、Workflow 名稱、URL、執行 ID與錯誤內容。
   - **LINE 即時推播**：整合 LINE Messaging API，推送包含錯誤簡述與追蹤連結的訊息，錯誤不漏接！
4. **靈活選擇搭配**：根據通知急迫性與用途，配合不同管道單獨或組合運用。

---

## 🚀 通知方式選擇建議

* 需即時反應 ➔ 選 LINE！
* 減少干擾、例行記錄 ➔ 用 Email。
* 想長期統計、維運管理 ➔ Google Sheet。

> ⏰ **小提醒：** 測試時請記得必須「啟用 workflow」而非僅按測試按鈕，否則 Error Workflow 不會啟動！如需串接 LINE 請參考上一集完整教學。[![YouTube](https://img.shields.io/badge/Watch%20on-YouTube-red?logo=youtube)](https://youtu.be/HJKDHJ5x1F0)

---

## 延伸學習資源

* [n8n 官方說明](https://docs.n8n.io/)
* [上一集：8分鐘學會 n8n 串接 LINE Messenger API](https://youtu.be/HJKDHJ5x1F0)
* [Google Sheet API 教學](https://developers.google.com/sheets/api)


---

## 🚀 快速上手 n8n 自動化資源懶人包

### 🎓 學習與社群

* 🔗 [加入 AI 學習社群 (Skool)](https://www.skool.com/ai-brain-alex/about?ref=5dde9b20e8e7432aa9a01df6e89685f4)
  建立學習 AI 與 n8n 的學習路徑，無痛上手！
* 🔗 [加入 Line 社群一起搞懂 AI](https://line.me/ti/g2/ZypIgLSzVPweRBgBqKvaRU10WEmnotuZOr7Lpg)
  互相幫助前進！打造自己的 AI 自動化場景！

### 📚 教學資源

* 🎥 [n8n AI 自動化工作流：從基礎到進階實戰](https://youtube.com/playlist?list=PLUf88uk7T54I83MBdbuXgUuA8rVklF4FA&si=wHsQw8YJu-erSdLd)
  YouTube 系列教學，邊看邊做快速上手！
* ⏱️ [碎片化時間學習 n8n](https://youtube.com/playlist?list=PLUf88uk7T54Iv6LV2NFgdTghaX2cPhtgH&si=G3gj2qn179ZFUqAZ)
  每天5分鐘學習，自動化養成沒負擔。

### 🛠️ 部署與工具

* 🧩 [zeabur n8n 部署模板 (隨時更新)](https://zeabur.com/zh-TW/templates/0TUVZ7?referralDesktop=qwedsazxc78)
  零架設壓力，點擊部署即可使用，適合初學者與進階用戶。
* 🌐 [n8n 官方網站](https://n8n.io/)
  了解更多功能與文件，掌握最新更新。
