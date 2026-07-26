---
published: 2023-03-17 15:49:47
tags: [开发工具]
title: 将WIM文件添加到启动菜单的方法（适用于WinPE和RamOS）
description: 将WIM文件添加到启动菜单
image: https://chat.474029.xyz/img/ramos.png
category: 前端开发
draft: false
---
# 准备工作

所需文件：[点此下载](https://pan.474029.xyz/down.php/782239e0102c589719e4a59770e2fbc0.7z)

# 方法

下载完成后，你会得到一个压缩包，将boot.sdi文件复制到C盘根目录。

![](https://chat.474029.xyz/img/ramos/1.png)

接着将你的wim文件放到C盘根目录。

![](https://chat.474029.xyz/img/ramos/2.png)

然后在下载的压缩包中打开BOOTICEx64.exe，如果打不开就用BOOTICEx86.exe。点击“BCD编辑”

![](https://chat.474029.xyz/img/ramos/3.png)

点击“智能编辑模式”。

![](https://chat.474029.xyz/img/ramos/4.png)

如图，点击“添加”，再选择“新建WIM启动项”

![](https://chat.474029.xyz/img/ramos/5.png)

将设备文件改为刚刚wim文件的名字（前面要加“\\”），sdi文件改为“\\boot.sdi”

如果你害怕出错的话，就把wim文件名字改成“software.wim”，然后一字不落地将下图的文字写上去。

![](https://chat.474029.xyz/img/ramos/6.png)

菜单标题你可以随便起，不要改其他的选项！！

最后，重启，在显示启动菜单时你就可以选择你刚刚添加的菜单进入RamOS了。

![](https://chat.474029.xyz/img/ramos/7.png)
