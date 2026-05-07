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
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
TQID: https://experienceleague.adobe.com/PcQL0NTo4cz4jEOXcQ-48tXu8Zr5U-BsbAx9hKn20Tk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
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

