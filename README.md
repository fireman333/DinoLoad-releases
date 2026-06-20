# DinoLoad 🦖

> macOS 桌面像素寵物 — 用「照顧一隻會餓的寵物」幫你養成清理 Downloads、專注、習慣的好習慣。

這個 repo **只放可下載的安裝檔（DMG）**，原始碼為私有。要安裝請到 👉 **[Releases](../../releases/latest)** 下載最新版的 `DinoLoad-x.y.z.dmg`。

---

## 安裝

DinoLoad 是免費測試版，還沒做 Apple 公證 (notarization)，所以直接雙擊會被 macOS 擋（「來自未經驗證的開發者」）。這不是病毒 —— 照下面**四個步驟**做，一定能裝起來：

**1.** 從上面的 **Releases** 下載 `DinoLoad-x.y.z.dmg`，**雙擊打開**它（會出現一個叫「DinoLoad」的磁碟）。

**2.** 打開「**終端機**」(Terminal)：按 `⌘ + 空白鍵` 開 Spotlight，輸入「終端機」按 Enter。

**3.** 把下面這**一整行**複製貼上到終端機，按 **Enter**：

```bash
cp -R "/Volumes/DinoLoad/DinoLoad.app" /Applications/ && xattr -cr "/Applications/DinoLoad.app" && open "/Applications/DinoLoad.app"
```

**4.** 完成！DinoLoad 會自動裝進「應用程式」並啟動。

> 這行做的事：把 app 複製到「應用程式」→ 清掉 macOS 的隔離標記（這步就是繞過「未驗證開發者」阻擋的關鍵）→ 啟動。之後直接從「應用程式」開即可，不用再跑一次。

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
