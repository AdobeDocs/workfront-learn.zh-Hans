---
title: 显示时间会影响项目时间轴
description: 查看关闭设置时间时项目时间轴会发生什么情况。
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
kt: 10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 2%

---

# 关闭时间如何影响项目时间轴

分配的用户在项目时间轴中的逗留时间是否取决于名为的项目设置 [!UICONTROL User Time Off]. 此设置确定任务的主要任务负责人的休息时间是否调整项目上该任务的计划日期。

让我们看看在选择每个设置时项目时间轴会发生什么情况 — C[!UICONTROL onsider user time off in task durations] 或 [!UICONTROL Ignore user time off in task durations].

![用户关闭时间设置](assets/toapt_01.png)

## 考虑任务持续时间中的用户空闲时间

此选项是Workfront的默认设置。

在本例中，任务的主要受分配人在其个人日历上标记了休假天数。

![个人日历](assets/toapt_02.png)

项目经理希望将此人员分配给具有计划日期且与用户休假时间重叠的任务。

![具有日期的项目任务](assets/toapt_03.png)

将此用户分配到任务后，计划日期会自动调整。 现在，任务的计划完成日期已延长数天，以适应用户的休假时间。 请务必注意，此更改可能会影响项目中其他任务的计划日期，并可能影响项目的计划完成日期。

![项目任务到期日期](assets/toapt_04.png)

## [!UICONTROL Ignore user time off in task durations]

使用此选项，任务的计划日期将保持最初计划的状态，即使主受分配人在该任务的持续时间内有休息时间。

该团队成员的日历上有天假。

![已标记结束日期的pto日历](assets/toapt_05.png)

项目经理会为他们分配一个与结束时间重叠的任务。 分配用户后，任务计划日期将保持原计划的状态。

![调整项目任务日期](assets/toapt_06.png)

为确保工作按时完成，在原始受让人不在办公室时指派可以处理任务的其他人可能会有所帮助。

## 在项目级别调整设置

要更改项目上的用户关闭时间设置，请执行以下操作：

* 在Workfront中单击项目名称以打开该项目。

* 选择 [!UICONTROL Edit] 从页面标题的3个圆点菜单中，找到项目名称的右侧。

* 滚动到 [!UICONTROL Project Settings] 部分，然后查找 [!UICONTROL User Time Off] 字段。

* 选择要应用于此项目的选项 —  [!UICONTROL Consider user time off in task durations] 或[!UICONTROL gnore user time off in task durations].

* 单击 [!UICONTROL Save] 按钮。

![考虑任务持续时间中的用户空闲时间](assets/toapt_07.png)


**注意**:当您选择 [!UICONTROL Project Details] 从项目页面的左侧面板菜单。

中的项目首选项中存在用于此设置的全局设置 [!UICONTROL Setup] 菜单。 此设置由系统管理员管理。 群组管理员可以为其管理的群组调整此设置。

Workfront建议您按照希望大多数项目在您的组织内处理休息时间的方式设置该设置。

还可以通过模板详细信息将设置内置到项目模板中。
