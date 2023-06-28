---
title: 开发工具
description: 使用DevTool增强对场景进行故障排除并简化复杂配置的能力。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 开发工具

使用开发工具增强对场景进行故障排除并简化复杂配置的能力。

## 练习概述

安装并使用Workfront开发工具中的各个区域，以更深入地了解所做的请求/响应以及高级方案设计技巧。

>[!NOTE]
>
>Workfront Fusion开发工具仅在使用的 [Chrome开发人员工具](https://developer.chrome.com/docs/devtools/).

![Devtool图像1](../12-exercises/assets/devtool-walkthrough-1.png)

## 要遵循的步骤

**安装开发工具。**

1. 下载在测试驱动器的Fusion Experience Files文件夹中找到的“workfront-fusion-devtool.zip”文档。
1. 将Zip文件解压缩到文件夹。
1. 在Chrome中打开选项卡并输入 **chrome://extensions**.
1. 使用右上角的开关打开开发人员模式，然后单击左上角的“Load unpacked”（加载解包）按钮。 选择包含开发工具的文件夹（这是您解压该工具的位置）。

   ![Devtool图像2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 解压缩后，开发工具会出现在其他扩展中。

   ![Devtool图像3](../12-exercises/assets/devtool-walkthrough-3.png)

   **使用实时流。**

1. 首先打开“使用数据存储同步数据”方案。
1. 通过键入F12或函数F12打开开发工具。 或者，您可以单击Chrome地址栏中的三个点菜单，然后导航到开发人员工具。

   ![Devtool图像4](../12-exercises/assets/navigate-to-devtools.png)

1. 单击“Workfront Fusion”选项卡，然后从左侧列表中选择“实时流”。
1. 单击一次运行可在事件发生时查看事件。
1. 单击某个事件可在右侧查看“请求标头”、“请求正文”、“响应标头”和“响应正文”选项卡。

   ![Devtool图像4](../12-exercises/assets/devtool-walkthrough-4.png)

   **使用场景调试器**

1. 选择场景调试器并单击模块可查看有关该模块操作的信息。

   ![Devtool图像5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 定位至“历史记录”标签。 单击执行上的详细信息可检查特定执行的模块操作详细信息。

   ![Devtool图像6](../12-exercises/assets/devtool-walkthrough-6.png)

   **使用工具**

1. 返回方案设计器，然后在开发工具中选择工具。 这将显示可用的工具。

   ![Devtool图像7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 焦点模块 — 使用模块ID快速查找并打开模块。
+ 通过映射查找模块 — 使用关键字搜索方案，以查找模块中的映射值和/或键。
+ 获取应用程序元数据 — 在场景中查看所选应用程序的元数据。
+ Copy Mapping — 将映射从一个模块复制到另一个模块。 您还可以在设计器中克隆模块。
+ 复制筛选器 — 复制筛选器。 筛选器始终分配给右侧的模块。
+ 交换连接 — 该工具从选定的模块获取连接，并在场景中设置与同一应用程序的所有模块的相同连接。 如果您必须在整个已完成方案中更改连接，这将很有帮助。 使用此工具可避免丢失所有映射，并节省时间。
+ 交换变量 — 查找给定变量在整个场景中或在一个模块中的所有匹配项，并将其替换为新的匹配项。 不支持通配符。 如果您意外地在整个场景中映射了一个值，这可以帮助您轻松交换正确的值。
+ 交换应用程序 — 将给定的应用程序交换为另一个应用程序。
+ Base 64 — 将输入的数据编码到Base64或解码Base64。 当您想要搜索编码请求中的特定数据时，此变量非常有用。
+ 复制模块名称 — 将选定的模块名称复制到剪贴板。
+ 重新映射源 — 将映射源从一个模块更改为另一个模块。 您需要首先添加模块，以用作场景中路由的源模块。
+ 迁移操作系统 — 专门用于将Google Sheets（旧版）模块升级到最新Google Sheets版本。 紧接在场景路由中的旧版模块之后，它会添加一个新版本的模块。
