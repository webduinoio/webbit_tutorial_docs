# Web:Bit 開發板

Web:Bit 提供了三種控制開發板的方式，分別是「模擬器」、「USB」和「Wi-Fi」，模擬器能夠在沒有硬體的狀況下進行學習，USB 可以在沒有網路的情況下，透過 USB 連線操控，而 Wi-Fi 則可以進行無線遠端遙控，透過三種不同操控方式的互相搭配，不論各種情境都能隨心所欲的控制。

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-01.jpg)

## 使用方式

下拉選單選擇「模擬器」，表示*使用右側的「虛擬開發板」*，開發板積木裡所有控制的元件，都會指向右側的虛擬開發板，例如繪製一個圖案，執行後，虛擬開發板就會顯示圖形。

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-02.jpg)

下拉選單選擇「USB」，表示透過「USB 線」控制「硬體開發板」，使用時請將開發板透過 USB 線連接電腦。 **網頁版或安裝版都可以使用這個功能**，例如繪製一個圖案，執行後，透過 USB 連接的開發板就會顯示圖形。

> 即日起，Web:Bit 網頁版也能透過 USB 控制開發板囉！使用前請先將開發板韌體更新到 1.1.0_0613_01 以上，接著將開發板透過 USB 線連接電腦，按下「執行」就可以開始控制。開發板韌體更新方式請參考[硬體開發板 ( 更新韌體 )](https://webbit.webduino.io/tutorials/doc/zh-tw/education/info/ota.html)。
>
> 使用網頁版 USB 功能，**不需要**同時開啟安裝版。

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-03.jpg)

下拉選單選擇「Wi-Fi」，表示*使用「Wi-Fi」連接「硬體開發板」*，也就是透過**每塊開發板的 Device ID 進行控制**，只要知道 Device ID，不論開發板身在何處，都能遠距操控。( 使用行動電源供電，會更有「遠距操控」或「無線操控」的感受 )

> 開發板 Device ID 請參考：[Web:Bit 硬體開發板 ( 初始化設定 )](../info/setup.html)

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-04.jpg)


## 控制多塊開發板

Web:Bit 編輯器可*同時控制多塊開發板*，只需要在編輯畫面裡放入開發板，指定開發板的操控方式，執行後就會看到所有開發板同時發生變化，下圖的例子，在同一個編輯畫面裡，讓一塊模擬器開發板和兩塊 Wi-Fi 開發板，同時呈現花朵圖案。

> 多塊開發板*最多包含一塊「模擬器」開發板和一塊「USB」開發板，「Wi-Fi」開發板則沒有數量限制*。

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-05.jpg)


在控制多塊開發板的情況下，**不支援使用函式控制**，要特別注意！

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-06.jpg)

![Web:Bit 開發板](../../../../media/zh-tw/education/board/board-07.jpg)



