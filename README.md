# DinoLoad 🦖

> macOS 桌面像素寵物 — 用「照顧一隻會餓的寵物」幫你養成清理 Downloads、專注、習慣的好習慣。

這個 repo **只放可下載的安裝檔（DMG）**，原始碼為私有。要安裝請到 👉 **[Releases](../../releases/latest)** 下載最新版的 `DinoLoad-x.y.z.dmg`。

---

## 安裝（重要）

DinoLoad 目前是**免費測試版**，還沒做 Apple 公證 (notarization)，所以第一次打開 macOS 會跳「**無法打開，因為來自未經驗證的開發者**」。這不是病毒警告 —— 只是 Apple 對未付費認證的 app 一律這樣擋。

> ⚠️ **重點**：不要直接對 DMG 裡的 app 解除隔離 —— DMG 是唯讀的會報錯。正確做法是**先複製到「應用程式」，再解除阻擋**。

### 方法一（最簡單、一定成功）：終端機貼一行
打開下載的 DMG 後，打開「終端機」(Terminal)，貼上這行按 Enter：

```bash
cp -R "/Volumes/DinoLoad/DinoLoad.app" /Applications/ && xattr -cr "/Applications/DinoLoad.app" && open "/Applications/DinoLoad.app"
```

複製到「應用程式」→ 清掉隔離標記 → 啟動。

### 方法二：用終端機跑內附的安裝腳本
打開「終端機」，輸入 `bash` 再空一格，把 DMG 裡的 `安裝.command` **拖**進終端機視窗，按 Enter。（用 `bash` 執行腳本不會被 Gatekeeper 擋；雙擊才會。）

### 方法三：雙擊 `安裝.command`
在 macOS 15 (Sequoia) 以上常會被擋（「系統不允許」）。被擋就改用方法一或方法二。DMG 裡的 `必讀-安裝說明.txt` 有完整說明。

---

## 系統需求

- macOS 13 (Ventura) 以上
- Universal binary：**Apple Silicon（M 系列）與 Intel Mac 都能跑**

## 安裝完之後

- DinoLoad 是**選單列小工具**（不在 Dock）。寵物浮在桌面，選單列右上角有 🦖，要退出從那裡選。
- 第一次啟動會請你授權「下載項目」資料夾與（選用的）行事曆／提醒事項權限。
- 拿到 30 碼解鎖代碼的話，到 **設定 → 寵物 → 更衣室 → 解鎖代碼** 貼上按「兌換」解鎖動物。

## 回報問題

測試遇到狀況，回報給提供測試版的人即可。祝清理愉快！
