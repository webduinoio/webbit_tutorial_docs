# 土壤湿度侦测

土壤湿度计主要可以侦测土壤湿度，以可简易监控水位高低，原理其实是侦测两块金属片的导电度换算成湿度，当湿度越高导电度也越高，常用在智慧植栽或智慧农业的领域。

> 如果要使用土壤湿度侦测，需搭配 Web:Bit 扩充板，购买方式请参考：[Web:Bit 扩充板](https://store.webduino.io/products/webbit-extension-board?utm_source=webbit&utm_medium=article#_blank)

## 土壤湿度侦测 积木清单

土壤湿度侦测的积木可以指定脚位，读取侦测到的湿度数值 ( 0～100，0 最乾，100 最湿 )。

![土壤湿度侦测](../../../../media/zh-cn/education/extension-full-package/soil-01.jpg)


## 土壤湿度侦测 接线图

将扩充套件包里的土壤湿度计的 S 连接 Web:Bit 开发板 1 号脚，+ 连接 3.3V，- 连接 GND。

![土壤湿度侦测](../../../../media/zh-cn/education/extension-full-package/soil-02.jpg)


## 小怪兽显示土壤湿度

将「小怪兽说话」的积木放入「重复无限次」的积木里，再将「土壤湿度侦测，脚位 X 侦测到的数值」连接小怪兽积木，程式执行后，用手同时按压土壤湿度计的两片金属片，或将土壤湿度计插入水中 ( 或土壤中 )，就会看见小怪兽讲出对应的数值，环境越潮湿数字越大 ( 最大 100 )，反之数字越小 ( 最小 0 )。

![土壤湿度侦测](../../../../media/zh-cn/education/extension-full-package/soil-03.jpg)


## 透过矩阵 LED 显示湿度

延伸上方的程式，加入逻辑判断，判断「0～20」、「20～40」、「40～60」、「60～80」和「80 以上」五个区间，每个区间分别显示不同的矩阵 LED 灯号，程式执行后，用手同时按压土壤湿度计的两片金属片，或将土壤湿度计插入水中 ( 或土壤中 )，就会看见 Web:Bit 的灯号随之变化。

> 范例： [透过矩阵 LED 显示湿度](https://webbit.webduino.io/blockly/?demo=default#byr1mQvrO6O3m#_blank)

![土壤湿度侦测](../../../../media/zh-cn/education/extension-full-package/soil-04.jpg)


