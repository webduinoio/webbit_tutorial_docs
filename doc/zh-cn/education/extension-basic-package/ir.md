# 红外线发射＆接收

红外线发射与接收，常见于我们日常生活的电器用品，只要是透过「红外线遥控器」操控的电器( 电视机、冷气机、玩具...等)，都是利用红外线发射与接收的原理，这篇教学将会介绍如何透过Web:Bit 侦测遥控器讯号以及发送红外线讯号。

> 如果要使用红外线发射＆接收功能，需搭配Web:Bit 扩充板，购买方式请参考：[Web:Bit 扩充板](https://store.webduino.io/products/webbit-extension-board?utm_source =webbit&utm_medium=article#_blank)

## 红外线发射＆接收 积木清单

红外线发射＆接收积木分为接收和发射，接收的积木又分成「接收到讯号...执行」和「接收到的代码」两种。

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-01.jpg)

> *红外线发射＆接收积木必须搭配「开发板」积木，且不支援模拟器*，只支援 USB 与 Wi-Fi 控制。
> - USB 控制模式为「安装版编辑器」限定，请参考 [Web:Bit 编辑器](../index.html#software)
> - Wi-Fi 模式需要开发板连接 Wi-Fi，请参考 [Web:Bit 硬体开发板 ( 初始化设定 )](../info/setup.html)

## 红外线发射 接线图

将红外线发射的长脚接在 Web:Bit 扩充板的 *2 号脚位*，短脚接在 GND 的位置。 ( 因为硬体设计限制，红外线发射仅能使用 2 号脚 )

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-02.jpg)

## 发射红外线讯号

红外线发射的积木可以发送十六进位的红外线代码，只要将已知的代码填入发射的栏位，执行后就会发送对应代码。

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-04.jpg)

如果搭配小怪兽的点击行为，就能够让点击绿色怪兽和点击红色怪兽时，分别发送不同的红外线讯号。

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-05.jpg)

## 红外线接收 接线图

将红外线接收的讯号脚 S 接在 Web:Bit 扩充板的 *1 号脚位*，- 号脚接在 GND，中间的脚位接在 3.3V 的位置。 ( 因为硬体设计限制，红外线接收仅能使用 1 号脚 )

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-03.jpg)

## 接收红外线讯号

红外线接收的积木有两个，执行后就会不断即时接收红外线讯号，只要收到讯号，就可以透过「接收到的代码」显示，下图的程式积木组合，执行后会透过绿色小怪兽显示遥控器发射的代码。

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-07.jpg)

如果搭配[逻辑判断](/zh-tw/docs/webbit/basic/logic.html)，就能够透过红外线遥控器遥控LED 点矩阵的图案显示，下图的程式积木组合，在收到A12345678 讯号时显示红色笑脸，收到B87654321 讯号时显示绿色方块。

![Web:Bit 红外线发射＆接收](../../../../media/zh-cn/education/extension-basic-package/ir-08.jpg)