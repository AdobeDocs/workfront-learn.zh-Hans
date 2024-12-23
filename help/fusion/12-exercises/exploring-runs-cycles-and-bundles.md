---
title: 探索运行、周期和捆绑练习
description: 使用场景的执行历史记录了解运行、周期和捆绑的行为方式。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '342'
ht-degree: 100%

---

# 探索运行、周期和捆绑练习

使用场景的执行历史记录了解运行、周期和捆绑的行为方式。

## 练习概述

练习不同的场景配置，探索如何使用运行和循环。

![探索运行、周期和捆绑图像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 应遵循的步骤

1. 克隆名为“在路由路径之间共享变量”的场景。将新场景命名为“在路由路径之间共享变量 - 周期测试”。
1. 删除“发送电子邮件”模块，因为此测试不需要它。

   **将您的场景设置为每次运行处理 3 个周期。每个周期处理 5 个项目。**

1. 单击“触发”模块，将 Maximal 字段更改为 5，这样每个周期只会处理 5 个项目。
1. 在“搜索”条件中，删除将搜索范围限制为单个项目的第二个过滤器。
1. 单击“确定”。

1. 在 Fusion 工具栏中，打开“场景”设置并将“最大周期数”字段从 1 更改为 3。
1. 单击“确定”。

   ![探索运行、周期和捆绑图像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **将场景计划为每分钟运行一次。**

1. 单击“触发”模块旁的时钟图标，并将“分钟”字段更改为 1 分钟。

   ![探索运行、周期和捆绑图像 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 接下来，将“运行一次”按钮下的“计划”开关切换为“开”。保存您的场景。

   ![探索运行、周期和捆绑图像 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 转到该场景的执行历史记录，并观察下一分钟内出现的新历史记录。您可能需要刷新页面。

   ![探索运行、周期和捆绑图像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 单击一次运行的“详细信息”按钮。单击右侧面板中的“简单”日志，其类似于您在 Workfront Fusion 培训的执行历史记录部分中所做的操作。
1. 已处理操作的记录被划分为多个周期。

   ![探索运行、周期和捆绑图像 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 窗口右上角的下拉菜单允许您选择每次设置运行的 3 个周期中的任意一个。

   ![探索运行、周期和捆绑图像 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
