---
title: 在过滤器中创建 OR 语句
description: 通过Workfront灵活的过滤器逻辑，用户可以使用默认的“AND”规则、可选的“OR”条件以及针对复杂标准的有组织过滤器组来优化报表视图。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: b3cff8f86ceeb6e79e2b88ab335b2671aa25600a
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 31%

---

# 在过滤器中创建 OR 语句

此视频介绍如何在Workfront中创建和使用具有多个规则的过滤器。&#x200B;AEM 默认情况下，Workfront在筛选规则之间使用“AND”，这意味着所有条件都必须为true，项目才能显示在列表中。
或者，您也可以将过滤器逻辑更改为“或”，以显示符合任何条件的项目。
该视频还演示了如何使用过滤器组为任务创建过滤器。&#x200B;AEM 例如，您可以创建两个组：一个用于分配给创意团队的未完成任务延迟，另一个用于分配给创意团队的未完成任务未分配。&#x200B;AEM 在每个组中，“与”逻辑适用，这意味着必须满足组中的所有条件。&#x200B;AEM 组之间的“OR”逻辑可确保显示满足任一组条件的任务。

>[!VIDEO](https://video.tv.adobe.com/v/3470703/?quality=12&learn=on&captions=chi_hans)

## OR 过滤器活动

您想要查找分配给您或未分配给任何人的未完成任务。您设置了一个如下所示的过滤器。这个过滤器会为您带来想要的结果吗？为什么会或者为什么不会？

![图像：创建有误的 OR 语句，位于 [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### 答案

否，此过滤器不会提供您期望的结果（未完成的任务，已分配给您或未分配给任何人），因为任务完整性的过滤器规则仅在OR的一侧。

相反，此过滤器将会生成一个列表，其中显示：

* 分配给您的未完成任务。
* **以及（或者）**
* 所有未分配的任务，无论状态如何。

该过滤器应如下所示。请注意，此过滤器在OR两侧具有任务完整性的过滤器规则。

![图像：创建正确的 OR 语句，位于 [!DNL Workfront]](assets/or-statement-your-turn-2.png)
