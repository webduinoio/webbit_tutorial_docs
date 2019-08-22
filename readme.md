# Web:Bit 教學

這是 Web:Bit 的教學文多語系檔案，新增或編輯文件後，會由 Webduino 官方審閱，審閱後就會公開於 Web:Bit 教學網站內，歡迎有志之士一同加入教學文的撰寫與維護～

## 目錄結構

- doc：教學文 markdown
  - zh-tw：繁體中文
  - zh-cn：簡體中文
  - en：英文
- media：教學文內所需圖檔
  - zh-tw：繁體中文
  - zh-cn：簡體中文
  - en：英文

## 編輯說明

- **msg.json** 為教學網站的語系檔。
- **readme.md** 為教學網站左側的目錄，超連結使用相對路徑連結對應的 markdown。
- `h1` tag 大標題會自動變成 html head 裡的 title。
- `h1`～`h6` tag 標題後方加上`{{hash}}`會自動生成`id`。
- 第一段文字`p`會自動變成 html meta 標籤的 description。
- 超連結預設 target 為 `_self`，若要修改可在超連結後方加上`#_blank`。
- 圖片放在 media 內，資料結構請和 markdown 文件相同，例如 **doc/zh-tw/test/a.md** 的圖片就放在 **media/zh-tw/test/** 資料夾中。
- 若 markdown 編輯時使用「相對路應」進行 media 資料夾中的圖片預覽，屆時轉換為 html 也會是以「同樣的相對路徑」呈現。
- html meta 標籤的預覽縮圖為同文件 markdown 檔名的 jpg 檔案，例如 a.md 的縮圖就是 a.jpg。
