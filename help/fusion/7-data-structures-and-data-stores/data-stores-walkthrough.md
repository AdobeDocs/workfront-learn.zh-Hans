---
title: 数据存储演练
description: 了解如何使用数据存储在公司列表和 Workfront 之间使用  [!DNL Adobe Workfront Fusion] 同步公司名称。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '393'
ht-degree: 100%

---

# 数据存储演练

在本练习中，我们会使用数据存储来同步公司列表和 Workfront 之间的公司名称。

这是 Workfront 和其他系统中公司单向同步的一个部分。目前，它只会在 CSV 文件和 Workfront 之间同步。但它还会在数据存储中维护一个表，用于跟踪每个公司的 Workfront ID (WFID) 和 CSV 文件中的公司 ID (CID)。这将使我们能够在将来的某个时候将其设为双向同步。

![Fusion 场景的图像](assets/data-structures-and-data-stores-2.png)

## 数据存储演练

Workfront 建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/3417967/?quality=12&learn=on&enablevpops&captions=chi_hans)



## 最后说明

现在您已经完成了有关数据结构和数据存储的学习，您可能会问自己：“应该在什么时候使用它们呢？”

数据结构最常用于序列化或解析 JSON, XML, CSV 等数据格式。数据结构使您能够控制数据的结构，甚至还能验证数据。使用数据结构的最常见原因是为了创建有效的数据，以发送到需要 JSON 或 XML 的 API。在这些情况下，您需要将 JSON 或 XML 应用程序与数据结构一起使用，以确保数据具有正确的格式。

数据存储应仅用于存储需要由多个场景执行访问的持久数据。例如，您可以存储有关需要对处理进行精确控制的高级用例所处理的最后一条记录的元数据。

数据存储的目的不是用作数据仓库或日志记录。数据存储在 Workfront Fusion 之外是不可访问的，并且与数据存储的大多数交互都是通过 Workfront Fusion 场景进行的。因此，无法将数据存储连接到数据仓库和日志记录用例所需的分析或报告工具。Workfront Fusion 在此类用例中的作用是填充适合组织和存储数据的系统（例如 SQL、MariaDB）。

## 想要了解详情？我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hans)
