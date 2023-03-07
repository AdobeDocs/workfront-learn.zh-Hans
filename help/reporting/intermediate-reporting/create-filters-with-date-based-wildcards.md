---
title: 使用基于日期的通配符创建过滤器
description: 了解如何使用基于日期的通配符以及何时使用，以及如何根据当前日期构建过滤器。
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 使用基于日期的通配符创建过滤器

在本视频中，您将了解如何：

* 了解何时使用基于日期的通配符
* 了解Workfront中两个基于日期的通配符之间的区别
* 向筛选器添加基于日期的通配符
* 使用通配符、属性、运算符和修饰符创建自定义日期
* 使用通配符创建自定义日期范围

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## 活动问题

1. 如果您希望出现截止日期为昨天或今天的问题，如何构建过滤器规则？
1. 如何构建筛选规则以查找上周到期的项目？
1. 以下筛选规则是您定期使用的任务报告的一部分。 您会从此报告获得什么类型的结果？

![用于使用基于日期的通配符创建任务过滤器的屏幕图像](assets/date-wildcard-answer-1.png)

## 答案

1. 筛选介于以下日期之间的问题计划完成日期 [!UICONTROL $$TODAY-1d] 和 [!UICONTROL $$TODAY].
1. 筛选介于以下日期之间的项目计划完成日期 [!UICONTROL $$TODAYb-1w] 和 [!UICONTROL $$TODAYe-1w].
1. 此报表查找分配给您的尚未完成（换句话说，完成百分比小于100）并且今天过期或到期的任务。 任务的计划完成日期的筛选规则指示查看到期日期等于或早于今天日期的任务。
