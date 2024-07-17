---
title: 验证报告
description: 了解如何使用报告功能来管理验证进度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 100%

---

# 验证报告

[!DNL Workfront] 的数字验证功能使您可以在一个地方（在 [!DNL Workfront] 中）管理项目和相关的审查工作流。通过报告类型、字段源以及显示审查和审批信息的字段名称，获得有关正在进行的验证工作的宝贵见解。

我们建议您与 [!DNL Workfront] 顾问合作，创建符合组织要求的报告。生成某些报告需要熟悉 [!DNL Workfront] 的文本模式报告。

从这些基本的标准报告开始，帮助您的团队在 [!DNL Workfront] 中管理正在进行审查和审批流程的验证。

## [!UICONTROL Proof Approval]

此报告类型可以帮助您跟踪未完成的验证审批，以确保按时完成。

![从 [!UICONTROL New Report] 下拉菜单选择 [!UICONTROL Proof Approval]](assets/proof-system-setups-proof-approval-report.png)

视图和过滤选项包括 [!UICONTROL decision date]、[!UICONTROL proof approval]、[!UICONTROL approver stage]、[!UICONTROL workflow template] 和 [!UICONTROL requester information]。通过文本模式报告功能，您可以创建按文档名称组织列表的分组。请参阅[了解分组的基本文本模式。](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=zh-Hans)

编写验证审批报告时，请确保您获得的是与最新版本的验证相关的信息。[!DNL Workfront] 建议在过滤器中包含此字段源和字段名称：

**[!UICONTROL Proof Approval]>>[!UICONTROL Is Current Document Version]**

![Report Builder 中的“过滤器”选项卡](assets/proof-system-setups-proof-approval-report-is-current-version.png)

当您报告具有多个版本的验证时，这非常有用，此时报告仅会列出每个需要审批的验证的当前版本。这会过滤掉您不再需要处理的早期版本。

## [!UICONTROL Document Version]

这种报告类型允许您管理和跟踪 [!DNL Workfront] 中的版本。

![从 [!UICONTROL New Report] 下拉菜单选择 [!UICONTROL Document Version]](assets/proof-system-setups-document-version-report.png)

视图选项包括 [!UICONTROL document version]、[!UICONTROL document]、[!UICONTROL entered by]、[!UICONTROL proof approval status]、[!UICONTROL proof creator] 和 [!UICONTROL document provider] 中的信息。

分组可以通过 [!UICONTROL document version]、[!UICONTROL entered by]、[!UICONTROL proof approval status] 或验证所有者信息来完成。

过滤器包括 [!UICONTROL document version]、[!UICONTROL access level]、[!UICONTROL document]、[!UICONTROL entered by]、[!UICONTROL proof approval status]、[!UICONTROL proof creator] 以及文档提供者信息。

您可以使用视图中的此列显示报告上每个文档当前处于活动状态的验证阶段的名称：

**[!UICONTROL Document Versions]>>[!UICONTROL Active Proof Stages]**

![Report Builder 中的“过滤器”选项卡](assets/proof-system-setups-active-proof-stages.png)

如果当前没有处于活动状态的阶段，则该列为空。

此字段源 >> 字段名称也可用作报告中的过滤器。

使用 [!UICONTROL Proof Creator] 字段源来报告有关创建验证的用户信息。选择 [!UICONTROL Name] 字段源，以在视图中显示验证创建者的名称。

**[!UICONTROL Proof Creator]>>[!UICONTROL Name]**

此字段源 >> 字段名称组合也可用作过滤器。

![Report Builder 中的“过滤器”选项卡](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
