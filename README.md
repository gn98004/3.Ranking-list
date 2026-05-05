# 小拾光 v1.22 Supabase Storage 圖片上傳版

## 更新重點
- 修正手機 / 新電腦登入時一直顯示「雲端尚未連線」的問題：登入視窗會自動展開 Supabase 連線設定，填完 Project URL 與 anon key 後即可登入。
- 發文封面可選擇本機圖片，上傳到 Supabase Storage 後自動回填圖片網址。
- 留言圖片 / GIF 改為發送時上傳到 Supabase Storage。
- 我的頁新增頭像上傳，圖片會上傳到 Supabase Storage。
- 保留管理員 / 一般使用者權限分流。

## 使用順序
1. 到 Supabase SQL Editor 執行 `supabase_v1_22_storage_setup.sql`。
2. 開啟 `index.html`。
3. 到「我的」→「登入 / 註冊」。
4. 如果手機顯示尚未連線，展開的「系統連線設定」貼上 Project URL 與 anon public key，按儲存。
5. 使用 Email / 密碼登入或註冊。
6. 測試發文圖片、留言圖片、頭像上傳。

## Storage bucket
預設 bucket 名稱：`xiaoshiguang-media`

建議限制：
- 發文封面：3MB 以下
- 留言圖片 / GIF：圖片 1MB 以下，GIF 2MB 以下
- 頭像：1MB 以下
