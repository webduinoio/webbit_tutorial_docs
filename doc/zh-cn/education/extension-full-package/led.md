# LED

LED 是发光二极体 ( Light-emitting diode ) 的缩写，是一种能发光的半导体电子元件，目前能够发出可见光、红外光一直到紫外光的光线，近年来更逐渐发展至各种照明用途，本篇所使用的 LED 是专门用于小型电子设备的材料，透过 Web:Bit 发送对应的讯号即可进行控制。

> 如果要使用 LED，需搭配 Web:Bit 扩充板，购买方式请参考：[Web:Bit 扩充板](https://store.webduino.io/products/webbit-extension-board?utm_source=webbit&utm_medium=article#_blank)

## LED 积木清单

LED 积木可以设定脚位以及指定状态为 ON 或 OFF。

![LED](../../../../media/zh-cn/education/extension-full-package/led-01.jpg)

## LED 接线图

使用扩充套件包的 LED 模组，将 S 讯号脚连接 Web:Bit 扩充板的 1 号脚，VCC 连接 3V3，GND 连接 GND。

![LED](../../../../media/zh-cn/education/extension-full-package/led-02.jpg)

## LED 闪烁

将 LED 的积木放在「重复无限次」的回圈里，将第一个 LED 积木状态设定为 ON，等待一秒后放入第二个 LED 状态为 OFF 的积木，最后再放入一个等待一秒的积木，程式执行之后，就会看见 LED 开始闪烁。

![LED](../../../../media/zh-cn/education/extension-full-package/led-03.jpg)

## 点击小怪兽控制 LED

放入「当滑鼠点击怪兽」的积木，设定点击绿色怪兽就会点亮 LED ( 状态 ON )，点击红色怪兽时关闭 LED ( 状态 OFF )，点击黄色怪兽就让 LED 闪烁 ( 延续上方 LED 闪烁的积木程式 )，完成后在所有怪兽的点击积木里，需要额外放入「停止所有回圈」的积木，如此才能在 LED 亮起或熄灭时停止闪烁，也能避免闪烁回圈重复叠加的情形发生。

> 范例：[点击小怪兽控制 LED](https://webbit.webduino.io/blockly/?demo=default#8qMJ9M0Wj8D3W#_blank)

![LED](../../../../media/zh-cn/education/extension-full-package/led-04.jpg)

## 使用 Web:Bit 按钮开关控制 LED

如果要使用 Web:Bit 开发版的按钮控制 LED 灯，可以将上方小怪兽的积木，换成按钮开关的积木，按下 A 的时候会点亮 LED ( 状态 ON )，按下 B 就关闭 LED ( 状态 OFF )，A 和 B 同时按下就让 LED 闪烁 ( 延续上方 LED 闪烁的积木程式 )

> 范例：[使用 Web:Bit 按钮开关控制 LED](https://webbit.webduino.io/blockly/?demo=default#py6lPpWKDzXqZ#_blank)

![LED](../../../../media/zh-cn/education/extension-full-package/led-04.jpg)

