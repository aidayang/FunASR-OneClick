# FunASR-OneClick
FunASR实时语音识别版免安装一键启动整合包，识别麦克风和电脑内播放的声音

## FunASR整合包说明
FunASR是阿里推出的一款语音识别转文字应用，我基于这个应用做了一个实时版的语音识别转文字软件，可以实时识别麦克风输入的声音或是电脑内播放的声音，支持实时翻译
为了方便大家快速上手体验，省去安装部署耗时，我制作了最新版免安装一键启动整合包

你也可以理解为这是一个电脑版的语音打字软件

## FunASR整合包使用教程
软件下载解压后直接双击【启动软件.exe】即可启动。软件操作界面比较简单

首先选择识别内容保存位置，识别结果输出文件格式为txt

块长度和上下文长度决定了最终的识别效果，块长度值越大，相同语速下每段识别出的内容的字数越多，上下文长度值建议是块长度值的1/2，这两个值越大，识别出的文字内容越准确，但是延迟也越高，这个可以自行测试效果，选择合适的值

音量阈值就是用于屏蔽低音噪音的，如果说话人环境比较嘈杂，可以设置该值，屏蔽掉低音噪音部分，值越大，屏蔽的声音分贝越高，也就是屏蔽的声音越多

翻译工具国内用户用百度，国外用户用谷歌，免费申请百度翻译API可以查看下面教程：https://nuowa.net/398

如果你想翻译成的目标语言在列表里没有，可自行设置语言代码，将所需要的语言代码填入目标语言输入框里即可，百度翻译和Google翻译语言代码参考下面文章：https://nuowa.net/711

待翻译文本长度的意思就是一次性提交给翻译工具的文本长度，软件并不是每次识别出内容之后都提交给翻译工具的，而是收集到一定长度的文本内容之后再发送给翻译工具进行翻译。发送给翻译工具的文本越短，翻译结果越不准确，发送的文本越长，翻译工具越能综合上下文意思翻译的更准确，但是收集的文本越长等待时间也就越长，可自行取舍。一个英文字母算一个字符，一个汉字也算一个字符，如果是类似英语语言这个值建议大一点

软件支持识别电脑内播放的声音或是麦克风等外部输入的声音。如果需要识别电脑内播放的声音，需要先进行电脑设置，鼠标右键点击电脑屏幕右下角音量喇叭图标，选择 【声音】，点击录制选项卡，鼠标右键点击【立体声混音】，选择【设置为默认设备】，如果立体声混音没启动的话，需要先启用，然后运行软件开始处理，就可以实时识别电脑播放声音了。

如果想同时接收麦克风声音和电脑内播放声音，可在软件音频源中选择电脑播放声音，电脑声音设置里-录制-麦克风，点击鼠标右键，选择麦克风属性，勾选【侦听此设备】

实时显示翻译结果如果勾选的话，在终端窗口里会替代输出原识别内容，改为显示实时语音翻译结果

软件使用视频教程：[youtube>>](https://www.youtube.com/watch?v=8aCEKFi8rh8)

## 注意事项
本软件只支持识别中英文，不支持识别其它语言

软件运行路径中不要出现中文及空格，否则会报错

软件只支持win10或win11，不支持其他版本Windows系统，也不支持手机和MAC

有部分Win11用户发现软件无法检测到音频，也就是电脑立体声混音没有音频输入，可以安装voicemeeter虚拟声卡解决。在【1 HARDWARE INPUT】设置硬件声音输入设备，在【VIRTUAL INPUT】选中【B】，在【HARDWARE OUT】选择声音输出设备，然后打开电脑系统-声音-录制，将默认设备选择为VoiceMeeter VAIO3 Output

## FunASR电脑实时语音识别转文字整合包下载链接

https://pan.quark.cn/s/4ae36edd5858

https://pan.baidu.com/s/1NZzKc7H9541F5VqILdNeog?pwd=ynur

## FunASR项目地址

https://github.com/modelscope/FunASR
