---
title: 数据存储演练
description: 了解如何使用数据存储在公司列表和Workfront之间同步公司名称，使用 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 96f963bf5a44eac234cbf9215f19f6dddbe23143
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 数据存储演练

## 概述

在本练习中，我们将使用数据存储来同步公司列表与Workfront之间的公司名称。

这是Workfront和其他一些系统公司单向同步的一部分。 目前，它将仅在CSV文件与Workfront之间同步。 但是，它还将在数据存储中维护一个表，该表将跟踪每个公司的Workfront ID(WFID)和CSV文件(CID)中的公司ID。 这将允许我们在未来的某个时刻实现双向同步。

![融合场景的图像](assets/data-structures-and-data-stores-2.png)

## 数据存储演练

Workfront建议先观看练习视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>有关完成演练的分步说明，请转到 [数据存储演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 练习。


## 最终说明

现在，您已经完成了有关数据结构和数据存储的学习，您可能会问自己，“您应何时使用它们？”

数据结构最常用于序列化或解析数据格式，如JSON、XML、CSV等。 数据结构使您能够控制数据结构，甚至验证数据。 您使用数据结构的最常见原因是，创建有效数据以发送到需要JSON或XML的API。 在这些情况下，您将需要使用JSON或XML应用程序以及数据结构，以确保数据格式正确。

数据存储仅应用于存储需要由多个方案执行访问的永久数据。 例如，您可以存储有关为高级用例处理的最后一条记录的元数据，这些用例要求对处理过程进行精确控制。

数据存储不设计为用作data warehouse或日志记录。 数据存储在Workfront Fusion之外不可访问，与数据存储的大多数交互都是通过Workfront Fusion方案进行的。 因此，无法将数据存储连接到data warehouse和日志记录用例预期使用的分析或报告工具。 Workfront Fusion在此类用例中的作用是填充适合组织和存储数据的系统（例如SQL、MariaDB）。

## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
