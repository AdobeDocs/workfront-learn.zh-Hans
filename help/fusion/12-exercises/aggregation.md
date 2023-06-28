---
title: 聚合
description: 了解如何将多包信息聚合到一个值中。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 聚合

了解如何将多包信息聚合到一个值中。

## 练习概述

使用您在上一个练习中构建的“迭代简介”方案，聚合项目中每个工作任务的已计划小时数，并向您自己发送一封包含该信息的电子邮件。

![聚合图像1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 要遵循的步骤

**添加过滤器并对计划的小时数求和。**

1. 克隆您在上一个练习中创建的“迭代简介”方案，并将其命名为“聚合简介”。
1. 在“读取项目”的“任务”模块与“计算任务数”模块之间添加过滤器。 将过滤器命名为“仅工作任务”。
1. 将条件设置为“子项数” [数字运算符：等于] 0.

   ![聚合图像2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. 在“随机数学”模块之后，添加数值聚合器工具模块。
1. 将源模块设置为读取项目的任务。
1. 将Aggregate函数设置为SUM。
1. 从读取项目的“任务”模块中，将“值”设置为“工作”字段。
1. 将此模块重命名为“所有任务计划小时数的总和”。

   ![聚合图像3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **请注意显示聚合结束迭代的阴影。**

   ![聚合图像4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **发送包含汇总小时数的电子邮件。**

1. 在数字聚合器后添加从电子邮件应用程序发送电子邮件模块。
1. 向自己发送电子邮件。
1. 主题行是“项目详细信息”。
1. 在“内容”字段中，输入“有一个名为 [项目名称] 具有总数量的 [结果] 计划小时数。” “[项目名称]“ ”取自“读取记录”模块和“[结果]“”取自聚合器模块。

   ![聚合图像5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 保存并运行一次。 在收件箱中查找电子邮件。

在迭代中，可以访问各个包。 但在迭代之外，在发送电子邮件模块中，只能访问聚合字段。
