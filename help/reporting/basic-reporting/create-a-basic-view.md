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
kt: 8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# 创建基本视图

在本视频中，您将了解：

* Workfront中的视图
* 如何创建和修改视图
* 如何与其他Workfront用户共享视图

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12)

## 活动：创建基本视图

作为项目经理、团队负责人或资源经理，您希望跟踪任务工作的进展情况。 通过此视图，您可以在列表或报告的一行中获取任务的多个状态指示器。

创建名为“任务状态视图”的任务视图，该视图具有以下列：

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Percent Complete]
* [!UICONTROL Status]
* [!UICONTROL Progress Status]
* [!UICONTROL Status Icons]

## 答案

![用于创建新视图的屏幕图像](assets/view-exercise.png)

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
