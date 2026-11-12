# 熊本福岡 冬日小旅行 12/9–12/16

一個單一 HTML 檔的旅遊行程網站(日系繪本風),內容包含:首頁倒數、航班、每日行程時間軸、出發前待辦(可打勾)、住宿。

- 純靜態,沒有build、沒有外部程式庫;只有字型 Huninn 會從 Google Fonts 載入
- 手機優先,繁體中文,只有淺色版面
- 支援系統的「減少動態效果」設定
- 待辦的勾選與最後看的日期,只存在每個人自己的瀏覽器(localStorage)

## 放到 GitHub Pages

1. 在 GitHub 建立新的 repo(例如 `kumamoto-fukuoka-trip`)
2. 把這個資料夾裡的檔案全部上傳到 repo 的根目錄(`index.html` 要在最外層)
3. 到 repo 的 **Settings → Pages**
4. **Build and deployment** 選 `Deploy from a branch`,Branch 選 `main`、資料夾選 `/ (root)`,按 Save
5. 等 1~2 分鐘,網址會是 `https://你的帳號.github.io/kumamoto-fukuoka-trip/`

## 注意

- GitHub Pages 的網站是**公開**的,知道網址的人都看得到。這個版本已經不放訂位代號和金額
- `index.html` 內有 `noindex`,請搜尋引擎不要收錄,但不等於不能被看到
- 要改行程:直接編輯 `index.html` 裡 `<script>` 開頭的 `DAYS`(每日行程)、`TODO`(待辦)、`STAYS`(住宿)
- 倒數用的出發時間在同一段的 `TRIP_START`

## 資料來源與限制

行程內容整理自 2026/11/11 的行程表。營業時間、路況、飯店設施(例如 KAMENOYU 的貸切風呂目前休止中)可能會變,出發前請再確認。
