---
title: 计算字段和表达式入门
description: 了解如何在计算字段中创建表达式，以收集有关贵组织正在完成工作的唯一自定义数据。
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: f81d156b4058bec70bc3256efda6f85746f0f625
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 计算字段和表达式入门

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

Workfront提供了多个业务领域中通用的各种字段，并定期用于工作管理。 诸如计划完成日期、项目预算、任务代理人名称等字段。

但是，每个组织都需要收集其特定行业和公司的数据，以便了解公司目标是否实现。 例如，您的组织希望跟踪：

* 项目将贡献哪一业务领域。
* 如果资金来自供应商、内部或两者。
* 所用图像需要什么分辨率。

尽管这些字段并非内置于 [!DNL Workfront]，您可以通过自定义表单创建自定义数据输入字段和预填充的多选答案字段。

此学习路径重点介绍计算字段。 您将了解计算字段的含义、通过数据表达式可提取到计算字段中的不同信息类型，以及如何构建这些计算字段以增强数据收集和报告功能。

![资源管理设置一个寻呼机](assets/GS01.png)

## 什么是计算字段？

计算字段会存储使用数据表达式和现有Workfront字段创建的自定义数据。

![具有利用率的工作负载平衡器报告](assets/GS02.png)

例如，您的组织有一个特定的项目编号或工作编号系统，该系统包括：

* 在项目创建的年份，
* 项目所有者的姓名缩写，以及
* 的 [!DNL Workfront] 项目参考编号。


使用计算字段中的表达式，您可以获取已存储在 [!DNL Workfront] 并创建该唯一项目ID或工作号，然后可将其添加到如下报表：

![具有利用率的工作负载平衡器报告](assets/GS03.png)

根据所需的特定数据，计算字段可能会很简单，使用一个或两个表达式，或者使用多个嵌入的表达式来处理更复杂的问题。 请记住，Workfront只能将已存储或提取到系统中的数据用于计算字段。

## 文本表达式

文本表达式搜索、剖析和组合 [!DNL Workfront] 以创建更有意义的数据，或更深入地了解贵组织正在完成的工作。

例如，文本表达式可用于：

* 在项目支出超过$5,000时显示“超过$5,000”，或在项目视图的列中显示“低于$5,000”。

* 为每个项目指定一个唯一编号，该编号包括项目创建年份、项目的  [!DNL Workfront] 引用编号、项目名称和项目所有者的缩写。

* 构建一个报告，其中列出未分配到项目组合和/或项目群的每个项目，以便您在经理会议中可以使用该报告。

在自定义字段中可以使用文本表达式在Workfront中执行这些类型的搜索和组合。

查看可能的文本表达式时，您会找到多个选项。

![资源管理设置一个寻呼机](assets/TE01.png)

最常使用以下六种文本表达式：

* CONCAT
* 左/右
* CONTAINS
* IF
* ISBLANK