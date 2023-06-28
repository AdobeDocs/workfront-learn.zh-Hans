---
title: 创建基本视图
description: 了解视图是什么、如何创建视图以及如何在Workfront中与其他用户共享视图。
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 创建基本视图

在本视频中，您将了解：

* Workfront中的视图
* 如何创建和修改视图
* 如何与其他Workfront用户共享视图

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## 活动1：创建任务状态视图

作为项目经理、团队负责人或资源经理，您希望跟踪任务工作的进展情况。 通过此视图，您可以在列表或报告的一行中获取任务的多个状态指示器。

创建名为“任务状态视图”的任务视图，该视图具有以下列：

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Percent Complete]
* [!UICONTROL Status]
* [!UICONTROL Progress Status]
* [!UICONTROL Status Icons]

## 活动1答案

![用于创建任务状态视图的屏幕图像](assets/view-exercise.png)

1. 在任务列表报告中，转到 **[!UICONTROL View]** 下拉菜单并选择 **[!UICONTROL New View]**.
1. 将视图命名为“任务状态视图”。
1. 删除以下列： [!UICONTROL Pln Hrs]， [!UICONTROL Predecessors]， [!UICONTROL Start On]、和 [!UICONTROL Due On].
1. 单击 **[!UICONTROL Add Column]**.
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后选择“Status” [!UICONTROL Task] 字段源。
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后选择“Progress Status”（进度状态） [!UICONTROL Task] 字段源。
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后选择“Task”字段源下的“Status Icons”。
1. 单击 **[!UICONTROL Save]**.

将鼠标悬停在 [!UICONTROL Status Icons] 栏查看它们表示的内容。 如果它们呈灰显状态，则表示任务没有注释、文档、批准流程等。 如果图标以彩色显示，则至少有一个项目与任务相关联。 您可以单击注释或文档图标以转到该项目。

## 活动2：创建里程碑视图

如果您使用里程碑，则此视图是按名称查看里程碑并使用内联编辑添加或编辑它们的最简单方法。

创建名为“里程碑视图”的任务视图，该视图具有以下列：

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Pln Hrs]
* [!UICONTROL Milestone: Name]
* [!UICONTROL Start On]
* [!UICONTROL Due On]
* [!UICONTROL Percent Complete]


## 活动2答案

![用于创建里程碑视图的屏幕图像](assets/view-milestone-exercise-1.png)

1. 在项目任务列表中，转到 **[!UICONTROL View]** 下拉菜单并选择 **[!UICONTROL New View]**.
1. 将视图命名为“里程碑视图”。
1. 单击 [!UICONTROL Predecessors] 列进行选择。
1. 在 [!UICONTROL Show in this column] 字段中，单击 [!UICONTROL Task >> Predecessors] 字段，然后键入&#39;&#39;[!UICONTROL milestone name]”并单击“[!UICONTROL Name]”在列表中。
1. 单击 **[!UICONTROL Save]**.

![使用里程碑视图的任务列表图像](assets/view-milestone-exercise-2.png)

## 活动3：创建持续时间类型和任务约束视图

通过此视图，您可以检查和编辑项目中的所有持续时间类型和任务限制。

创建一个名为“持续时间类型和任务约束视图”的任务视图，该视图包含以下列：

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Planned Duration]
* [!UICONTROL Pln Hrs]
* [!UICONTROL Predecessors]
* [!UICONTROL Start On]
* [!UICONTROL Due On]
* [!UICONTROL Duration Type]
* [!UICONTROL Task Constraint]
* [!UICONTROL Constraint Date]

更改 [!UICONTROL Field Format] 在 [!UICONTROL Start On] 和 [!UICONTROL Due On] 列来同时显示日期和时间。

## 活动3答案

![显示持续时间类型和任务限制视图的屏幕图像](assets/view-activity-3.png)

1. 在项目任务列表中，转到 **[!UICONTROL View]** 下拉菜单并选择 **[!UICONTROL New View]**.
1. 将视图命名为“持续时间类型和任务限制视图”。
1. 删除 [!UICONTROL % Complete] 列。
1. 单击 **[!UICONTROL Add Column]**.
1. 在 [!UICONTROL Show in this column] 字段，类型 [!UICONTROL "duration"] 然后选择 [!UICONTROL "Planned Duration"] 在 [!UICONTROL Task] 字段源。
1. 将此列移动到 [!UICONTROL Duration] 和 [!UICONTROL Pln Hrs] 列。
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 在 [!UICONTROL Show in this column] 字段，类型 [!UICONTROL "duration type"] 然后选择 [!UICONTROL "Duration Type"] 在 [!UICONTROL Task] 字段源。
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 在 [!UICONTROL Show in this column] 字段，类型 [!UICONTROL "constraint"] 然后选择 [!UICONTROL "Task Constraint"] 在任务字段源下。
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 在 [!UICONTROL Show in this column] 字段，类型 [!UICONTROL "constraint"] 然后选择 [!UICONTROL "Constraint Date"] 在任务字段源下。
1. 选择 [!UICONTROL Start On] 列，然后单击 [!UICONTROL Advanced Options].
1. 在 [!UICONTROL Field Format] 下拉选择 [!UICONTROL "10/17/60 3:00 AM"].
1. 选择 [!UICONTROL Due On] 列，然后单击 [!UICONTROL Advanced Options].
1. 在 [!UICONTROL Field Format] 下拉选择 [!UICONTROL "10/17/60 3:00 AM"].
1. 单击 **[!UICONTROL Save]**.
