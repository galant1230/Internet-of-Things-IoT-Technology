# 🏥 室內跌倒防治系統 - 物聯網智慧監測

## 📌 Description
本專案致力於開發 **智慧穿戴式裝置**，透過 **ANT+** 偵測佩戴者的 **心率變化**，若系統發現異常，將立即通報給 **定位程式**，並使用 **MQTT 及 LINE Notify** 進行緊急通知。  
此外，系統整合 **iBeacon Library** 及 **雷達掃描技術** 來確定事故發生地點，並派遣 **小鴨車** 進行即時影像回傳，協助觀護人員做出即時應對。
[Demo](https://www.youtube.com/watch?v=svAmBd3rSOQ&ab_channel=RenTsai)

---

## 📥 System Workflow
### 1️⃣ **心率監測**
- **使用 ANT+ 技術** 監測穿戴裝置使用者的心率變化。
- 當系統偵測到心率異常，觸發 **MQTT 通知**。

### 2️⃣ **即時定位**
- 透過 **iBeacon Library** 確定使用者位置。
- **雷達掃描器 (Radar Scanner)** 透過 Java 程式過濾數據，確保定位準確性。

### 3️⃣ **緊急通知**
- 觸發 **LINE Notify** 自動傳送警報訊息。
- 透過 **MQTT** 即時傳輸事故地點資訊。

### 4️⃣ **小鴨車派遣**
- **小鴨車 (Duck Car)** 自動前往事故發生地點。
- 拍攝現場影像並回傳至監控系統，提供即時畫面給觀護人員。

---

## ⚙️ 技術架構
- **感測技術**：ANT+、Garmin Monitor
- **通訊技術**：MQTT、LINE Notify
- **定位技術**：iBeacon Library、Radar Location
- **行動偵測**：Movestick Mini
- **影像回傳**：小鴨車 (Duck Car)
- **設備控制**：Raspberry Pi

---

## 📊 Application & Benefits
- **長者照護**：即時監測獨居長者健康狀況，降低跌倒事故風險。
- **智慧居家**：結合 IoT 物聯網技術，打造更安全的居住環境。
- **自動化監測**：減少人力依賴，提高事故應變效率。

---

## 📎 References
- **MQTT Protocol**：[官方文件](https://mqtt.org/)
- **iBeacon 技術**：[Apple Developer 文檔](https://developer.apple.com/ibeacon/)
- **LINE Notify API**：[官方網站](https://notify-bot.line.me/en/)

