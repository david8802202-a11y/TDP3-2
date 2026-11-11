# 記憶德州

記憶 + 德州撲克的多人卡牌遊戲。主桌用 iPad 或電腦開網頁，玩家用手機掃 QR code 加入，不需要帳號。

## 檔案

- `index.html`：多人模式。直接開是主桌，網址帶 `?room=房號` 時是玩家手機畫面。
- `solo.html`：單人練習。

## 上傳到 GitHub Pages

1. 在 GitHub 建立一個新的 repository，例如 `memory-holdem`，設為 Public。
2. 進入 repository，按 **Add file → Upload files**，把 `index.html`、`solo.html`、`README.md` 拖進去，按 **Commit changes**。
3. 到 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾 `/ (root)`，按 **Save**。
4. 等 1–2 分鐘，頁面上方會出現網址，格式是 `https://你的帳號.github.io/memory-holdem/`。

## 玩法

1. 主桌開上面的網址，畫面會出現 QR code 和 5 碼房號。
2. 玩家用手機掃碼，輸入暱稱加入。人數不限，隨時可以加入。
3. 主桌按「開始」：16 張牌翻開 20 秒，所有人看主桌記牌。
4. 蓋牌後亮出 3 張公牌，玩家在手機上選 2 張（A–P），20 秒內按確認。
5. 所有在線玩家都確認，或時間到，主桌公布每個人的牌型與排名，冠軍累計勝場。

## 注意事項

- 主桌的分頁要一直開著，關掉或重新整理就是新房間，玩家要重掃。
- 連線使用 PeerJS 的免費公用配對伺服器，偶爾可能不穩。大家連同一個 Wi-Fi 最穩定。
- 玩家手機斷線會自動重連，勝場會保留（同一支手機、同一個瀏覽器）。
- 必須透過 GitHub Pages 的網址開啟；直接雙擊本機檔案，手機無法掃碼連入。
