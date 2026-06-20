# DinoLoad 🦖

> macOS 桌面像素寵物 — 用「照顧一隻會餓的寵物」幫你養成清理 Downloads、專注、習慣的好習慣。

這個 repo **只放可下載的安裝檔（DMG）**，原始碼為私有。要安裝請到 👉 **[Releases](../../releases/latest)** 下載最新版的 `DinoLoad-x.y.z.dmg`。

---

## 安裝（重要）

DinoLoad 目前是**免費測試版**，還沒做 Apple 公證 (notarization)，所以第一次打開 macOS 會跳「**無法打開，因為來自未經驗證的開發者**」。這不是病毒警告 —— 只是 Apple 對未付費認證的 app 一律這樣擋。用下面任一方法即可：

### 方法一（最簡單）：雙擊「安裝.command」
打開下載的 DMG → 雙擊裡面的 **`安裝.command`**。它會自動把 app 裝到「應用程式」、解除阻擋、並啟動。
若雙擊被擋：對 `安裝.command` 按右鍵 →「打開」→ 再按一次「打開」。

### 方法二（最保險）：終端機貼一行
打開「終端機」(Terminal)，貼上這行按 Enter：

```bash
xattr -dr com.apple.quarantine "/Volumes/DinoLoad/DinoLoad.app" && cp -R "/Volumes/DinoLoad/DinoLoad.app" /Applications/ && xattr -dr com.apple.quarantine "/Applications/DinoLoad.app" && open "/Applications/DinoLoad.app"
```

DMG 裡的 `必讀-安裝說明.txt` 有完整圖解與第三種（拖曳）方法。

---

## 系統需求

- macOS 13 (Ventura) 以上
- Universal binary：**Apple Silicon（M 系列）與 Intel Mac 都能跑**

## 安裝完之後

- DinoLoad 是**選單列小工具**（不在 Dock）。寵物浮在桌面，選單列右上角有 🦖，要退出從那裡選。
- 第一次啟動會請你授權「下載項目」資料夾與（選用的）行事曆／提醒事項，這些是餵食移檔與習慣功能需要的權限。
- 拿到 30 碼解鎖代碼的話，到 **設定 → 寵物 → 更衣室 → 解鎖代碼** 貼上按「兌換」解鎖動物。

## 回報問題

測試遇到狀況，回報給提供測試版的人即可。祝清理愉快！
