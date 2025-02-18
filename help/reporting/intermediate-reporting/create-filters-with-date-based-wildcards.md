---
title: 使用基于日期的通配符创建过滤器
description: 了解如何以及何时使用基于日期的通配符，以及如何基于当前日期构建过滤器。
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 70%

---

# 使用基于日期的通配符创建过滤器

在本视频中，您将学习如何：

* 知道何时使用基于日期的通配符
* 了解Workfront使用的两个基于日期的通配符之间的差异
* 将基于日期的通配符添加到过滤器
* 使用通配符、属性、运算符和修饰符创建自定义日期
* 使用通配符创建自定义日期范围

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)


## 使用基于日期的通配符活动创建过滤器

[单击此处](/help/assets/create-filters-with-date-based-wildcards-activities.pdf)下载此页面的 PDF。

### 活动问题

1. 如果您想要查看截止日期为昨天或今天的问题，您将如何构建过滤规则？
1. 您将如何构建过滤规则来查找上周到期的项目？
1. 以下过滤规则是您经常使用的任务报告的一部分。您会从这份报告中得到什么类型的结果？

![使用基于日期的通配符创建任务过滤器的屏幕图像](assets/date-wildcard-answer-1.png)

### 答案

1. 过滤规划完成日期在 [!UICONTROL $$TODAY-1d] 和 [!UICONTROL $$TODAY] 之间的问题。
1. 过滤规划完成日期在 [!UICONTROL $$TODAYb-1w] 和 [!UICONTROL $$TODAYe-1w] 之间的项目。
1. 此报表查找分配给您的尚未完成（换句话说，完成百分比小于100）以及今天过期或到期的任务。 任务的计划完成日期的筛选规则表示，查看到期日期等于或早于今天日期的任务。
