---
title: 自定义系统范围问题状态
description: 了解如何更改问题状态名称、控制使用状态的问题类型以及锁定/解锁组级别自定义的状态。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 自定义系统范围状态

[!DNL Workfront] 提供了多种默认状态，以适应贵组织的问题管理工作流。 这些状态可以重命名以匹配贵组织的术语。 可以将和状态分配给特定问题类型。

如果需要，可以创建其他状态。 只有系统管理员可以创建系统范围的状态。 此外，系统管理员控制组管理员可以编辑哪些状态。

![[!UICONTROL Issues] 选项卡 [!UICONTROL Statues] 页面位置 [!UICONTROL Setup]](assets/admin-fund-all-issue-statuses.png)

## 修改现有状态

[!DNL Workfront] 建议使用最小状态数。 这使得用户能够更轻松地选择正确的状态，并导致需要维护的状态列表更短。

您可以编辑现有状态以更改名称、为其分配的问题类型、相关颜色等。

![问题状态列表，具有 [!UICONTROL Edit] 高亮显示的选项](assets/admin-fund-edit-issue-status.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Statuses]**.
1. 选择 **[!UICONTROL Issues]** 按Tab键并确保 [!UICONTROL System Statuses] 显示在右上角。
1. 选择 **[!UICONTROL Master List]** 查看所有问题类型的状态。 您可以在此处创建或修改问题状态。
1. 将鼠标悬停在要重命名的状态右侧，然后单击 **[!UICONTROL Edit]**.
1. 根据需要，为状态提供一个新名称或更改任何其他信息。
1. 如果这些设置应该应用于中的所有用户，则锁定状态。 [!DNL Workfront] 实例。
1. 解锁状态以允许组管理员仅编辑其组的状态。
1. 选中状态应用于的问题类型对应的框。
1. 单击 **[!UICONTROL Save]**.

![用于创建新状态的窗口](assets/admin-fund-edit-issue-status-2.png)

### 状态分配

并非所有状态都可以分配给所有问题类型。 此 [!UICONTROL Statuses] 页面有列，显示每种状态可用于的问题类型。

![在“状态”页面的“问题”选项卡上突出显示的更改顺序](assets/admin-fund-issue-type-statuses.png)


要仅查看分配给特定问题类型的状态，只需单击窗口顶部的问题类型名称。

![[!UICONTROL Issue] 选项卡/ [!UICONTROL Status] 突出显示列的页面](assets/admin-fund-statuses-issue-type.png)

从这里，您可以将问题拖放到您希望它们在中显示的顺序中 [!UICONTROL Status] 下拉菜单。

要编辑状态，您需要返回到 [!UICONTROL Master List].
