---
title: 浏览运行、周期和包
description: 了解使用方案执行历史记录的运行、循环和包的行为方式。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11050
thumbnail: KT1101.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 浏览运行、周期和包

了解使用方案执行历史记录的运行、循环和包的行为方式。

## 练习概述

使用不同的方案配置实践，以探索如何使用运行和循环。

![浏览运行周期并捆绑图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 要遵循的步骤

1. 克隆名为“在路由路径之间共享变量”的方案。 将新方案命名为“在路由路径之间共享变量 — 周期测试”。
1. 删除发送电子邮件模块，因为此测试不需要此模块。

   **设置方案以每次运行处理3个周期。 在每个周期中处理5个项目。**

1. 单击触发模块，将“最大”字段更改为5，这样每个周期只处理5个项目。
1. 在“搜索”标准中，删除将搜索限制为单个项目的第二个过滤器。
1. 单击确定。

1. 在“融合”工具栏中，打开“方案”设置，并将“最大周期数”字段从1更改为3。
1. 单击确定。

   ![浏览运行周期并捆绑图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **计划方案每分钟运行一次。**

1. 单击触发器模块的时钟图标，然后将“分钟”字段更改为1分钟。

   ![浏览运行周期并捆绑图像2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 接下来，将“运行一次”按钮下的“计划”切换开关切换为“启用”。 保存方案。

   ![浏览运行周期并捆绑图像3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 转到方案的执行历史记录，然后在下一分钟内看到新的历史记录。 您可能需要刷新页面。

   ![浏览运行周期并捆绑图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 单击运行的Details按钮。 单击右侧面板中的简单日志，与在Workfront Fusion培训的执行历史记录部分中的操作类似。
1. 已处理操作的记录按周期分段。

   ![浏览运行周期和捆绑图像5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 窗口右上方的下拉菜单允许您从设置为每次运行的3个循环中选择任意一个。

   ![浏览运行周期和捆绑图像6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
