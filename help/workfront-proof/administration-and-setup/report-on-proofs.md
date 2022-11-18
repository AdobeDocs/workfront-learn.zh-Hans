---
title: 校样报告
description: 了解如何使用报告功能管理校样进度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# 校样报告

[!DNL Workfront]通过的数字校对功能，您可以在一个位置管理项目和相关的审阅工作流程。 [!DNL Workfront]. 深入了解正在对显示审阅和批准信息的报表类型、字段来源和字段名称执行的校对工作。

我们建议您与 [!DNL Workfront] 顾问创建符合贵组织要求的报表。 有些报表需要熟悉 [!DNL Workfront]的文本模式报告。

从这些基本的标准报表开始，帮助您的团队管理通过 [!DNL Workfront].

## [!UICONTROL Proof Approval]

此报表类型可帮助您跟踪未完成的校样批准，以确保满足截止日期。

![选择 [!UICONTROL Proof Approval] 从 [!UICONTROL New Report] 下拉菜单](assets/proof-system-setups-proof-approval-report.png)

查看和过滤选项包括 [!UICONTROL decision date], [!UICONTROL proof approval], [!UICONTROL approver stage], [!UICONTROL workflow template]和 [!UICONTROL requester information]. 通过文本模式报告，您可以创建按文档名称组织列表的分组。

在编写校样批准报告时，请确保您获得了与校样的最新版本相关的信息。 [!DNL Workfront] 建议在筛选器中包含此字段源和字段名称：

**[!UICONTROL Proof Approval]>>[!UICONTROL Is Current Document Version]**

![报表生成器中的“过滤器”选项卡](assets/proof-system-setups-proof-approval-report-is-current-version.png)

当您报告的校样具有多个版本时，这非常有用，因为报表仅列出了每个需要批准的校样的当前版本。 这会过滤掉您不再需要处理的早期版本。

## [!UICONTROL Document Version]

此报表类型允许您在 [!DNL Workfront].

![选择 [!UICONTROL Document Version] 从 [!UICONTROL New Report] 下拉菜单](assets/proof-system-setups-document-version-report.png)

查看选项包括 [!UICONTROL document version], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator]和 [!UICONTROL document provider].

分组可由 [!UICONTROL document version], [!UICONTROL entered by], [!UICONTROL proof approval status]，或校样所有者信息。

过滤器包括 [!UICONTROL document version], [!UICONTROL access level], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator]、和文档提供程序信息。

您可以在视图中显示针对报表中具有此列的每个文档当前处于活动状态的校对阶段的名称：

**[!UICONTROL Document Versions]>>[!UICONTROL Active Proof Stages]**

![报表生成器中的“过滤器”选项卡](assets/proof-system-setups-active-proof-stages.png)

如果当前没有活动阶段，则列为空。

此字段源>>字段名称也可用作报表中的过滤器。

使用 [!UICONTROL Proof Creator] 字段源来报告有关创建校样的用户的信息。 选择 [!UICONTROL Name] 字段源来显示视图中校样创建者的名称。

**[!UICONTROL Proof Creator]>>[!UICONTROL Name]**

此字段源>>字段名称组合也可用作过滤器。

![报表生成器中的“过滤器”选项卡](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
