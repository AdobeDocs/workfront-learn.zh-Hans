---
title: 数据存储演练
description: 了解如何使用数据存储来同步公司列表与Workfront之间的公司名称，使用 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 数据存储演练

## 概述

在本练习中，我们将使用数据存储来同步公司列表与Workfront之间的公司名称。

这是Workfront和其他一些系统的公司单向同步的一部分。 目前，它仅会在CSV文件和Workfront之间同步。 但它也会在数据存储中维护一个表，该表将跟踪每个公司的CSV文件(CID)中的Workfront ID (WFID)和公司ID。 这将允许我们在未来某个时间点使其成为双向同步。

![融合场景的图像](assets/data-structures-and-data-stores-2.png)

## 数据存储演练

Workfront建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>有关完成演练的分步说明，请转到 [数据存储演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 运动。


## 最终注释

既然您已学习完数据结构和数据存储，您可能会问自己：“何时应使用它们？”

数据结构最常用于序列化或解析数据格式，如JSON、XML、CSV等。 通过数据结构，您可以控制数据的结构，甚至可以验证数据。 使用数据结构的最常见原因是创建有效数据以发送到预期JSON或XML的API。 在这些情况下，您需要使用JSON或XML应用程序以及数据结构，以确保数据格式正确。

数据存储只应用于存储需要由多个场景执行访问的永久数据。 例如，对于需要精确控制处理的高级用例，您可以存储有关上次处理的记录的元数据。

数据存储不是设计为data warehouse或日志记录。 在Workfront Fusion之外无法访问数据存储，并且大多数与数据存储的交互都是通过Workfront Fusion场景进行的。 因此，无法将数据存储连接到data warehouse和日志记录用例所预期的分析或报表工具。 在像这样的用例中，Workfront Fusion的作用是填充适合组织和存储数据的系统（例如SQL、MariaDB）。

## 想要了解更多信息？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
