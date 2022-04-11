# 影像分类

扩充功能中的影像分类功能可以使用程式积木，配合训练好的影像辨识模型来辨识侦测到的物体。
本文会先列出「影像分类」积木的各种功能，再介绍影像分类的程式操作步骤，因为会需要使用到 [影像训练](https://md.kingkit.codes/s/g0MObOuu7) 的分类模型，所以在执行「影像分类」积木前，您需要先至影像训练平台建立分类和模型。

## 镜头来源

「镜头来源」积木可以选择使用镜头讯号的来源，分为：
- 视讯镜头：使用电脑内建视讯镜头。
- 镜头网址：使用 [WebEye](https://store.webduino.io/products?query=webeye) 等装置时，能够取得网页中的影像。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-01.png)

## 模型分类

「模型分类」积木表示辨识到的影像是某模型中的某分类。透过下拉选单，可以将影像训练建立的模型和分类名称设定到积木中，让程式判断辨识结果是否为真，再搭配其它积木执行后续动作。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-02.png)

积木下拉选单中的模型分类会对应到您在 [影像训练](https://md.kingkit.codes/s/g0MObOuu7) 中建立的模型和分类。这里的例子是使用「模型 ABC」及其分类。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-03.png)

## 信心度

「信心度」积木能够读取出影像辨识的信心度数值，单位为 ％。信心度最高为 100、最低为 0，若信心度越高，代表辨识错误的可能性越低。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-04.png)

> 因为影像训练辨识的结果会落在一个区间范围内，若信心度为 90%，代表有 90% 的机率真正的结果会落在这个区间范围内。

## 透明度

「透明度」积木可以改变影像的透明度，数值可以是 0 ~ 100，0 为完全透明、100 为原始颜色 ( 透明度不变 )。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-05.png)

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-06.png)

## 范例：影像分类

1. 首先建立影像分类模型。
2. 为了要在辨识的时候显示信心度，使用「小怪兽讲话」积木加上「信心度」积木，让其中一只小怪兽说出信心度的数值。

    ![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-07.png)

3. 再来要撰写影像分类的逻辑程式，这里的例子中会有 4 种辨识结果，包含「A」、「B」、「C」 和「都不是」。

    使用「如果执行」积木，后方加入「模型分类」积木，让影像分类成功时执行下一动作。这里的例子是让小怪兽说出辨识结果，因此在「如果」、「否则如果」后方分别设定 3 种辨识结果，并让小怪兽说出。
    
    因为辨识的物品有可能都不是分类的影像，所以在「否则」后方设定小怪兽说出「都不是」。

    ![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-08.png)

4. 完成影像分类的逻辑程式后，就能够正常进行辨识，但是这样的程式只能进行判断一次，所以需要在最外侧增加一个「重复」积木。这里选用「无限重复」积木，可以让程式不断辨识影像，并显示辨识结果。

    ![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-09.png)

5. 完成之后按下执行，可以看到随着镜头呈现的影像改变，小怪兽说出的辨识结果和信心度也会随着改变。

![Web:Bit 影像分类](../../../../media/zh-cn/education/extension/imagemlDetect-blockly-10.gif)
