---
title: 使用基于用户的通配符创建过滤器
description: 了解如何使用基于用户的通配符以及如何基于登录用户构建过滤器。
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 48%

---

# 使用基于用户的通配符创建过滤器

在本视频中，您将学习如何：

* 了解为什么使用通配符
* 使用基于用户的通配符构建过滤器

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>构建能够查看任务或问题分配信息的过滤器时，请使用“任务用户” >> “ID 字段源和名称”。此选项会查看所有   分配给任务或问题的用户，而不仅仅是“所有者”或主要受让人。

>[!TIP]
>
>即使在为自己构建过滤器时也请使用 $$USER.ID（而不是您的名字）。这样，如果有人看到您正在运行的过滤器并显示“与我共享”，则该过滤器已设置，因此使用该过滤器的每个人都会看到自己的信息。

>[!TIP]
>
>使用基于用户的通配符时，您必须使用“等于”过滤限定符。


## 使用基于用户的通配符活动创建过滤器

[单击此处](/help/assets/create-filters-with-user-based-wildcards-activities.pdf)下载此页面的 PDF。

### 活动1

这周你有一些额外的时间，所以你想看看你的团队中是否有任何人在他们的任务中可以使用一些帮助。 创建任务筛选器以查找本周到期但尚未完成的任务。

### 答案1

你帮助队友真是太棒了！ 设置如下图所示的过滤器，您会发现任务：

* 尚未完成的任务（即，他们没有等于[!UICONTROL Complete]的[!UICONTROL Complete]状态或状态）；
* 这些项目中的项目具有[!UICONTROL Current]状态（毕竟，您不希望为尚未启动的项目查找任务）；
* 根据 Workfront 团队设置的定义，分配给您主团队中某个人的任务；
* 而且完成日期为本周某个时间的（此规则使用预建日期过滤器来定义“本周”）。

![使用基于用户的通配符创建任务过滤器的屏幕图像](assets/user-wildcard-exercise-answer.png)

如果您需要进一步限制列表，则可能需要添加一些额外的过滤器。例如，您可能需要添加一个过滤规则来查看您的团队使用的特定程序或项目组合。
