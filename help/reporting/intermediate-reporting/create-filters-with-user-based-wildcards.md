---
title: 使用基于用户的通配符创建过滤器
description: 了解如何使用基于用户的通配符以及如何根据登录的用户构建过滤器。
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 使用基于用户的通配符创建过滤器

在本视频中，您将了解如何：

* 了解为何使用通配符
* 使用基于用户的通配符构建过滤器

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>构建查看任务或问题分配信息的过滤器时，请使用分配用户>> ID字段源和名称。  此选项查看分配给任务或问题的所有用户，而不仅仅是“所有者”或主要被分配人。

>[!TIP]
>
>使用$$USER.ID（而不是您的姓名），即使您自己构建过滤器也是如此。 这样，如果有人看到您正在运行的过滤器并显示“与我共享”，则该过滤器已设置，因此使用该过滤器的每个人都会看到自己的信息。

>[!TIP]
>
>在使用基于用户的通配符时，必须始终使用相等过滤器限定符。

## 活动

这周你有一些额外的时间，所以你想看看你的团队中是否有任何人在他们的任务中可以使用一些帮助。 创建任务筛选器以查找本周到期但尚未完成的任务。

## 答案

你帮助队友真是太棒了！ 通过如下图所示的过滤器设置，您可以找到任务：

* 尚未完成(这意味着它们没有 [!UICONTROL Complete] 相等的状态或状态 [!UICONTROL Complete])；
* 这些项目中具有的 [!UICONTROL Current] 状态（毕竟，您不希望为尚未启动的项目查找任务）；
* 如Workfront团队设置所定义，分配给您的主团队中的某个人；
* 而且完成日期为本周某个时间的（此规则使用预建日期过滤器来定义“本周”）。

![用于创建具有基于用户的通配符的任务过滤器的屏幕图像](assets/user-wildcard-exercise-answer.png)

如果需要进一步限制列表，您可能需要添加一些其他过滤器。 例如，您可能希望添加一个过滤器规则，用于查看您团队处理的特定项目或项目组合。
