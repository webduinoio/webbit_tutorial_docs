# Web:Bit 硬体开发板 ( 初始化设定 )

使用 Web:Bit 之前，最重要的就是进行初始化设定，初始化设定的目的在于让 Web:Bit 开发板可以自动上网 ( Internet )，有了初始化设定，我们也能够自订开发板的显示名称和密码，更可以连上 internet 进行远端更新。

>- 需要透过「Wi-Fi」连线控制开发板，才需要先进行初始化设定，如果单纯使用「USB 操控」，则可以不进行初始化设定。
>
>- 在进行初始化过程中，如果遇到无法连上网路的问题，请参考 [常见问题：无法连线到 Wi-Fi 怎么办？ ](../../faq/wifi.html#connect1#_blank)

## 初始化方法 1：使用安装版进行初始化{{step1}}

如果是使用安装版 ( 不清楚什么是安装版，请参考 [Web:Bit 编辑器](../index.html#software) )，可以直接透过安装版的工具，按照下列步骤进行初始化设定。

> 安装版下载：[WebBitSetup.exe](https://ota.webduino.io/WebBitInstaller/WebBitSetup.exe#_blank)

<iframe width="560" height="315" src="https://www.youtube.com/embed/MfYnym2oWsI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### 步骤 1、开启工具列

打开安装版后，最上方会出现安装版的「版本号码」以及「扫描 USB 装置」的提示讯息，此时可以将 Web:Bit 硬体开发板使用 USB 线连接电脑，让软体进行扫描。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-01.jpg)

扫描到开发板后，上方会出现 Web:Bit 开发板的 *Device ID、版本号码以及连线成功的文字提示*。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-02-1.jpg)

**如果一直出现「扫描 USB 装置」，没有出现连线成功的讯息**，表示 Web:Bit 开发板的韧体可能有问题 ( 程式错误或自行写入其他韧体 )，此时可以用滑鼠选择「*工具 > 回复原厂韧体*」进行韧体更新。 ( 已经出现连线成功文字讯息可忽略此步骤，*强制更新韧体可能会让 Device ID 不同*，请特别注意！ )

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-02-2.jpg)

当开发板透过 USB 连线成功后，用滑鼠选择「*工具 > 设定 Web:Bit WiFi*」，即可开始进行 WiFi 初始化更新。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-02.jpg)

### 步骤 2、设定 Wi-Fi SSID 与密码

点选设定 WiFi 后，会弹出一个对话视窗，询问欲连线的 WiFi 基地台 SSID 名称和连线密码，请填入所在场所例如：公司、学校或家里的 Wi-Fi 基地台的帐号和密码。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-03.jpg)

设定完成后，会弹出一个对话视窗，询问是否关闭 USB 连线，如果选择「确定」，开发板就会透过刚刚设定的 Wi-Fi SSID 与密码，连线到指定的 Wi-Fi 基地台，如果选择「取消」，就会关闭 Wi-Fi 连线功能，仅能使用 USB 连线操作。

若选择关闭 USB 连线功能，*Web:Bit 开发板会进入重启并闪烁红灯，当红灯熄灭且绿灯亮起一次之后，表示 Bit 开发板已经成功连结上家里或环境内的 WiFi 基地台*。 ( 若红灯持续闪烁或恒亮，请重新进行步骤 2，若红灯闪完后亮起「蓝灯」而不是绿灯，表示已有新版本可以进行下载更新，请参考 [硬体开发板 ( 更新韧体 )](ota.html) 一文。 )

> *在 Wi-Fi 连线操控的状态下，可以使用远端操控* ( 例如将开发板接行动电源远离电脑、在公司或学校控制家里的开发板 )，*透过 USB 操控必须将开发板连接控制的电脑*，虽然说无法远距操控，但可以在没有 Wi-Fi 的情形下进行操作体验。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-04.jpg)

## 初始化方法 2：连线到开发板进行初始化{{step2}}

如果无法使用安装版初始化，也可以透过有 Wi-Fi 连线功能的电脑或行动装置，连接到开发板进行初始化设定，相关步骤如下所示：

<iframe width="560" height="315" src="https://www.youtube.com/embed/EF49lfAxRsU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### 步骤 1、接上电源，输入 WiFi 帐号密码连线

把 Web:Bit 接上电源，一开始在开发板正面的全彩 LED 点矩阵，会透过跑马灯显示一串文字 ( *预设是 bit 三个英文字加上四个数字* )，这串文字对应到电脑或行动装置 WiFi 搜寻里的 SSID 名称，例如显示 bit1234，在 WiFi 搜寻中就会看到 bit1234 的名称，**注意，这串文字「不是」操控开发板的 Device ID，是识别用的 SSID**！

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-05.gif)

由于开发板尚未初始化设定完成，也就无法连线至区域网路，所以一开始*会闪红灯，或者红灯恒亮*。这时请准备一台具备 WiFi 功能的电脑、笔电或行动装置，使用这台装置进行 Wi-Fi 搜寻刚刚看到为「bitXXXX」的装置 ( 以上述的例子就是搜寻 bit1234 )，找到该装置后，输入预设密码 *12345678*，进行连线。

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-06.jpg)


### 步骤 2、设定 WiFi 帐号密码与显示名称

*确认连线成功*后，打开浏览器 ( 建议使用 Chrome )，网址列输入 192.168.4.1 连线到 Bit 开发板的设定画面，画面中包含以下几种设定：

|分类|设定|说明|
|--|--|--|
|Wi-Fi|**WiFi SSID、PWD**|必须至少填入一组 Wi-Fi 基地台 SSID 和密码，表示开发板要连接哪个 Wi-Fi 基地台，最多可填入三组，依据不同的环境自动切换。 |
|Device|**Device ID**|每块开发板的唯一识别代码，目前版本预设都是短 ID，如果看到 ID 为 18 码的长 ID，可以点击 Shorten the ID 的按钮更换为短 ID，或进行远端更新自动更换为「短 ID」( *注意！远端更新需要设定 Web:Bit 的网路连线，在网路连线状态下才能更换*，参考 [Web:Bit 硬体 ( 更新韧体 )](ota.html) )|
|Device|**Device SSID、PWD**|装置*在 WiFi 搜寻中所显示的名称和密码*，若不填写会自动产生 SSID 以及预设密码 12345678。 |
|Device|**MQTT Server**|开发板要连接的伺服器，预设 Global，中国地区请选择 China。 |
|Device|**Enable WiFi AP**|是否永远在 Wi-Fi 搜寻清单中可以看见开发板，预设持续显示，可选择三分钟后在搜寻清单里隐藏。 |
|Info|-|开发板相关资讯，包含网路卡卡号、Wi-Fi 连线以及版本资讯。 |

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-07.jpg)

设定完成后按下 SUBMIT 储存，出现 SAVE OK 的字样表示储存成功，此时 Web:Bit 开发板会重启并闪烁红灯，当红灯熄灭且绿灯亮起一次之后，表示 Bit 开发板已经成功连结上家里或环境内的 WiFi 基地台。 ( 若红灯持续闪烁或恒亮，请移除电源，重新操作步骤 1 与步骤 2，若红灯闪完后亮起「蓝灯」而不是绿灯，表示已有新版本可以进行下载更新，请参考 [Web:Bit 更新韧体](ota.html) 一文。 )

![Web:Bit 硬体 ( 初始化设定 )](../../../../media/zh-cn/education/info/setup-08.jpg)