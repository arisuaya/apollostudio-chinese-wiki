# 1.初次上手

我们建议你阅读 项目结构页 ，它概括了Apollo Studio的所有内容和功能。其余的页面可作为该页介绍的材料的深入参考。

## 必要的设置

![Firmware warning](https://cdn.discordapp.com/attachments/653392306291998721/679321874227920907/unknown.png)

为了确保你的灯尽可能顺利地运行，确保你的Launchpad固件是最新的。

![Driver warning](https://cdn.discordapp.com/attachments/339228623271886848/706681073953931324/unknown.png)

如果你运行的是Windows，Apollo Studio需要安装Novation USB Driver 2.17.10或更新版本。这样做的原因是为了使你的Launchpad能够同时与多个应用程序一起使用，在开发Launchpad封面时你几乎总是想这样做（通常与Ableton Live一起）。

## Splash Screen

当Apollo打开时，你看到的第一件事是Splash屏幕，它由一些标签组成。在这个屏幕上，你可以启动你的项目，与Apollo社区互动或了解开发者的新更新。

![File Tab](https://cdn.discordapp.com/attachments/349854261787754498/640965774105772034/unknown.png)

在文件选项卡上，你会发现一个最近打开的项目列表，以及两个按钮用于启动一个新的项目或从磁盘上打开一个现有的项目。你可以分别用CTRL-N（PC）或CMD-N（Mac）和CTRL-O（PC）或CMD-O（Mac）快捷键快速访问这些按钮。在Windows上，你也可以直接将文件拖到这里来快速打开。

![Learn Tab](https://cdn.discordapp.com/attachments/349854261787754498/640965848793612298/unknown.png)

在 "学习 "标签上，你会发现有几个按钮可以链接到互动的地方：学习材料、问题报告和支持页面。

* 文档将带你到这个Wiki
* 视频教程带你到YouTube播放列表，其中包括关于Apollo的视频指南。
* 报告错误会在GitHub上启动一个错误报告问题。
* 功能请求在GitHub上启动一个增强问题。
* 问问题 在GitHub上启动一个问题。
* Discord服务器将带你到我们的Discord邀请。
* 官方网站会带你到Apollo Studio的官方网站。
* 成为赞助人将带你到阿波罗工作室的Patreon页面。

![News Tab](https://cdn.discordapp.com/attachments/653392306291998721/653392405047017473/unknown.png)

在新闻标签上，你可以找到阿波罗工作室官方网站上最新的博客文章的链接，以及最新更新的补丁说明。

![Update](https://cdn.discordapp.com/attachments/653392306291998721/679297645679869952/unknown.png)

如果有新版本的Apollo Studio，你会注意到一个自动更新的标语。请留意新版本的发布!

## 设置首选项

Apollo的首选项窗口是你可以找到各种设置的地方，这些设置决定了Apollo的外观、行为和与外部世界的接口。这个窗口可以从左上角的齿轮图标进入。也可以通过CTRL-,\(PC\)或CMD-,\(Mac\)快捷键进入偏好设置。

![Preferences window](https://media.discordapp.net/attachments/636554452727496736/745998284828442756/unknown.png?width=345&height=480) ![Preferences window](https://media.discordapp.net/attachments/636554452727496736/745998329619677306/unknown.png?width=345&height=480)

Apollo的首选项分布在几个部分：

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

