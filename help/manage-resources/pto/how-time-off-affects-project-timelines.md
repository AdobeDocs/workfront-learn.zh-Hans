---
title: 显示休息时间会影响项目时间线
description: 查看当休息时间设置打开和关闭时项目时间线会发生什么情况。
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 2%

---

# 休息时间对项目时间线的影响

分配用户的休息时间是否计入项目时间线取决于名为的项目设置 [!UICONTROL User Time Off]. 该设置确定任务的主要被分配人的休息时间是否调整了项目上该任务的计划日期。

让我们看一下选择每个设置后项目时间线会发生什么情况 — C[!UICONTROL onsider user time off in task durations] 或 [!UICONTROL Ignore user time off in task durations].

![用户休息时间设置](assets/toapt_01.png)

## 考虑任务持续时间中的用户空闲时间

此选项是Workfront的默认设置。

在本例中，任务的主要被分配人在个人日历上标记了休息日。

![个人日历](assets/toapt_02.png)

项目经理想要将此人分配给计划日期与用户的休息时间重叠的任务。

![具有日期的项目任务](assets/toapt_03.png)

当此用户被分派到任务时，将自动调整计划日期。 现在，任务的计划完成日期已延长几天，以适应用户的休息时间。 请务必注意，此更改可能会影响项目中其他任务的计划日期，并可能影响项目的计划完成日期。

![具有到期日期的项目任务](assets/toapt_04.png)

## [!UICONTROL Ignore user time off in task durations]

利用此选项，任务的计划日期保持与原计划日期相同，即使主要被分配人在任务持续期间具有空闲时间。

团队成员在其日历上标记了休息日。

![带有已标记关闭日期的pto日历](assets/toapt_05.png)

项目经理为他们分配一个与休息时间重叠的任务。 分配用户后，任务计划日期仍保持原计划。

![调整项目任务日期](assets/toapt_06.png)

为了确保按时完成工作，在原始被分配人不在办公室时，分配另一个能够处理该任务的人可能会有所帮助。

## 调整项目级别的设置

要更改项目的“用户休假”设置，请执行以下操作：

* 在Workfront中单击项目名称以打开该项目。

* 选择 [!UICONTROL Edit] 从页眉中的3个圆点菜单，到项目名称的右侧。

* 滚动到 [!UICONTROL Project Settings] 部分并查找 [!UICONTROL User Time Off] 字段。

* 选择要应用于此项目的选项 —  [!UICONTROL Consider user time off in task durations] 或I[!UICONTROL gnore user time off in task durations].

* 单击 [!UICONTROL Save] 按钮来打开窗口。

![考虑任务持续时间中的用户空闲时间](assets/toapt_07.png)


**注释**：此设置在你选择时不可用 [!UICONTROL Project Details] 从项目页面的左侧面板菜单中。

在的项目首选项中，存在全局设置进行此设置 [!UICONTROL Setup] 菜单。 此设置由系统管理员管理。 组管理员可以为其管理的组调整此设置。

Workfront建议设置您希望组织的大多数项目都处理休假的方式。

还可通过模板详细信息将该设置内置到项目模板中。
