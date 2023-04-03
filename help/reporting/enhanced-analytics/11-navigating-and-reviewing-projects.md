---
title: 了解在中导航和审核项目 [!UICONTROL Enhanced Analytics]
description: 了解如何阅读Workfront的飞行计划图。
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# 了解在中导航和审核项目 [!UICONTROL Enhanced Analytics]

在此视频中，您将学习：

* 如何阅读飞行计划图

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## 飞行计划图

![飞行计划图表的图像，其编号与下面的项目符号匹配](assets/section-2-1.png)

在图表上，您会看到：

1. 项目名称位于左侧。
1. 日期在底部显示。
1. 垂直蓝线显示鼠标悬停的特定日期。
1. 水平蓝线显示项目的计划开始日期和结束日期。
1. 绿色线条表示项目处于“目标”状态。
1. 橙色线条表示项目面临风险。
1. 红线表示项目出现问题。

查看有关项目的此信息可帮助您确定：

* 哪些事件会将项目延长到计划完成日期之后。
* 当项目开始出现问题时。
* 同一时间段内打开的项目数量。
* 活动项目的数量。
* 哪些项目需要特别关注或支持。

## 条件基于进度状态

项目条件直观地显示了项目的进展情况。 Workfront根据项目中任务的进度状态确定条件。

![可能的进度状态图像](assets/section-2-2.png)

可以设置项目的条件：

* **手动**，则当项目的条件类型设置为“手动”时，用户将有权管理项目。 这样，您就可以独立于关键路径来设置项目的条件。
* **自动**，由Workfront指定。

Workfront建议您将条件类型设置为“进度状态”，以便根据任务的进度清晰地指示项目的实际进度。

![可能的进度状态图像](assets/section-2-3.png)

在这种情况下，项目条件可以是：

* **On Target** — 当关键路径上最后一个任务的进度状态为“开启”时，项目的条件将为“启动”。 项目正在跟踪以按计划完成。
* **面临风险** — 当关键路径上最后一个任务的进度状态为“落后”或“处于危险”时，项目的状态为“处于危险”。 该项目有望很晚完成，但还不晚。
* **遇到麻烦** — 当关键路径上最后一个任务的进度状态为“延迟”时，则项目的条件为“出现问题”。 到期日期已过，项目现在已延迟。

>[!NOTE]
>
>可以针对您的环境自定义条件，以便您可以找到三个以上的选项，或者名称可能与上述选项不同。 有关自定义条件的信息，请参阅文章创建或编辑自定义条件。
