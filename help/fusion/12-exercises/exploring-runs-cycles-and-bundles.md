---
title: 浏览运行、循环和捆绑包
description: 使用场景的执行历史记录了解运行、循环和捆绑包的行为。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 浏览运行、循环和捆绑包

使用场景的执行历史记录了解运行、循环和捆绑包的行为。

## 练习概述

对不同场景配置进行练习，以探索如何使用运行和周期。

![浏览运行循环和捆绑包图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 要遵循的步骤

1. 克隆名为“在路由路径之间共享变量”的方案。 将新方案命名为“在路由路径之间共享变量 — 循环测试”。
1. 删除发送电子邮件模块，因为此测试不需要该模块。

   **将方案设置为每次运行处理3个周期。 每个周期处理5个项目。**

1. 单击触发器模块并将Maximal字段更改为5，因此每个周期仅处理5个项目。
1. 在搜索条件中，删除将搜索限制为单个项目的第二个过滤器。
1. 单击“确定”。

1. 在Fusion工具栏中，打开场景设置，并将最大循环数字段从1更改为3。
1. 单击“确定”。

   ![浏览运行循环和捆绑包图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **计划每分钟运行的场景。**

1. 单击触发器模块的时钟图标，并将“分钟”字段更改为1分钟。

   ![浏览运行循环和捆绑包图像2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 接下来，将“运行一次”按钮下的“计划”切换开关切换为“开启”。 保存您的方案。

   ![浏览运行循环和捆绑包图像3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 转到场景的执行历史记录，并观看下一分钟内出现的新历史记录。 您可能需要刷新页面。

   ![浏览运行循环和捆绑包图像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 单击运行的详细信息按钮。 在右侧面板中单击简单日志，类似于在Workfront Fusion培训的执行历史记录部分中所执行的操作。
1. 已处理操作的记录被切割成循环。

   ![浏览运行循环和捆绑包图像5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 窗口右上方的下拉菜单允许您选择设置为每次运行的3个周期中的任意一个。

   ![浏览运行循环和捆绑包图像6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
