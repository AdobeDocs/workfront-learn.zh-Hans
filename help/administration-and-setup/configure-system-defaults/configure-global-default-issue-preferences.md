---
title: 配置全局默认问题首选项
description: 了解如何为已转换的问题、实际日期和问题访问权限设置问题首选项。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 配置全局默认问题首选项

一些系统范围的设置为问题在 [!DNL Workfront].

最佳做法是保留全局默认值，并允许项目经理在项目级别或项目模板中进行所需的调整。

可以调整全局问题首选项，但建议您和 [!DNL Workfront] 顾问讨论了贵组织的工作流、流程和报告需求需要哪些设置。 您的顾问还可以帮助您了解在某些设置发生更改时会发生什么情况。

问题首选项允许系统管理员在将问题转换为任务或项目时控制选项、如何计算实际日期以及在分配问题时由谁获得项目访问权限。 让我们看看这些设置在 [!DNL Workfront].

## 转换的问题首选项

这些设置可控制问题在转换为任务或项目(位于 [!DNL Workfront].

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL Issues] 突出显示的部分](assets/admin-fund-issue-prefs-converting.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 的双曲余切值。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Issues]** 中。
1. 单击所需的选项。
1. 完成后保存。

让我们查看此部分中的选项，以便您为组织选择适当的选项。

* **[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object Changes]**

   此设置允许您将原始问题的解决情况与新对象（任务或项目）的解决情况关联。

   启用（选中）此设置后，您可以创建与任务或项目状态具有相同状态键的自定义问题状态。 将任务或项目（可解析的对象）设置为自定义状态时，问题状态中也会显示更改。

   禁用后，解析对象状态将自动设置为默认状态，而不是自定义状态。

   要使此设置生效，请使用[!UICONTROL Keep the original issue and tie its resolution to the task]“ ”选项。

* **[!UICONTROL Keep the original issue and tie is resolution to the task/project]**

   当问题转换后，这表示 [!DNL Workfront] 以保留原始问题。 随着任务或项目的状态发生更改，问题的状态也会发生更改。 任务或项目标记为完成后，问题即被标记为已解决。

   如果未勾选此选项，则会删除原始问题，并且只保留已转换的任务或项目。

   此设置会影响最初在项目上记录或遇到的问题的报告 [!DNL Workfront] 请求队列。

* **[!UICONTROL Allow Primary Contact to have access to the task/project]**

   这样，创建原始问题的人员便可以访问在转换期间创建的任务或项目。 他们可以审查工作、进行更新并随时了解工作进展。

* **[!UICONTROL Allow these settings to be changed during conversion]**

   选中此选项后，表示“[!UICONTROL Keep original issue]&quot;和&quot;[!UICONTROL Allow Primary Contact]“ ”可由用户转换问题进行更改。 如果希望默认值保持不变，请取消选择此选项。

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 实际日期首选项

在整个过程中使用的日期类型有多种 [!DNL Workfront]. 实际日期是“时间戳”， [!DNL Workfront] 会在发生特定状态更改时生成。

的 [!UICONTROL Actual Start Date] 当问题状态从“新建”更改为其他状态时，将创建时间戳。 的 [!UICONTROL Actual Completion Date] 时间戳是指问题状态变为指示其已关闭的状态时。

请务必注意，此首选项控制任务和问题的实际日期设置。

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL Actual Dates] 突出显示的部分](assets/admin-fund-issue-prefs-actual-dates.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 的双曲余切值。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Actual Dates]** 中。
1. 为 **[!UICONTROL Actual Start Date]** — [!UICONTROL Now] （当前日期和时间）或 [!UICONTROL The Planned Start Date] ( [!UICONTROL Actual Start Date] 与问题详细信息中设置的开始日期匹配)。
1. 现在，为 **[!UICONTROL Actual Completion Date]** — [!UICONTROL Now] （当前日期和时间）或 [!UICONTROL The Planned Completion Date] ( [!UICONTROL Actual Start Date] 与“问题详细信息”中设置的日期匹配)。
1. 完成后保存。


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 问题访问

的 [!UICONTROL Access] “问题”设置控制在Workfront中为用户分配了问题后，向用户授予的访问权限。 这些设置控制对问题本身的访问，以及对与问题关联的项目的访问。

在更改这些设置之前，请与您的 [!DNL Workfront] 顾问和您的内部治理团队。

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL When someone is assigned to an ISSUE] 突出显示的部分](assets/admin-fund-issue-prefs-access-1.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 的双曲余切值。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Access]** 部分并找到“[!UICONTROL When someone is assigned to an ISSUE]“ ”选项。
1. 为问题本身设置共享访问权限。 [!UICONTROL View], [!UICONTROL Contribute]或 [!UICONTROL Manage]. [!DNL Workfront] 建议按原样保留高级选项。
1. 如果问题受分派人还应有权访问项目，请勾选方框
1. 然后，选择项目的共享访问权限 —  [!UICONTROL View], [!UICONTROL Contribute]或 [!UICONTROL Manage]. 当您设置 [!UICONTROL Advanced Options]，请记住贵组织的工作流和访问需求。
1. 完成后保存。

![[!UICONTROL Access] 窗口显示 [!UICONTROL Contribute] 选项](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
