---
title: 自定义系统范围的问题状态
description: 了解如何更改问题状态名称、控制状态用于的问题类型，以及锁定/解锁状态以进行组级别自定义。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 自定义系统范围的状态

[!DNL Workfront] 提供了各种默认状态，以适应贵组织的问题管理工作流。 可以重命名这些状态以匹配贵组织的术语。 可以将状态分配给特定的问题类型。

如果需要，可以创建其他状态。 只有系统管理员才能创建系统范围的状态。 此外，系统管理员还控制组管理员可以编辑哪些状态。

![[!UICONTROL Issues] 选项卡 [!UICONTROL Statues] 页面 [!UICONTROL Setup]](assets/admin-fund-all-issue-statuses.png)

## 修改现有状态

[!DNL Workfront] 建议设置最少的状态数。 这样，为用户选择正确的状态会更加容易，并且会导致要维护的状态列表缩短。

您可以编辑现有状态以更改名称、分配给的问题类型、相关颜色等。

![问题状态列表 [!UICONTROL Edit] 高亮显示选项](assets/admin-fund-edit-issue-status.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 的双曲余切值。
1. 选择 **[!UICONTROL Statuses]**.
1. 选择 **[!UICONTROL Issues]** 选项卡，确保 [!UICONTROL System Statuses] 显示。
1. 选择 **[!UICONTROL Master List]** 查看所有问题类型的状态。 您可以在此处创建或修改问题状态。
1. 将鼠标悬停在要重命名的状态的右侧，然后单击 **[!UICONTROL Edit]**.
1. 根据需要为状态指定新名称或更改任何其他信息。
1. 如果这些设置应用于 [!DNL Workfront] 实例。
1. 解锁状态，以允许组管理员仅编辑其组的状态。
1. 选中状态应用于的问题类型对应的复选框。
1. 单击 **[!UICONTROL Save]**.

![用于创建新状态的窗口](assets/admin-fund-edit-issue-status-2.png)

### 状态分配

并非所有状态都可以分配给所有问题类型。 的 [!UICONTROL Statuses] 页面的列显示了每个状态可用于的问题类型。

![“状态”页面的“问题”选项卡上突出显示的更改顺序](assets/admin-fund-issue-type-statuses.png)


要仅查看分配给特定问题类型的状态，只需单击窗口顶部的问题类型名称。

![[!UICONTROL Issue] 选项卡 [!UICONTROL Status] 突出显示列的页面](assets/admin-fund-statuses-issue-type.png)

从此处，您可以将问题拖放到您希望它们在 [!UICONTROL Status] 下拉菜单。

要编辑状态，您需要返回到 [!UICONTROL Master List].
