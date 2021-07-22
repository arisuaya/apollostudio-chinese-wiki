# 初次设定与总概括

{% hint style="info" %}
我们建议你阅读 项目结构页 ，它概括了Apollo Studio的所有内容和功能。其余的页面可作为该页介绍的材料的深入参考。
{% endhint %}

为了确保你的灯尽可能顺利地运行，请确保你的Launchpad固件是最新的，当Apollo检测到固件版本低于推荐固件时，将会弹出窗口，你可以使用Novation Component或Launchpad Utility来更新

![](../.gitbook/assets/driver-warning.png)

如果你运行的是Windows系统，Apollo Studio需要安装Novation USB Driver 2.17.10或更新的版本才能运行（推荐使用USB Driver 2.22，不会蓝屏）。驱动是为了使你的Launchpad能够同时与多个进行MIDI交互的应用程序兼容（配合Ableton Live）。

当Apollo检测到未安装驱动时将会弹窗

![&#x9A71;&#x52A8;&#x8B66;&#x544A;](https://img.kaiheila.cn/assets/2021-06/R5ZX1JmCVP0e604r.png)

## 主页

当Apollo启动时，你看到的第一界面便是主页，它由一些标签页组成。在这个页面上，你可以启动你的Apollo工程，与Apollo社区互动或了解开发者的新更新。

在文件选项卡上，你可以看到“最近打开的项目”列表，以及两个按钮用于“创建一个新的项目（New Project）”或“从磁盘上打开一个现有的项目（Open Project）”。你可以用CTRL+N（PC）或CMD+N（Mac）和CTRL+O（PC）或CMD+O（Mac）快捷键快速使用这些按钮。

在Windows上，你也可以直接将文件拖到窗口上来打开。

![&#x6587;&#x4EF6;](https://img.kaiheila.cn/assets/2021-06/K75TroGfM80hs08w.png)

在 "学习 "标签页上，你会发现有几个按钮可以进行链接的跳转：

* 说明文档Documentation会跳转至Apollo的Github Wiki
* 视频教程Video Tutorials会跳转至YouTube Apollo视频教学的播放列表
* 报告问题Report a Bug会跳转至GitHub上并开启一个Bug提交的Issue。
* 功能请求Feature Request会跳转至GitHub上并开启一个功能新增请求的Issue。
* 问问题Ask a Question会跳转至GitHub上并开启一个提问的Issue。
* Discord服务器会跳转至Apollo Studio的官方Discord群组。
* 官方网站Official Website会跳转至Apollo Studio的官方网站。
* 成为赞助人Become a Patron会跳转至Apollo Studio的Patreon页面。

![&#x5B66;&#x4E60;](https://img.kaiheila.cn/assets/2021-06/8bvOVJILPp0hs08w.png)

在新闻标签上，你可以找到Apollo Studio官方网站上最新的博客文章的链接，以及新版本更新的修改说明。

![&#x65B0;&#x95FB;](https://img.kaiheila.cn/assets/2021-06/skHCE5qT6k0hs08w.png)

如果有新版本的Apollo Studio，你会注意到一个自动更新的标语。请留意新版本!

![Update](https://img.kaiheila.cn/assets/2021-06/KzuvHSih360hs09q.png)

## 偏好设置

Apollo的偏好设置窗口是你可以找到各种设置的地方，这些设置决定了Apollo的外观、行为和与外接设备的设定。这个窗口可以从左上角的齿轮图标进入。也可以通过CTRL+,\(PC\)或CMD+,\(Mac\)快捷键进入偏好设置。

![Preferences window](https://img.kaiheila.cn/assets/2021-06/81saLIQqMl0cs0hs.png) ![Preferences window](https://img.kaiheila.cn/assets/2021-06/bpf6BaqIE90cs0hs.png)

Apollo偏好设置有几个部分：

* 外观部分改变用户界面的布局或风格。
* 主题部分改变颜色方案。请注意，需要重新启动才能使改变生效。
* 处理部分限制了在任何时候在Launchpad上绘制的每秒最大帧数（FPS）。这一点很重要，因为过度刺激Launchpad会导致滞后，或者在生成效果时CPU使用率过高。
* 屏幕上的Launchpad风格设置控制Launchpad在用户界面上的显示方式。
* 启动板配置部分用来帮助Apollo识别MIDI端口作为启动板。可以为每个启动板选择一个旋转，以及输入格式。此外，还可以创建虚拟启动板。
* 组的行为部分改变了主编辑器在向组添加链时的行为。
* 模式编辑器部分改变了模式编辑器的行为，并允许清除你的颜色历史。
* 模式MIDI导入调色板部分改变了模式编辑器的导入功能如何从一些预设的方法中解释MIDI文件中的音符的速度值，以及选择一个自定义的Retina调色板文件。
* 文件管理部分是指Apollo在你工作时如何在后台处理你的文件，以及允许你清除最近的项目列表。
* 撤销历史部分允许你取消对可以撤销的操作的限制。请注意，禁用这一限制将随着时间的推移大大增加内存的使用。
* Discord Rich Presence部分控制Apollo如何与作为活动应用程序/游戏的Discord接口。
* 应用程序管理部分用于管理自动更新，以及显示存储崩溃日志的文件夹。最好保持自动更新功能，以免错过关键修复和新功能。在下载更新之前，阿波罗将始终征求您的同意。
* 使用统计部分显示关于使用情况和在Apollo中工作的时间的信息。

