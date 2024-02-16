---
title: 迭代器简介练习
description: 学习使用迭代型应用程序，并对每个信息捆绑包执行操作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,noCatalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '388'
ht-degree: 100%

---

# 迭代器简介练习

学习使用迭代型应用程序，并对每个信息捆绑包执行操作。

## 练习概述

查看 Workfront 中的特定项目，然后查看该项目中的所有任务。您将会使用增量工具模块来计算项目中的任务数量。最后，您将会使用“设置变量”模块从“未决问题数量”中减去“子任务数量”，从而为每个任务捆绑包生成一个数值。

![迭代器简介图像 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 应遵循的步骤

**阅读项目和相关任务。**

1. 启动新场景。将其命名为“迭代简介”。
1. 选择 Workfront 作为触发器模块，读取一条记录。
1. 对于记录类型，选择“项目”。
1. 对于输出，选择 ID、名称和描述。
1. 在 ID 字段中，输入 Workfront 测试版实例中 Northstar Fashion Exhibitors Booth 项目的项目 ID。
1. 将此模块重命名为“查找 WF 项目”。
1. 添加另一个 Workfront 模块，以读取与该项目相关的任务。选择“读取相关记录”模块。
1. 对于记录类型，选择“项目”。
1. 对于父记录 ID，从读取记录模块中选择 ID。
1. 对于集合，选择任务。
1. 对于输出，选择 ID、名称、描述、子任务数量、未决问题数量和工作。
1. 将此模块重命名为“阅读项目的任务”。
1. 保存该场景，然后单击“运行一次”，以查看输出。

   + 单击执行检查器，您会看到 1 个捆绑包作为输入（项目），28 个捆绑包作为输出（任务）。

   **计算并处理迭代捆绑包。**

1. 在读取相关记录之后添加另一个模块。选择增量函数工具模块。

   + 将重置值字段保留为“从不”，然后单击“确定”。

1. 将此模块重命名为“计算任务数量”。
1. 添加“设置变量”模块。将变量名称设置为“随机数学”。
1. 在变量值字段中，从未决 opTask 数量中减去未决子任务数量。

   **它应该如下所示：**

   ![迭代器简介图像 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 将此模块重命名为“随机数学”。
1. 保存该场景并单击“运行一次”。

对于“读取相关记录”迭代器模块生成的每个任务，Workfront Fusion 执行了 28 次。这 28 个捆绑包将在整个场景中继续受到处理，除非通过添加聚合器来关闭循环。
