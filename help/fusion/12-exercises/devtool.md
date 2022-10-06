---
title: 开发工具
description: 使用DevTool增强您对方案进行故障诊断的能力并简化复杂配置。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11057
thumbnail: KT11057.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# 开发工具

使用开发工具增强您对方案进行故障诊断的能力并简化复杂配置。

## 练习概述

安装和使用Workfront开发工具中的不同区域，以便更深入地了解所发出的请求/响应以及高级方案设计技巧。

>[!NOTE]
>
>Workfront Fusion Dev工具仅在使用 [Chrome开发人员工具](https://developer.chrome.com/docs/devtools/).

![Devtool图像1](../12-exercises/assets/devtool-walkthrough-1.png)

## 要遵循的步骤

**安装开发工具。**

1. 下载“workfront-fusion-devtool.zip”文档，该文档位于测试驱动器的Fusion Exerice Files文件夹中。
1. 将Zip文件解压到文件夹中。
1. 在Chrome中打开选项卡，然后输入 **chrome://extensions**.
1. 使用右上方的开关打开开发人员模式，然后单击左上方显示的“Load unplocked”按钮。 选择包含开发工具的文件夹（您可在此处解压缩该工具）。

   ![Devtool图像2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 解压后，开发工具即会显示在您的其他扩展中。

   ![Devtool图像3](../12-exercises/assets/devtool-walkthrough-3.png)

   **使用实时流。**

1. 首先，打开“使用数据存储同步数据”方案。
1. 键入F12或函数F12以打开开发工具。 或者，您也可以单击Chrome地址栏中的三点式菜单，然后导航到开发人员工具。

   ![Devtool图像4](../12-exercises/assets/navigate-to-devtools.png)

1. 单击Workfront Fusion选项卡，然后从左侧的列表中选择Live Stream 。
1. 单击运行一次，以查看事件发生时的事件。
1. 单击某个事件可查看右侧的“请求标头”、“请求正文”、“响应标头”和“响应正文”选项卡。

   ![Devtool图像4](../12-exercises/assets/devtool-walkthrough-4.png)

   **使用方案调试器**

1. 选择Scenario Debugger并单击某个模块可查看有关该模块操作的信息。

   ![Devtool图像5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 导航到历史记录选项卡。 单击执行的详细信息，以检查特定执行的模块操作详细信息。

   ![Devtool图像6](../12-exercises/assets/devtool-walkthrough-6.png)

   **使用工具**

1. 返回到方案设计器，然后在开发工具中选择工具。 此时会显示可用的工具。

   ![Devtool图像7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 集中模块 — 使用模块ID快速查找并打开模块。
+ 通过映射查找模块 — 使用关键字搜索方案以查找模块中映射的值和/或键。
+ 获取应用程序元数据 — 在某种情况下，查看选定应用程序的元数据。
+ 复制映射 — 将映射从一个模块复制到另一个模块。 您还可以在设计器中克隆模块。
+ 复制过滤器 — 复制过滤器。 过滤器始终会被分配给右侧的模块。
+ 交换连接 — 该工具从选定模块获取连接，并在方案中为同一应用程序的所有模块设置相同的连接。 如果您必须在整个已完成的方案中更改连接，则此操作会很有帮助。 使用此工具，避免丢失所有映射并节省时间。
+ 交换变量 — 在整个方案或一个模块中查找出现的所有给定变量，并将它们替换为新的变量。 不支持通配符。 如果您在整个方案中意外映射了一个值，这可以帮助您轻松交换正确的值。
+ 交换应用程序 — 将给定的应用程序交换为另一个应用程序。
+ Base 64 — 将输入的数据编码为Base64或对Base64进行解码。 当您想要在编码请求中搜索特定数据时，此变量非常有用。
+ 复制模块名称 — 将选定的模块名称复制到剪贴板。
+ 重新映射源 — 将映射源从一个模块更改为另一个模块。 在方案中，您需要首先将要用作源模块的模块添加到路由中。
+ 迁移操作系统 — 专门用于将Google工作表（旧版）模块升级到最新的Google工作表版本。 它会在方案路由中模块的旧版本之后添加模块的新版本。
