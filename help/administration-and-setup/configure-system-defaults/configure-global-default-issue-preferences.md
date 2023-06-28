---
title: 配置全局默认问题首选项
description: 了解如何为转换的问题、实际日期和问题访问权限设置问题偏好设置。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 配置全局默认问题偏好设置

一些系统范围的设置为以下情况下问题的行为方式建立了默认值： [!DNL Workfront].

最佳实践是保留全局默认值，并允许项目经理在项目级别或项目模板中进行所需的调整。

全局问题偏好设置可以调整，但建议您 [!DNL Workfront] 顾问讨论组织的工作流、流程和报告需求所需的设置。 您的顾问还可以帮助您了解如果更改某些设置将会发生什么情况。

问题首选项允许系统管理员控制将问题转换为任务或项目时的选项、计算实际日期的方式以及在分配问题时谁获得项目访问权限。 让我们看一下这些设置位于何处 [!DNL Workfront].

## 转换的问题偏好设置

这些设置控制问题转换为中的任务或项目时发生的情况 [!DNL Workfront].

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL Issues] 部分突出显示](assets/admin-fund-issue-prefs-converting.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Issues]** 部分。
1. 单击所需的选项。
1. 完成后保存。

让我们看一下此部分中的选项，以使您可为您的组织选择适当的选项。

* **[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object Changes]**

  此设置允许您将原始问题的解决方案与新对象（任务或项目）的解决方案相关联。

  启用（选中）此设置后，您可以创建状态键与任务或项目状态相同的自定义问题状态。 当任务或项目（可解析对象）设置为自定义状态时，更改也会显示在问题状态上。

  禁用后，解析对象状态将自动设置为默认状态，而不是自定义状态。

  要使此设置生效，请使用“[!UICONTROL Keep the original issue and tie its resolution to the task]必须选择“ ”选项。

* **[!UICONTROL Keep the original issue and tie is resolution to the task/project]**

  当问题得到转化时，这说明 [!DNL Workfront] 保留原来的问题。 问题状态会随着任务或项目状态的改变而改变。 将任务或项目标记为完成后，问题将标记为已解决。

  如果未选中此选项，则原始问题将被删除，并且仅保留已转换的任务或项目。

  此设置会影响有关最初在项目中记录的问题或通过 [!DNL Workfront] 请求队列。

* **[!UICONTROL Allow Primary Contact to have access to the task/project]**

  这允许原始问题创建者访问在转化期间创建的任务或项目。 他们可以审查工作、进行更新并随时了解进度。

* **[!UICONTROL Allow these settings to be changed during conversion]**

  选中此选项时，表示&#39;&#39;的默认设置[!UICONTROL Keep original issue]“ ”和“ ”[!UICONTROL Allow Primary Contact]”可以由转化问题的用户进行更改。 如果希望默认值保持不变，请取消选择此选项。

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 实际日期首选项

整个过程中使用了多种类型的日期 [!DNL Workfront]. 实际日期是一个“时间戳”，它可以 [!DNL Workfront] 在发生特定状态更改时生成。

此 [!UICONTROL Actual Start Date] 当问题状态从新状态更改为其他状态时，将创建时间戳。 此 [!UICONTROL Actual Completion Date] 时间戳是指问题状态更改为指示其已关闭的状态。

需要注意的是，此首选项控制任务和问题的实际日期设置。

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL Actual Dates] 部分突出显示](assets/admin-fund-issue-prefs-actual-dates.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Actual Dates]** 部分。
1. 为选择所需的选项 **[!UICONTROL Actual Start Date]** — [!UICONTROL Now] （当前日期和时间）或 [!UICONTROL The Planned Start Date] (此 [!UICONTROL Actual Start Date] 匹配问题详细信息中设置的开始日期)。
1. 现在，为以下项选择选项 **[!UICONTROL Actual Completion Date]** — [!UICONTROL Now] （当前日期和时间）或 [!UICONTROL The Planned Completion Date] (此 [!UICONTROL Actual Start Date] 匹配问题详细信息中设置的日期)。
1. 完成后保存。


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 问题访问权限

此 [!UICONTROL Access] 问题设置控制当在Workfront中为用户分配问题时授予用户的访问权限。 这些设置控制对问题本身的访问，以及与问题关联的项目的访问。

在更改这些设置之前，请与讨论任何工作流或进程需求 [!DNL Workfront] 顾问和您的内部治理团队。

![[!UICONTROL Tasks & Issues] 首选项窗口 [!UICONTROL When someone is assigned to an ISSUE] 部分突出显示](assets/admin-fund-issue-prefs-access-1.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Tasks & Issues]**.
1. 滚动到 **[!UICONTROL Access]** 部分并查找&quot;[!UICONTROL When someone is assigned to an ISSUE]”选项。
1. 设置问题本身的共享访问权限 —  [!UICONTROL View]， [!UICONTROL Contribute]，或 [!UICONTROL Manage]. [!DNL Workfront] 建议保留高级选项不变。
1. 如果问题被分派人还应具有项目的访问权限，请选中方框
1. 然后选择项目的共享访问权限 —  [!UICONTROL View]， [!UICONTROL Contribute]，或 [!UICONTROL Manage]. 当您设置 [!UICONTROL Advanced Options]，请牢记您组织的工作流和访问需求。
1. 完成后保存。

![[!UICONTROL Access] 窗口显示 [!UICONTROL Contribute] options](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
