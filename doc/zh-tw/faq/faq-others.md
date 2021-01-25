# 其它問題

### 1. 我想要做出XXX應用，但是學習手冊內沒有說明，該怎麼找到案例？{{others1}}

學習手冊中沒有收錄的以及非使用相關的問題，請洽 [技術社團](https://www.facebook.com/groups/webduino/#_blank)。

### 2. 如何購買 Web:Bit？{{others2}}

我們擁有自己的購物網站，可以直接在 [Web:Bit 商品資訊](https://store.webduino.io/products/webduino-bit) 找到 Web:Bit 及相關產品。

### 3. 為什麼停止執行程式後，LED 燈不會熄滅？{{others3}}

" 程式停止 " 是停止執行動作，不會重置開發板，所以開發板會維持在最後一個指令。
若要將燈熄滅，可再設計拉取一個滅燈指令或直接將開發板斷電。

### 4. 我該如何找到 MoonCar 的教學手冊？{{others4}}

MoonCar 教學手冊分類在 Web:Bit 教學手冊的目錄中。
歡迎參考 [MoonCar 教學手冊](https://webbit.webduino.io/tutorials/doc/zh-tw/education/extension-mooncar/mooncar.html#_blank)。

### 5. MoonCar 辨識顏色時間為什麼是設定 0.3 秒？{{others5}}

設定 0.3 秒是因為程式需要執行時間，為避免時間過短影響程式讀取，您可以在設計程式時更改時間大於 0.3 秒，但請避免小於 0.3 秒。

### 6. 光敏電阻偵測速度設定 100ms 是什麼意思？{{others6}}

光敏電阻偵測速度設定 100ms ( 0.1 秒 )，代表每一秒會取樣 10 次。