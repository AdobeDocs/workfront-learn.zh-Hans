---
title: 跟踪校对进度
description: 了解如何使用 [!UICONTROL SOCD] 用于跟踪中验证进度的指示器、验证进度和报告 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 跟踪校对进度

作为审阅和批准流程中的项目经理、验证经理或其他利益相关者，您将需要跟踪验证的进度。 你可以使用执行此操作 [!DNL Workfront’s] 内置 **验证进度指示器** 在 [!UICONTROL Documents] 页面或编写自定义报告。

查看验证进度 [!DNL Workfront]，您必须拥有计划、工作或审阅许可证，并且是验证用户。 如果你不确定 [!DNL Workfront] 配置文件符合这些要求，请联系您组织的验证系统管理员。

## 跟踪验证进度 [!UICONTROL SOCD] 指标和验证状态

使用全面了解验证如何完成审阅和批准流程 [!UICONTROL SOCD] 中的图标 [!UICONTROL Documents] 列表。 这些图标指示对验证执行的特定操作。

![的图像 [!UICONTROL Documents] 列出于 [!DNL  Workfront] 使用的项目 [!UICONTROL SOCD] 高亮显示的图标。](assets/manage-proofs-socd.png)

这些图标指示从您向收件人发送验证到他们对验证做出决策期间对验证完成的工作。

* **S —** 校样已发送给收件人。
* **O —** 证明已打开。
* **C —** 对证明进行了评论。
* **D —** 已对证明做出决定（批准、拒绝等）。

这些颜色指示操作是否完成。

* **白色 —** 该步骤尚未发生。
* **绿色 —** 步骤已完成。
* **橙色 —** 验证截止日期在24小时内，并且该步骤尚未发生。
* **红色 —** 验证截止日期已过，尚未执行步骤。

此 [!UICONTROL SOCD] 在 [!UICONTROL Documents] 列表、摘要面板中或 [!UICONTROL Document Details]是验证进度的高级摘要。 [!DNL Workfront] 根据在验证过程中“落后”最多的收件人配置此项。

例如，如果有三名审阅人/批准人，且只有两名审阅人/批准人查看了验证并发表了评论，则 [!UICONTROL SOCD] 图标将显示校样已发送([!UICONTROL S])并打开([!UICONTROL O])，但未发表评论([!UICONTROL C])。

如果您想知道每个验证收件人的表现，请打开验证工作流。 总体验证进度位于窗口顶部。 灰色条中的每个阶段都有各自的进度指示器。  每个用户旁边都显示该个人的进度。

![的图像 [!UICONTROL Proofing Workflow] 部分。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校对状态

验证状态基于阶段的验证收件人的状态。 总体验证状态在 [!UICONTROL Documents] 页面，右侧 [!UICONTROL SOCD] 指示器，以便您轻松判断您是否对验证做出了决定。

![的图像 [!UICONTROL Documents] 列出于 [!DNL  Workfront] 突出显示整体验证状态的项目。](assets/manage-proofs-overall-status.png)

此校对状态指示校对的整体状态。 例如，如果两个收件人批准验证，则其个人状态将显示 [!UICONTROL Approved]. 但是，第三个收件人尚未做出决定，因此该人的状态为 [!UICONTROL Pending]. 因此，总体状态显示为 [!UICONTROL Pending].

如果为贵组织配置了自定义状态，则将使用这些状态。 否则，您将看到以下标准状态选项：

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

打开验证工作流窗口，以查看分配了以下内容的收件人的验证状态： [!UICONTROL Reviewer & Approver] 或 [!UICONTROL Approver]校对角色。

## 报告位置 [!DNL Workfront]

您还可以利用 [!DNL Workfront’s] 报告功能，用于在验证通过审阅和批准流程时对其进行跟踪。

验证审批报告可帮助您跟踪未完成的审批，以确保遵守截止日期。

![中的验证审批报告图像 [!DNL  Workfront].](assets/proof-approval-report.png)

文档版本报告允许您管理和跟踪校样版本。

![中文档版本报表的图像 [!DNL  Workfront].](assets/document-version-report.png)

我们建议您与您的 [!DNL Workfront] 顾问创建满足您组织要求的报表。 部分报告需要熟悉 [!DNL Workfront’s] 文本模式报表。

## 轮到你了

与您的团队或验证系统管理员联系，了解您将在Workfront中使用哪种类型的报告，以保持验证工作流顺利运行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
