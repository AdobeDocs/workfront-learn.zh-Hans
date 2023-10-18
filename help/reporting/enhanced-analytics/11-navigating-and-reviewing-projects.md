---
title: 了解如何导航和审查项目
description: 了解如何在中阅读外部测试版计划表 [!UICONTROL Enhanced Analytics].
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 了解如何导航和审查项目

在本视频中，您将了解：

* 如何阅读外部测试版计划表

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## 外部测试版计划图

![飞行计划图的图像，其数字与下面的项目符号相匹配](assets/section-2-1.png)

在图表上，您会看到：

1. 项目名称在左侧。
1. 日期显示在底部。
1. 垂直蓝线显示鼠标悬停的特定日期。
1. 水平蓝线显示项目的计划开始日期和结束日期。
1. 绿色线条表示项目符合目标。
1. 橙色线条表示项目有风险。
1. 红线表示项目存在问题。

查看关于您项目的此信息可帮助您确定：

* 哪些事件使项目延长超过计划的完成日期。
* 当项目开始遇到问题时。
* 同一时间段内打开的项目数。
* 有多少项目处于活动状态。
* 哪些项目需要额外的关注或支持。

## 完成情况基于进度状态

项目完成情况直观地显示了项目的进展情况。 Workfront根据项目中任务的进度状态确定完成情况。

![可能进度状态的图像](assets/section-2-2.png)

可以设置项目的条件：

* **手动**，由具有管理项目权限的用户在项目的条件类型设置为手动时执行。 这允许您独立于关键路径设置项目的条件。
* **自动**，当Workfront将项目的条件类型设置为进度状态时。

Workfront建议您将条件类型设置为进度状态，以便根据任务的进度，清楚地指示项目的真正进度。

![可能进度状态的图像](assets/section-2-3.png)

当设置为“进度状态”时，项目完成情况可以是：

* **准时** — 当关键路径上最后一个任务的进度状态为“准时”时，项目的状态将为“准时”。 该项目有望按计划完成。
* **处于风险** — 当关键路径上最后一个任务的进度状态为“落后”或“存在风险”时，则项目的状态为“存在风险”。 项目按计划可能会延迟完成，但并未延迟。
* **存在问题** — 当关键路径上最后一个任务的进度状态为“延迟”时，则项目的状况为“存在问题”。 到期日期已过，项目现在延迟。

>[!NOTE]
>
>可以为您的环境自定义条件，因此您可能会找到三个以上的选项，或者名称可能与上述选项不同。 有关自定义条件的信息，请参阅文章 [创建或编辑自定义条件](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-conditions/create-edit-custom-conditions.html?lang=en).
