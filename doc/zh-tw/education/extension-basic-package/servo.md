# 伺服馬達

伺服馬達會依照指示命令動作，由程式控制馬達的旋轉角度，馬達就會轉幾度，搭配各種不同的齒輪組合，就能實際應用在玩具、模型屋、機械夾臂...等領域，實現許多有趣好玩的創意。

> - 如果要使用伺服馬達功能，需搭配 Web:Bit 擴充板，購買方式請參考：[Web:Bit 擴充板](https://store.webduino.io/products/webbit-extension-board?utm_source=webbit&utm_medium=article#_blank)
>
> - 本篇教學內容等同「[擴充套件包 - 伺服馬達](../extension-full-package/servo.html)」

## 伺服馬達 積木清單

伺服馬達積木可以設定腳位以及指定旋轉的角度 ( 0～180 度 )。

![Web:Bit 伺服馬達](../../../../media/zh-tw/education/extension-basic-package/servo-01.jpg)

> *伺服馬達積木必須搭配「開發板」積木，且不支援模擬器*，只支援 USB 與 Wi-Fi 控制。
>
> 詳情請參考 [Web:Bit 開發板](https://webbit.webduino.io/tutorials/doc/zh-tw/education/board/board.html)

## 伺服馬達 接線圖

將伺服馬達的橘色線 ( 訊號線 ) 接在 Web:Bit 擴充板的 1 號腳，紅色線接到 3.3V，棕色線接到 GND。

> 注意，因 Web:Bit 擴充板輸出電壓為 3.3V，請確認伺服馬達為支援 3.3V 的型號。

![Web:Bit 伺服馬達](../../../../media/zh-tw/education/extension-basic-package/servo-02.jpg)

## 改變旋轉角度

使用「點擊小怪獸」的積木，設定點擊綠色小怪獸時伺服馬達旋轉至 180 度，點擊紅色小怪獸時伺服馬達旋轉至 0 度，程式執行後，就可以透過滑鼠點擊小怪獸控制伺服馬達。

![Web:Bit 伺服馬達](../../../../media/zh-tw/education/extension-basic-package/servo-03.gif)




