---
title: 配置全局默认项目设置
description: 了解如何更改自定义状态、设置全局项目首选项以及创建全局默认设置的计划。
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
jira: KT-8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 100%

---

# 配置全局默认项目设置

<!--
21.4 updates have been made
-->

在本视频中，您将学习如何：

* 更改自定义状态
* 设置全局项目首选项
* 创建和使用计划

>[!VIDEO](https://video.tv.adobe.com/v/3423345/?quality=12&learn=on&enablevpops&captions=chi_hans)

## 全局和组项目、任务和问题设置

当您在 [!DNL Workfront] 中打开 [!UICONTROL Projects] 设置时，您会注意到窗口顶部的搜索栏中会显示“[!UICONTROL System Project Preferences]”。这是为了让您知道这些设置会影响 [!DNL Workfront] 系统中的每个人——这是一个全局配置。

![[!UICONTROL Project Preferences] 页面，位于 [!UICONTROL Setup]](assets/admin-fund-system-project-preferences-1.png)

当您打开 [!UICONTROL Tasks & Issues] 设置时，您会看到类似的内容。

![[!UICONTROL Task & Issue Preferences]，位于 [!UICONTROL Setup]](assets/admin-fund-task-issue-preferences-2.png)

然而，可能并非 [!DNL Workfront] 中的每个组都需要相同的项目、任务和问题首选项。例如，营销团队希望新项目的状态为“规划中”，而项目经理团队更喜欢“请求”状态。

[!DNL Workfront] 允许组管理员调整其组的某些项目、任务和问题首选项。可调整的首选项由 [!DNL Workfront] 系统管理员使用锁定/解锁切换开关确定。

首先导航到 [!UICONTROL Setup] 区域：

1. 选择 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单中的 **[!UICONTROL Project Preferences]**。
1. 选择 **[!UICONTROL Projects]** 或 **[!UICONTROL Tasks & Issues]**，具体取决于您要修改的设置。

锁定首选项以防止组管理员为其组调整该设置。

![锁定的首选项消息](assets/admin-fund-preferences-locked-3.png)

解锁首选项以供组管理员进行自定义。

![未锁定的首选项消息](assets/admin-fund-preferences-unlocked-4.png)

某些设置无法解锁并保留全局系统设置。

![锁定的首选项消息](assets/admin-fund-preferences-always-locked-5.png)

### 设置组和子组首选项

对于系统管理员解锁的任何设置，组管理员可以对其管理的组以及嵌套在这些组下的任何子组进行调整。此外，组管理员可以控制其子组管理员可以修改哪些设置。

1. 选择 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 单击左侧菜单中的 **[!DNL Groups]**。
1. 单击组或子组名称将其打开。
1. 选择左侧菜单中的 **[!UICONTROL Project Preferences]** 或 **[!UICONTROL Tasks & Issues Preferences]**。
1. 对每个已解锁的首选项进行所需的更改。
1. 选择 **[!UICONTROL Save]**。

![[!UICONTROL Project Status] 部分，在 [!UICONTROL Group] 页面上](assets/admin-fund-group-preferences.png)

如果您的组织没有使用组管理员，系统管理员可以管理不同组的首选项设置。

<!--
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
-->
