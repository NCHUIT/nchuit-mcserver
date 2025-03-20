# NCHUIT-MCServer
*查看不同語言的 README 文件：[English](README.md)*

## 📋 介紹
這是國立中興大學資訊科學研習社官方 Minecraft 伺服器！

本伺服器是模組服，我們使用 [Manual-MMDM](https://github.com/coke5151/manual-mmdm) 來管理並分別匯出客戶端/伺服端模組。

## 🎮 遊戲資訊
- **遊戲版本**：`1.19.2`
- **模組載入器**：`Forge`
- **Forge 版本**：`1.19.2-43.4.0`
- **伺服器位址**：`nchuit.ddns.net`
- **記憶體需求**：建議分配至少 4GB 以上的 RAM 給遊戲

## 📊 模組列表與依賴關係
你可以在 [dependency-tree.txt](./manual-mmdm/dependency-tree.txt) 檔案中找到所有模組的完整列表及其依賴關係。這個檔案是由 Manual-MMDM 工具自動生成的，提供以下詳細資訊：
- 伺服器包含的所有模組
- 每個模組的版本資訊
- 模組之間的依賴關係

## 📥 客戶端遊玩
> 💡 **安裝圖文說明**在 [HackMD](https://hackmd.io/@113team/S1zUeqdQyg)

### 系統需求
- **1.19.2 需要 Java 17 或更新的版本**

### 安裝方法
#### 使用 Prism Launcher（推薦）：
1. 請在 Release 區下載 Prism-Launcher 開頭的 `.zip` 檔案
2. 直接將**壓縮檔**匯入 Prism Launcher 中（不需要解壓縮）
3. 設定 RAM 及 Java

#### 手動安裝（官方啟動器）：
1. 請安裝指定的 Forge 版本
2. 從 Release 下載 Client-Mods 開頭的 `.zip` 檔
3. 解壓縮後將模組丟到 `.minecraft/mods` 資料夾中
4. 設定好你的 Minecraft 啟動器，確保開啟的是 Forge 版本，並且分配至少 3GB 的記憶體給遊戲

## 🖥️ 架設伺服器
- 推薦使用新版的 [Adoptium 發行版](https://adoptium.net/)而非 OpenJDK

### 步驟
1. 下載 Server-Template 開頭的 `.zip` 檔，並解壓縮
2. 編輯 `user_jvm_args.txt`，設定要分配的 RAM，推薦至少 6GB
3. Windows 執行 `run.bat` / Linux 執行 `run.sh` 來執行伺服器！

> ⚠️ **注意**：第一次執行時會生成 `eula.txt` 檔案，記得修改檔案同意條款再重新開啟伺服器！（這步就跟所有 Minecraft 伺服器開服過程一樣，詳情可以上網搜尋教學）

## 🔧 模組管理
請下載最新版的 [Manual-MMDM](https://github.com/coke5151/manual-mmdm) 後，放置到 manual-mmdm 資料夾中使用，並且所有被管理的模組應放在 `manual-mmdm/mods` 中。

> ⚠️ **重要提醒**：請務必在提交（commit）變更前，使用 Manual-MMDM 工具中的「匯出 JSON」和「生成依賴樹」功能。這能確保所有模組的依賴關係都被正確記錄和追蹤。建議將生成的 dependency-tree 檔案置放在專案根目錄，並將 manual-mmdm.json 放置在 manual-mmdm 資料夾中。

## 📦 發佈指南
如果你是模組包編輯者，在更動了模組之後想要發佈 Release，請你準備好以下檔案：

1. `Client-Mods-<tag>.zip`：內容為使用 [Manual-MMDM](https://github.com/coke5151/manual-mmdm) 匯出的所有客戶端 Mods。
2. `Prism-Launcher-<tag>.zip`：將 Manual-MMDM 匯出的客戶端模組放置到 Repository 的 `prism-launcher-template/minecraft/mods` 中，之後將整個 `prism-launcher-template` 資料夾壓縮並重新命名。
3. `Server-Template-<tag>.zip`：從本 Repository 的 `server-template` 資料夾下載伺服器模板後，將 Manual-MMDM 匯出的伺服器模組放到 `server-template/mods` 中。這個壓縮檔解壓縮後應為整個伺服器模板 + 模組。

**提交前檢查清單**：
- 使用 Manual-MMDM 工具中的「匯出 JSON」功能更新模組資訊
- 使用「生成依賴樹」功能記錄模組間的依賴關係
- 確認所有變更都已正確記錄後再進行提交

## ❓ 常見問題 (FAQ)
1. **問題**：遊戲啟動時出現記憶體不足錯誤  
   **解決方案**：確保已分配足夠的 RAM 給 Minecraft（至少 3GB）

2. **問題**：無法連接到伺服器  
   **解決方案**：確認伺服器地址輸入正確，並檢查你的網路連線是否正常

3. **問題**：模組顯示版本不相容  
   **解決方案**：確保你使用的是正確的Forge和Minecraft版本（1.19.2 和 Forge 1.19.2-43.4.0）

## 📞 聯絡我們
如有任何問題或建議，歡迎透過以下方式聯絡我們：
- 電子郵件：[it.nchu@gmail.com](mailto:it.nchu@gmail.com)
- 社團網站：[nchuit.com](https://nchuit.com/)

## 📜 授權條款
本專案採用 MIT 授權條款 - 詳情請參閱 [LICENSE](LICENSE) 檔案。