---
title: 迭代器练习简介
description: 了解如何使用迭代类型应用程序并对每个信息捆绑包执行操作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 迭代器简介

了解如何使用迭代类型应用程序并对每个信息捆绑包执行操作。

## 练习概述

查看Workfront中的特定项目，然后查看该项目中的所有任务。 您将使用增量工具模块来计算项目中的任务数。 最后，您将使用Set变量模块从未结问题数中减去子项数，以生成每个任务捆绑包的数值。

![迭代器简介（图1）](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 要遵循的步骤

**阅读项目和相关任务。**

1. 开始新方案。 将其命名为“迭代简介”。
1. 选择Workfront作为触发器模块，读取记录。
1. 对于“记录类型”，请选择“项目”。
1. 对于“输出”，请选择“ID”、“名称”和“描述”。
1. 在ID字段中，从Workfront试用版实例中放置Northstar Fashion Exhibitors Booth项目的项目ID。
1. 将此模块重命名为“查找WF项目”。
1. 添加另一个Workfront模块以读取与此项目相关的任务。 选择读取相关记录模块。
1. 对于“记录类型”，请选择“项目”。
1. 对于“父记录ID”，请从“读取记录”模块中选择该ID。
1. 对于收藏集，选择任务。
1. 对于输出，选择ID、名称、描述、子项数量、未完成的问题数量和工作。
1. 将此模块重命名为“读取项目的任务”。
1. 保存方案，然后单击运行一次以查看输出。

   + 单击执行检查器，您将看到一个捆绑作为输入（项目），28个捆绑作为输出（任务）。

   **计数和处理迭代的包。**

1. 在读取相关记录后添加另一个模块。 选择增量函数工具模块。

   + 将“Reset a value（重置值）”字段保留为“Never（从不）” ，然后单击“OK（确定）”。

1. 将此模块重命名为“计算任务数”。
1. 添加一个Set变量模块。 将变量名称设置为“随机数学”。
1. 在“变量值”字段中，从打开的opTasks数中减去打开的子项数。

   **它应如下所示：**

   ![迭代器简介（图2）](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 将此模块重命名为“随机数学”。
1. 保存方案并单击运行一次。

对于读取相关记录迭代器模块生成的每项任务，Workfront Fusion执行了28次执行。 在整个场景中，将继续处理这28个捆绑包，除非添加聚合器来结束循环。
