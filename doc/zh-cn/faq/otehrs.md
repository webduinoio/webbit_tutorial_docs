# 其它问题

### 1. 我想要做出XXX应用，但是学习手册内没有说明，该怎么找到案例？{{others1}}

学习手册中没有收录的以及非使用相关的问题，请洽 [技术社团](https://www.facebook.com/groups/webduino/#_blank)。

### 2. 如何购买 Web:Bit？{{others2}}

我们拥有自己的购物网站，可以直接在 [Web:Bit 商品资讯](https://store.webduino.io/products/webduino-bit#_blank) 找到 Web:Bit 及相关产品。

### 3. 为什么停止执行程式后，LED 灯不会熄灭？{{others3}}

" 程式停止 " 是停止执行动作，不会重置开发板，所以开发板会维持在最后一个指令。
若要将灯熄灭，可再设计拉取一个灭灯指令或直接将开发板断电。

### 4. 我该如何找到 MoonCar 的教学手册？{{others4}}

MoonCar 教学手册分类在 Web:Bit 教学手册的目录中。
欢迎参考 [MoonCar 教学手册](h/tutorials/doc/zh-cn/education/extension-mooncar/mooncar.html)。

### 5. MoonCar 辨识颜色时间为什么是设定 0.3 秒？{{others5}}

设定 0.3 秒是因为程式需要执行时间，为避免时间过短影响程式读取，您可以在设计程式时更改时间大于 0.3 秒，但请避免小于 0.3 秒。

### 6. 光敏电阻侦测速度设定 100ms 是什么意思？{{others6}}

光敏电阻侦测速度设定 100ms ( 0.1 秒 )，代表每一秒会取样 10 次。