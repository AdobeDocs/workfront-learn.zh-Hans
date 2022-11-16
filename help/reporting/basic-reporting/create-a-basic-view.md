---
title: 创建基本视图
description: 了解视图是什么，如何创建视图，以及如何与Workfront中的其他用户共享视图。
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# 创建基本视图

在此视频中，您将学习：

* 什么风景在Workfront
* 如何创建和修改视图
* 如何与其他Workfront用户共享视图

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12)

## 活动：创建基本视图

作为项目经理、团队负责人或资源经理，您希望跟踪任务工作的进展情况。 通过此视图，您可以在列表或报表的一行中获得任务的多个状态指示器。

创建名为“任务状态视图”的任务视图，并包含以下列：

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Percent Complete]
* [!UICONTROL Status]
* [!UICONTROL Progress Status]
* [!UICONTROL Status Icons]

## 回答

![用于创建新视图的屏幕图像](assets/view-exercise.png)

1. 在任务列表报表中，转到 **[!UICONTROL View]** 下拉菜单，然后选择 **[!UICONTROL New View]**.
1. 将视图命名为“任务状态视图”。
1. 删除这些列： [!UICONTROL Pln Hrs], [!UICONTROL Predecessors], [!UICONTROL Start On]和 [!UICONTROL Due On].
1. 单击 **[!UICONTROL Add Column]**.
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后选择“status” [!UICONTROL Task] 字段源。
1. 单击 **[!UICONTROL Add Column]** 再次。
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后选择“Progress Status”（进度状态） [!UICONTROL Task] 字段源。
1. 单击 **[!UICONTROL Add Column]** 再次。
1. 在 [!UICONTROL Show in this column] 字段中，键入“status”，然后在“任务”字段源下选择“Status Icons”。
1. 单击 **[!UICONTROL Save]**.

将鼠标悬停在 [!UICONTROL Status Icons] 列来查看它们所代表的内容。 如果灰显，则表示任务没有注释、文档、审批流程等。 如果图标以颜色显示，则至少有一个项目与任务关联。 您可以单击注释或文档图标以转到该项目。
