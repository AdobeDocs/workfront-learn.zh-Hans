---
title: 从项目时间线中跟踪进度
description: 了解如何从中的项目时间线跟踪工作进度 [!DNL  Workfront] 使用完成百分比、状态、分配或约束。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Intermediate
jira: KT-10150
exl-id: c8793f49-24b8-48cc-af84-5239234ead0e
source-git-commit: e25a7c0119567c068504edcb8c3ddd29622d52c5
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 从项目时间线中跟踪进度

确保任务按应在项目截止日期前完成的方式进行。 扫描时 [!UICONTROL Task] 列表，中有几个功能 [!DNL  Workfront] 可以帮助您监控工作的进度和状态。

## 完成百分比

每个工作任务的完成百分比有时用于衡量工作的进展情况。 请注意……此字段必须手动调整，因为它是被分派人估计其持续时间。

>[!TIP]
>
>尽管工作任务的完成百分比需要手动更新，但Workfront会根据每个子任务的完成百分比以及持续时间或计划小时数计算父任务的完成百分比。 这意味着，如果将大型任务分解为较小的子任务，您将获得更好的完成百分比准确性。


![项目任务列表显示 [!UICONTROL Percent Complete] 列](assets/planner-fund-task-percent-complete.png)

完成百分比会自动更改的情况有三次：

* 当任务 [!UICONTROL Status] 设置为“完成”，则完成百分比将更改为100。
* 如果任务 [!UICONTROL Status] 回退到新，完成百分比将重置为0。
* 在父任务中，当子任务的完成百分比发生变化时。

## 状态

包括 [!UICONTROL Status] 中的列 [!UICONTROL View] 以快速查看哪些任务已开始、正在进行以及已完成。 您甚至可以在 [!UICONTROL View] 对每个状态进行彩色编码，使信息更易于解密。

## 任务分派

在审阅项目时，审阅任务分配。 也许工作落后，因为没有人被分派这项任务。 或者被分配人没有合适的技能集来完成工作。 将更多人员添加到任务或重新分配任务以确保完成工作。

## 任务限制

有时任务限制会发生变化，而您并没有意识到这一点。 限制会影响时间线的行为，因此您应该确保已按照所需的方式设置限制。

![显示任务限制列的项目任务列表](assets/planner-fund-task-constraint.png)

创建自定义视图，视图包括 [!UICONTROL Task Constraint] 列，可在任务列表中查看此信息。 如果您从开始日期起计划项目，则希望任务具有 [!UICONTROL As Soon As Possible] ([!UICONTROL ASAP])约束。

有关任务限制的更多详细信息，请参阅 [了解和管理持续时间类型和任务限制](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).
