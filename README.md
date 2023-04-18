## MediaPublish

刚刚突然有点想法，想做一套多媒体发布管理系统，但只是停留在想法，也许最终也只有这篇Readme。


**具体说说**

### 背景
在过去一两年的工作中接触到一些展厅项目，一开始无论硬件配套还是软件配套都相对原始，比如播放视频可能是找个播放器PotPlayer循环播放，比如更改视频文件还得找个U盘插上一体机（安卓）或者PC电脑手动替换。

标准化建设下PC应该全部集中放在机房，显示屏则和PC相距较远，或者PC放在显示器附近柜子里，插U盘或者鼠标都极不方便，在实际操作中有出现无线鼠标+USB延长线的方式，但这些操作都是极为不方便、不人性化。

也衍生一些面上的需求，比如讲解员想在某一块展示区域切换内容，那不可能去一个个插鼠标解决，貌似有kvm那种方式解决？但也很不人性化。
后来我极力从软件角度找了一些解决方式：

 - 借助vlclib做了WPF/Winform桌面程序，实现对播放器的自主控制（UI样式、视频切换、暂停、播放、播放模式、音量等等）
 - 借助vnc实现在内网内远程桌面，未来想法是将vnc或者类似功能软件嵌入到这个平台里。
 - 借助adb、scrcpy可对安卓设备进行控制、远程桌面连接，简单看了下这些应该是可以嵌入到平台里的
 当然我也从硬件角度做了一点改变：
 - 加装PC开机卡，不用手动一个个按开机键。

其它一些不做阐述。

### 想法
<p>也不是为了解决问题，就是觉得这明明就可以做成一套系统，我觉得它可以拥有以下功能：</p>
- 较为自由的PC端多媒体播放器（支持常见视频、图片格式，有必要加上Word、PPT、PDF等)
- 较为自由的安卓端多媒体播放器（支持常见视频、图片格式，支持触控）
- 较为自由的iPad控制端，傻瓜式操作用于讲解员角色
- 较为自由的PC控制端，可以实现全局尽可能多的功能控制功能，如1.调整任一终端的文件 2.远程桌面任意终端 3.配置任意终端 4. 其它可能出现的功能

预计有PC端控制端、iPad端、Android被控端、PC被控端

### 现实
- 这套程序也许不会动工，也许是个长期项目，写个好几年
- 这套程序尽可能实现多的功能，尽可能对每个面的功能及逻辑细化；也不仅仅以上这些想法，也许会增加很多，也许会推翻再设想
- 这套程序就当是对过去一部分工作总结和扩展，当作练手，当作爱好
- 这套程序不是为工作而写，这个环境下不允许我写这套软件，实际非常有用，不做无意义的感情和精力付出
- 希望生活变得好一点点
