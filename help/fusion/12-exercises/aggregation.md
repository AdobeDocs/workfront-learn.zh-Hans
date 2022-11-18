---
title: 聚合
description: 了解如何将多个信息包聚合到一个值中。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 聚合

了解如何将多个信息包聚合到一个值中。

## 练习概述

使用您在上一个练习中构建的“迭代简介”方案，汇总项目中每个工作任务的计划小时数，并向您自己发送一封包含该信息的电子邮件。

![聚合映像1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 要遵循的步骤

**添加过滤器并对计划小时数进行求和。**

1. 克隆在上一个练习中创建的“迭代简介”方案，并将其命名为“聚合简介”。
1. 在读取项目的任务模块和计数任务模块之间添加过滤器。 将筛选器命名为“仅工作任务”。
1. 将条件设置为“子项数” [数值运算符：等于] 0。

   ![聚合映像2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. 在“随机数学”模块之后，添加数字聚合器工具模块。
1. 将源模块设置为“读取项目的任务”。
1. 将聚合函数设置为SUM。
1. 在读取项目的任务模块中将值设置为工作字段。
1. 将此模块重命名为“所有任务计划小时数的总和”。

   ![聚合映像3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **请注意显示聚合结束迭代的阴影。**

   ![聚合映像4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **发送包含累计小时数的电子邮件。**

1. 在数字聚合器之后，从电子邮件应用程序添加发送电子邮件模块。
1. 将电子邮件发送给您自己。
1. 主题行是“项目详细信息”。
1. 在“内容”字段中，放置“存在一个名为 [项目名称] 具有 [结果] 计划时间。” “[项目名称]“ ”是从“读取记录”模块中获取的，并且“[结果]“ ”是从聚合模块中获取的。

   ![聚合图像5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 保存并运行一次。 在您的收件箱中查找电子邮件。

在小版本中，可以访问各个包。 但在小版本之外，在发送电子邮件模块中，只能访问聚合字段。
