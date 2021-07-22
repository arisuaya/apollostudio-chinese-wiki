# Apollo Studio工程的结构

{% hint style="info" %}
本章介绍了Apollo Studio的基本概念

我们建议你尽可能的理解这一章，因为对程序的基本概念有扎实的了解将助于你充分利用Apollo Studio进行灯光制作
{% endhint %}

## 项目和轨道

你在Apollo Studio中创建和处理的文件类型被称为Apollo Studio工程（.approj）。这些文件可以直接双击打开（仅在Windows上）或通过主页的“打开工程”按钮打开。工程中使用的所有外部文件都直接存储在工程文件中，所以不需要维护一个特定的文件夹。在工程文件旁边，工程备份和自动保存文件将在“（工程文件名称）Backups"文件夹中生成

![Apollo Project file](https://cdn.discordapp.com/attachments/588912865927233550/602273609196634136/unknown.png)

工程中包含承载你所有效果的“轨道”。整个工程可修改的主要参数为BPM和Macros。BPM会影响设备显示灯光的总速率。Macros（宏）保存着项目范围内用户自定义的值，可以在演奏工程时动态地改变和检查。它们最常被用来改变按键与效果的实时映射（通常称为 "Page页面"）。此外还包含使用情况（工程开启时间和工程创建日期）和工程作者的信息

![Project window](https://cdn.discordapp.com/attachments/653392306291998721/653394157364183041/unknown.png)

轨道含有Devices并管理信号的流动。它可重命名，需将一个用于按钮输入和灯光效果输出的目标Launchpad设置。当双击一个轨道时，所选轨道的窗口就会显示出来，展示它所包含的Devices。它们可以被独立地导出为Apollo轨道（.aptrk）文件

![Apollo Track file](https://cdn.discordapp.com/attachments/588912865927233550/602275354941325313/unknown.png)

在工程窗口的顶部，偏好设置按钮旁边有几个额外的按钮

* Pin按钮代表偏好设定中的 "窗口置顶Always on top"设置。你可以在多数Apollo窗口找到它
* 保存工程按钮 ”软盘形状，`CTRL+S`\(PC\)或`CMD+S`\(Mac\)” 在工程与磁盘上现有文件状态不一致时保存项目。你可以右击来进行另存为（`CTRL+SHIFT+S`\(PC\)或`CMD+SHIFT+S`\(Mac\)）或保存副本
* 撤销和重做按钮（呈弯曲的箭头形状，`CTRL+Z`\(PC\)或`CMD+Z`\(Mac\)表示撤销，`CTRL+Y`/`CTRL+SHIFT+Z`\(PC\)或`CMD+Y`/`CMD+SHIFT+Z`\(Mac\)表示重做）将分别撤销或重做你对项目做的操作。你可以右键点击其中任何一个来访问撤消历史窗口，它可以让你看到你对项目所做的所有修改，允许你跳回到任何时间点。
* 清除按钮（画笔形状，`CTRL+F`\(PC\)或`CMD+F`\(Mac\)）清除所有启动板并停止所有处理。在触发这个的时候按住\`SHIFT'会强制清除所有的启动板，而不是在一些光被卡住的情况下。

在关闭窗口时按住`CTRL`\(PC\)或`CMD`\(Mac\)，或使用快捷键`CTRL+SHIFT+W`\(PC\)或`CMD+SHIFT+W`\(Mac\)，可以完全关闭项目本身而不考虑其他打开的窗口。

## Launchpad

Apollo Studio将实际的MIDI输入和输出端口抽象为一个概念，简单地称为启动板。支持的Launchpad型号是MK2、库存的Pro和运行最近固件构建的自定义Pro单元；X和Mini MK3。

![Track Launchpads](https://cdn.discordapp.com/attachments/653392306291998721/653394646353051658/aaaaaaaaaa.png)

当Launchpad被连接时，Launchpad的类型会被立即识别，这使得光效输出可以无缝地适应不同的型号。只有真正的Launchpad的MIDI端口才会被显示为可用的Launchpad。此外，还可以在首选项窗口中覆盖输入格式（Drum Rack或XY Layout），以及Launchpad的物理旋转。

![Launchpad Configuration](https://cdn.discordapp.com/attachments/653392306291998721/653395248663232526/unknown.png)

可以通过按[Preferences](1.-First-Steps#setting-up-preferences)窗口的Launchpad Configuration部分的+按钮来添加虚拟启动板。这些显示为一个单独的窗口，可以通过点击按钮来输入，并且可以通过接收轨道输出来渲染灯光效果。同样的弹出窗口也可以通过点击物理启动板名称旁边的灰色弹出按钮来访问。在左上角，你可以使用刷子图标来清除所有的启动板并停止处理灯光效果，与项目窗口类似。一个虚拟启动板可以在首选项中被锁定，这意味着它将在下次启动时被重新创建，并且在其窗口关闭时不会断开连接。

![Launchpad pop-out window](https://cdn.discordapp.com/attachments/349854261787754498/640970278700187668/unknown.png)

## 链和设备

设备是在链内发现的，用于处理信号。有许多不同种类的设备，但它们都从左边接收信号，以自己的方式进行处理，然后将其发送到右边。与音轨类似，这些设备也可以独立导出为Apollo Chain（.apchn）和Apollo Device（.apdev）文件。

![Apollo Chain and Device files](https://cdn.discordapp.com/attachments/588912865927233550/602277643336941578/unknown.png)

考虑从Launchpad上按下一个按钮，以信号的形式进入轨道的主链。该输入被送入轨道的设备链，从最左边的设备开始。这个设备处理（改变）信号，并将结果送入下一个设备，以此类推。每条轨道的设备数量理论上是无限的。在实践中，计算机的处理器速度对你能同时使用的设备数量有限制。当信号完全通过设备链后，它以光效的形式退出到Launchpad。

![Device in a chain](https://cdn.discordapp.com/attachments/653392306291998721/653395825367580702/unknown.png)

## 信号

设备不使用MIDI音符，而使用信号进行通信。信号存储了关于按钮位置、全RGB颜色、层、当前宏、混合模式等信息。所有这些信息根本不可能存储在一个纯粹的MIDI音符中。因为Apollo用于处理的布局是XY布局，所以Launchpad中间没有奇怪的垂直间隙，这使网格感觉很自然，容易操作。

当接收Launchpad的输入时，MIDI音符被转换为信号。然后位置被转换为XY布局坐标，信号的颜色总是白色的，亮度取决于基础MIDI音符的速度。当输出到Launchpad时，多个层的信号被渲染成一个信号，并作为RGB SysEx信息送出到Launchpad。

![Signal indicators](https://cdn.discordapp.com/attachments/653392306291998721/653396349290676224/unknown.png)

行进中的信号可以用设备之间和链上的小点指示器进行可视化。这些是以轻微的性能为代价的，虽然它们在创建项目时很有用，但为了最终的性能，它们应该在\[Preferences\]（1.-First-Steps\#setting-up-preferences）的外观部分被禁用。

