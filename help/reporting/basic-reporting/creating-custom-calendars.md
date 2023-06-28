---
title: 创建自定义日历
description: 了解如何创建自己的自定义日历，以显示您的工作项和个人休息时间。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: create-a-custom-calendar.png
jira: KT-10024
exl-id: d5c928f2-7989-401f-ad86-08fe971c9ff5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# 创建自定义日历

在本节中，您将了解如何：

* 创建新日历
* 创建日历分组
* 将工作项添加到日历分组
* 创建休息时间日历

以下是如何创建自己的自定义日历。

## 首先，添加新日历

1. 从 **[!UICONTROL Main Menu]**，选择 **[!UICONTROL Calendars]** 区域。
1. 单击 **[!UICONTROL New Calendar]** 选项。
1. 键入日历的名称，然后按 **[!UICONTROL Return]**.

## 第二，添加日历分组

1. 要显示与特定项目相关的项，请在 [!UICONTROL grouping] 字段（显示与该项目相关的所有任务）。
1. 或者单击 **[!UICONTROL Add advanced items]** 选项，用于将来自各种项目的工作项包含在系统中。

![用于向日历添加分组的屏幕图像](assets/calendar-2-1.png)

## 第三，将工作项添加到日历分组

1. 命名分组以反映要显示的内容。
1. 为组选择颜色指定。
1. 选择要使用的日期类型 — [!UICONTROL Projected dates]， [!UICONTROL Planned dates]，或 [!UICONTROL Custom]. ([!UICONTROL Custom] 日期是包含的日期字段 [!UICONTROL custom forms].)
1. 选择要在日历上显示的日期 — [!UICONTROL End Date Only]， [!UICONTROL Start Date Only]，或 [!UICONTROL Duration (Start to End)].
1. 如果要显示 [!UICONTROL Actual dates] 在该信息可用时，从菜单中选择“是”。 如果您始终希望使用选定的日期类型，请选择“否”([!UICONTROL Projected]， [!UICONTROL Planned]，或 [!UICONTROL Custom])以显示。
1. 选择要在日历中看到的项目信息类型 — [!UICONTROL Tasks]， [!UICONTROL Projects]， [!UICONTROL Issues]，或 [!UICONTROL Time Off].
1. 设置过滤器以显示所需信息。
1. 单击 **[!UICONTROL Save]**.

![用于将工作项添加到日历分组的屏幕图像](assets/calendar-2-2.png)

>[!NOTE]
>
>通过使用“添加到日历”选项，可以将其他分组添加到现有日历中。

## 创建显示个人休息时间的日历

[!DNL Workfront] 提供一种方法，让您在用户配置文件中使用个人休息时间功能指定休息时间。 这会提醒项目经理您不可用，并允许计划的完成日期根据需要自动或手动调整。

在“日历”区域中，您可以创建一个显示这些休息时间条目的日历视图。

要为特定人员创建日历，请执行以下操作：

1. 单击 **[!UICONTROL Add to Calendar]** （在左侧面板中）。
1. 单击 **[!UICONTROL Add advanced items]**.
1. 命名分组以反映要显示的内容。
1. 为分组选择颜色指定。
1. 设置 [!UICONTROL Date Field] 到 [!UICONTROL Planned dates].
1. 选择要在日历上显示的日期 — [!UICONTROL Duration].
1. 忽略在实际日期不可用时信息的显示方式。 不适用。
1. 选择 [!UICONTROL Time Off] 以了解要查看的信息类型。
1. 对于筛选器，将用户ID设置为团队成员的姓名。
1. 单击 **[!UICONTROL Save]**.

![用于向日历分组添加休息时间条目的屏幕图像](assets/calendar-2-3.png)
