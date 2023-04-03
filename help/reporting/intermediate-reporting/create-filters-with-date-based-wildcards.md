---
title: 使用基于日期的通配符创建过滤器
description: 了解如何以及何时使用基于日期的通配符，以及如何根据当前日期构建过滤器。
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
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 使用基于日期的通配符创建过滤器

在此视频中，您将学习如何：

* 了解何时使用基于日期的通配符
* 了解Workfront的两个基于日期的通配符之间的差异
* 向过滤器添加基于日期的通配符
* 使用通配符、属性、运算符和修饰符创建自定义日期
* 使用通配符创建自定义日期范围

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)

## 活动问题

1. 如果希望某个截止日期为昨天或今天的问题，应如何构建过滤器规则？
1. 如何构建过滤器规则以查找上周到期的项目？
1. 以下过滤器规则是您定期使用的任务报表的一部分。 您会从此报表获得哪类结果？

![用于创建任务过滤器的屏幕图像，带有基于日期的通配符](assets/date-wildcard-answer-1.png)

## 答案

1. 在以下日期之间过滤发布计划完成日期 [!UICONTROL $$TODAY-1d] 和 [!UICONTROL $$TODAY].
1. 在项目计划完成日期之间进行筛选 [!UICONTROL $$TODAYb-1w] 和 [!UICONTROL $$TODAYe-1w].
1. 此报表会查找分配给您的尚未完成的任务（换言之，完成百分比小于100），以及已逾期或今天到期的任务。 任务计划完成日期的过滤器规则用于查看到期日等于当天日期或早于当天日期的任务。
