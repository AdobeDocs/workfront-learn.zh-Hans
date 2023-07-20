---
title: 了解特定于组的批准流程
description: 了解组管理员如何为其管理的组创建或编辑批准流程。
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 了解特定于组的批准流程

系统和组管理员均可以在以下位置创建批准流程： [!DNL Workfront]. 系统管理员可以创建流程以在整个 [!DNL Workfront] 系统或仅用于特定组的系统。 组管理员只能为其管理的组创建或编辑进程。

对于可由以下位置中的每个人使用的审批流程： [!DNL Workfront]，确保 [!UICONTROL "This approval process can be used by"] 字段设置为 [!UICONTROL All groups].

![[!UICONTROL Edit Approval Process] 突出显示组字段的窗口](assets/admin-fund-approval-processes-1.png)

中可用的状态 [!UICONTROL "Start Approval Process when the status is set to"] 菜单取决于“使用者”字段中的选择。 替换为 [!UICONTROL All groups] 选中，则只有系统范围的锁定状态可用。

要限制特定组的审批流程，请从的列表中选择该组的名称 [!UICONTROL "This approval process can be used by"] 字段。

![[!UICONTROL Edit Approval Process] 展开组字段的窗口](assets/admin-fund-approval-processes-2.png)

此 [!UICONTROL All groups] 选项对组管理员不可用。

选择特定组后，只有该组的可用状态会显示在 [!UICONTROL "Start Approval Process when the status is set to"] 菜单。

![[!UICONTROL Edit Approval Process] 突出显示状态字段的窗口](assets/admin-fund-approval-processes-3.png)

