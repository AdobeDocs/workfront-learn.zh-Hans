---
title: 创建问题状态
description: 了解如何创建问题状态以满足组织工作流的需求。
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
ht-degree: 1%

---

# 创建问题状态

[!DNL Workfront] 建议先修改系统中的现有问题状态，然后再开始创建新状态。 这有助于限制需要维护的状态数量。

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Statuses]**.
1. 选择 **[!UICONTROL Issues]** 选项卡。
1. 确保将右上角的字段设置为 [!UICONTROL System Statuses]. 这可确保新状态可在您的全局范围内使用 [!DNL Workfront] 实例。
1. 选择 **[!UICONTROL Master List]** 以查看所有问题状态。 您可以在此处创建或修改状态。
1. 单击 **[!UICONTROL Add a New Status]**.
1. 根据您的组织需要填写字段 — 名称、描述、颜色、等于、键等。
1. 选中可与此状态一起使用的问题类型的复选框。
1. 单击 **[!UICONTROL Save]**.

![新状态窗口打开 [!UICONTROL Statuses] 页面](assets/admin-fund-create-issue-status.png)

## 问题状态和组管理员

组管理员可以为他们管理的组创建和自定义问题状态。 这为他们的团队提供了一些自主权，为他们提供了保持工作运转所需的状态。 它还可消除系统范围状态清单冗长的需要。

如果系统管理员将现有状态配置为允许自定义，则组管理员可以编辑现有状态。

系统管理员可以通过选择位于的右上角的组名称来管理组的状态。 [!UICONTROL Statuses] 窗口。

![上的组列表菜单 [!UICONTROL Statuses] 页面](assets/admin-fund-change-group-master-list.png)

组管理员可以单击 [!UICONTROL Groups] 中的部分 [!UICONTROL Setup] 区域，通过单击名称打开其组，然后选择 [!UICONTROL Statuses] （在左侧面板菜单中）。 确保选择问题选项卡。

![[!UICONTROL Statuses] 部分 [!UICONTROL Group] 页面](assets/admin-fund-group-issue-statuses.png)

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
