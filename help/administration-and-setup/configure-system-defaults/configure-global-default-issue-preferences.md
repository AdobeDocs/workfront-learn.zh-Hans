---
title: 配置全局默认问题首选项
description: 了解如何为已转换的问题、实际日期和问题访问权限设置问题首选项。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 74%

---

# 配置全局默认问题首选项

一些系统范围的设置会为 [!DNL Workfront] 中某些情况下的问题行为建立了默认值。

最佳实践是保留全局默认值不变，并允许项目经理在项目级别或项目模板中进行所需的调整。

全局问题偏好设置可以调整，但建议您和您的[!DNL Workfront]顾问讨论组织的工作流、流程和报告需求所需的设置。 您的顾问还可以帮助您了解如果更改某些设置会发生什么。

问题首选项允许系统管理员控制将问题转换为任务或项目时的选项、实际日期的计算方式以及分配问题时谁可以访问项目。我们来看看这些设置在[!DNL Workfront]中的位置。

## 转换后的问题首选项

这些设置控制问题在[!DNL Workfront]中转换为任务或项目时发生的情况。

![[!UICONTROL Tasks & Issues] 首选项窗口，其中突出显示 [!UICONTROL Issues] 部分](assets/admin-fund-issue-prefs-converting.png)

1. 单击 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单面板中的 **[!UICONTROL Project Preferences]** 部分。
1. 选择 **[!UICONTROL Tasks & Issues]**。
1. 滚动到 **[!UICONTROL Issues]** 部分。
1. 单击所需的选项。
1. 完成后保存。

让我们看一下此部分中的选项，以使您可为您的组织选择适当的选项。

* **[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object Changes]**

  通过此设置，您可以将原始问题的解决方案与新对象（任务或项目）的解决方案关联起来。

  启用（选中）此设置后，您可以创建与任务或项目状态具有相同状态键的自定义问题状态。当任务或项目（可解决对象）设置为自定义状态时，相关的更改也会显示在问题状态中。

  禁用后，解决对象状态会自动设置为默认状态，而不是自定义状态。

  要使此设置生效，必须选择“[!UICONTROL Keep the original issue and tie its resolution to the task]”选项。

* **[!UICONTROL Keep the original issue and tie is resolution to the task/project]**

  当问题被转换时，这会告诉 [!DNL Workfront] 保留原始问题。问题的状态会随着任务或项目的状态发生变化而改变。当任务或项目被标记为已完成时，该问题就会被标记为已解决。

  如果未选中此选项，则原始问题会被删除，并且仅会保留转换后的任务或项目。

  此设置会影响对最初在项目上记录的问题或通过 [!DNL Workfront] 请求队列产生的问题的报告。

* **[!UICONTROL Allow Primary Contact to have access to the task/project]**

  这使得创建原始问题的人员可以在转换期间访问创建的任务或项目。他们可以审查工作、进行更新并随时了解其进展情况。

* **[!UICONTROL Allow these settings to be changed during conversion]**

  选中此选项后，表示转化问题的用户可更改“[!UICONTROL Keep original issue]”和“[!UICONTROL Allow Primary Contact]”的默认设置。 如果您希望默认值保持不变，请取消选择此选项。

<!--
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
-->

## 实际日期首选项

[!DNL Workfront] 中使用多种类型的日期。实际日期是[!DNL Workfront]在某些状态发生更改时生成的“时间戳”。

当问题状态从“新建”变为另一状态时，会创建 [!UICONTROL Actual Start Date] 时间戳。[!UICONTROL Actual Completion Date] 时间戳是指问题状态何时更改为表示其已关闭的状态。

请注意，此首选项控制任务和问题的实际日期设置，这一点很重要。

![[!UICONTROL Tasks & Issues] 首选项窗口，其中突出显示 [!UICONTROL Actual Dates] 部分](assets/admin-fund-issue-prefs-actual-dates.png)

1. 单击 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单面板中的 **[!UICONTROL Project Preferences]** 部分。
1. 选择 **[!UICONTROL Tasks & Issues]**。
1. 滚动到 **[!UICONTROL Actual Dates]** 部分。
1. 为 **[!UICONTROL Actual Start Date]** 选择所需的选项 — [!UICONTROL Now]（当前日期和时间）或 [!UICONTROL The Planned Start Date]（[!UICONTROL Actual Start Date] 与问题详细信息中设置的日期匹配）。
1. 现在为 **[!UICONTROL Actual Completion Date]** 选择选项 — [!UICONTROL Now]（当前日期和时间）或 [!UICONTROL The Planned Completion Date]（[!UICONTROL Actual Start Date] 与问题详细信息中设置的日期匹配）。
1. 完成后保存。


<!--
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
-->

## 问题访问权限

当在Workfront中为问题分配任务时，问题的[!UICONTROL Access]设置控制授予用户的访问权限。 这些设置除了控制对与问题关联的项目的访问权限外，还控制对问题本身的访问权限。

在更改这些设置之前，请与您的 [!DNL Workfront] 顾问和内部治理团队讨论任何工作流或流程需求。

![[!UICONTROL Tasks & Issues] 首选项窗口，其中突出显示 [!UICONTROL When someone is assigned to an ISSUE] 部分](assets/admin-fund-issue-prefs-access-1.png)

1. 单击 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单面板中的 **[!UICONTROL Project Preferences]** 部分。
1. 选择 **[!UICONTROL Tasks & Issues]**。
1. 滚动到&#x200B;**[!UICONTROL Access]**&#x200B;部分并找到“[!UICONTROL When someone is assigned to an ISSUE]”选项。
1. 设置问题本身的共享访问权限——[!UICONTROL View]、[!UICONTROL Contribute] 或 [!UICONTROL Manage]。[!DNL Workfront] 建议保留高级选项不变。
1. 如果问题受让人也应该有权访问该项目，请选中此框
1. 然后选择项目的共享访问权限—— [!UICONTROL View]、[!UICONTROL Contribute] 或 [!UICONTROL Manage]。在设置[!UICONTROL Advanced Options]时，请牢记组织的工作流和访问需求。
1. 完成后保存。

![[!UICONTROL Access] 窗口，其中显示 [!UICONTROL Contribute] 选项](assets/admin-fund-issue-prefs-access-2.png)

<!--
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
-->
