---
title: 迭代器练习简介
description: 了解如何使用迭代类型的应用程序并对每个信息包执行操作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: 1ab337568afd314d461ddea5952c9b4c900b9c26
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 迭代器简介

了解如何使用迭代类型的应用程序并对每个信息包执行操作。

## 练习概述

在Workfront中查看特定项目，然后查看该项目中的所有任务。 您将使用增量工具模块计算项目中的任务数。 最后，您将使用“设置”变量模块从“未解决问题数”中减去“子项数”，为每个任务包生成一个数值。

![迭代器简介图1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 要遵循的步骤

**阅读项目和相关任务。**

1. 开始新方案。 将其命名为“迭代简介”。
1. 选择Workfront作为触发模块，读取记录。
1. 对于“记录类型”，选择“项目”。
1. 对于“输出”，选择“ID”、“名称”和“描述”。
1. 在ID字段中，将Northstar Fashion Preamers Booth项目的项目ID放在您的Workfront试用实例中。
1. 将此模块重命名为“查找WF项目”。
1. 添加另一个Workfront模块，以读取与此项目相关的任务。 选择“读取相关记录”模块。
1. 对于“记录类型”，选择“项目”。
1. 对于父记录ID，从读取记录模块中选择该ID。
1. 对于收藏集，选择任务。
1. 对于“输出”，选择“ID”、“名称”、“描述”、“子项数”、“未解决问题数”和“工作”。
1. 将此模块重命名为“读取项目的任务”。
1. 保存方案，然后单击运行一次以查看输出。

   + 单击执行检查器，您会看到一个包作为输入（项目），28个包作为输出（任务）。

   **计数并处理迭代包。**

1. 在“读取相关记录”之后添加另一个模块。 选择“增量”功能工具模块。

   + 将重置值字段保留为从不，然后单击确定。

1. 将此模块重命名为“计算任务数”。
1. 添加设置变量模块。 将变量名称设置为“随机数学”。
1. 在“变量值”字段中，从打开的opTask数中减去打开的子项数。

   **它应该如下所示：**

   ![迭代器简介图2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 将此模块重命名为“随机数学”。
1. 保存方案，然后单击运行一次。

对于读取相关记录迭代器模块生成的每个任务，Workfront Fusion执行了28次。 在整个方案中，将继续处理这28个包，除非添加聚合器以关闭循环。
