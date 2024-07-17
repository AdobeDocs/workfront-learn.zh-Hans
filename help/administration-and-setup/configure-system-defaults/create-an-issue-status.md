---
title: 创建问题状态
description: 了解如何创建问题状态，以满足组织工作流的需求。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 100%

---

# 创建问题状态

[!DNL Workfront] 建议您在开始创建新状态之前修改系统中现有的问题状态。这有助于限制需要维护的状态数量。

1. 单击 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单面板中的 **[!UICONTROL Project Preferences]** 部分。
1. 选择 **[!UICONTROL Statuses]**。
1. 选择 **[!UICONTROL Issues]** 选项卡。
1. 确保右上角的字段设置为 [!UICONTROL System Statuses]。这样可以确保新状态在整个 [!DNL Workfront] 实例中全局可用。
1. 选择 **[!UICONTROL Master List]**，以查看所有问题状态。您可以在此处创建或修改状态。
1. 单击 **[!UICONTROL Add a New Status]**。
1. 根据您的组织需要填写相关字段——名称、描述、颜色、等同项、键等。
1. 选中此状态可用于的问题类型的复选框。
1. 单击 **[!UICONTROL Save]**。

![[!UICONTROL Statuses] 页面上的新状态窗口](assets/admin-fund-create-issue-status.png)

## 问题状态和组管理员

组管理员可以为其管理的组创建问题状态，并对其进行自定义。这为他们的组提供了一定的自主权，使他们具备确保工作顺利进行所需的状态。它还消除了对一长串系统范围状态的需要。

如果系统管理员已将组管理员配置为允许自定义，则组管理员可以编辑现有状态。

系统管理员可以通过选择 [!UICONTROL Statuses] 窗口右上角的组名称来管理组的状态。

![[!UICONTROL Statuses] 页面上的组列表菜单](assets/admin-fund-change-group-master-list.png)

组管理员可以单击 [!UICONTROL Setup] 区域中的 [!UICONTROL Groups] 部分，通过单击相关名称打开他们的组，然后在左侧面板菜单中选择 [!UICONTROL Statuses]。请务必选择“问题”选项卡。

![[!UICONTROL Statuses] 部分，在 [!UICONTROL Group] 页面中](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
