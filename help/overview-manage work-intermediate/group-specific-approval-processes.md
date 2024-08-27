---
title: 了解特定于组的审批流程
description: 了解组管理员如何为其管理的组创建或编辑审批流程。
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
hide: true
source-git-commit: 5362e8a60d39e61021bb9ab22e3d9afffd41f96a
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 100%

---

# 了解特定于组的审批流程

系统管理员和组管理员都可以在 [!DNL Workfront] 中创建审批流程。系统管理员可以创建用于整个 [!DNL Workfront] 系统或仅用于特定组的流程。组管理员只能为他们管理的组创建或编辑流程。

对于 [!DNL Workfront] 中每个人都可以使用的审批流程，请确保 [!UICONTROL "This approval process can be used by"] 字段设置为 [!UICONTROL All groups]。

![[!UICONTROL Edit Approval Process] 窗口，其中组字段突出显示](assets/admin-fund-approval-processes-1.png)

[!UICONTROL "Start Approval Process when the status is set to"] 菜单中可用的状态取决于“使用者”字段中的选择。选择 [!UICONTROL All groups] 后，仅系统范围内的锁定状态可用。

要限制特定组的审批流程，请从 [!UICONTROL "This approval process can be used by"] 字段的列表中选择该组的名称。

![[!UICONTROL Edit Approval Process] 窗口，其中组字段已展开](assets/admin-fund-approval-processes-2.png)

[!UICONTROL All groups] 选项不适用于组管理员。

选择特定组时，只有该组的可用状态会显示在 [!UICONTROL "Start Approval Process when the status is set to"] 菜单中。

![[!UICONTROL Edit Approval Process] 窗口，其中状态字段已突出显示](assets/admin-fund-approval-processes-3.png)

