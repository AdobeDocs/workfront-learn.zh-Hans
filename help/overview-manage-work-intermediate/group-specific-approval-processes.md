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
exl-id: 9986469c-b02f-48ac-b71e-055473a2855b
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:17:51.764Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 167
ht-degree: 100%

---

# 了解特定于组的审批流程

系统管理员和组管理员都可以在 [!DNL Workfront] 中创建审批流程。 系统管理员可以创建用于整个 [!DNL Workfront] 系统或仅用于特定组的流程。 组管理员只能为他们管理的组创建或编辑流程。

对于 [!DNL Workfront] 中每个人都可以使用的审批流程，请确保 [!UICONTROL "This approval process can be used by"] 字段设置为 [!UICONTROL All groups]。

![[!UICONTROL Edit Approval Process] 窗口，其中组字段突出显示](assets/admin-fund-approval-processes-1.png)

[!UICONTROL "Start Approval Process when the status is set to"] 菜单中可用的状态取决于“使用者”字段中的选择。 选择 [!UICONTROL All groups] 后，仅系统范围内的锁定状态可用。

要限制特定组的审批流程，请从 [!UICONTROL "This approval process can be used by"] 字段的列表中选择该组的名称。

![[!UICONTROL Edit Approval Process] 窗口，其中组字段已展开](assets/admin-fund-approval-processes-2.png)

[!UICONTROL All groups] 选项不适用于组管理员。

选择特定组时，只有该组的可用状态会显示在 [!UICONTROL "Start Approval Process when the status is set to"] 菜单中。

![[!UICONTROL Edit Approval Process] 窗口，其中状态字段已突出显示](assets/admin-fund-approval-processes-3.png)
