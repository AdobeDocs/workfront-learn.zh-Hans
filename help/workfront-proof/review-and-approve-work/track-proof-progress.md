---
title: 跟踪验证进度
description: 了解如何使用 [!UICONTROL SOCD] 指标、验证进度和报告来跟踪  [!DNL  Workfront] 中的验证进度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 63%

---

# 跟踪验证进度

作为审阅和批准流程中的项目经理、验证经理或其他利益相关者，您将需要跟踪验证的进度。 您可以使用 [!UICONTROL Documents] 页面上的 [!DNL Workfront's] 内置&#x200B;**验证进度指示器**&#x200B;或通过编写自定义报告来进行跟踪。

要在 [!DNL Workfront] 中查看验证进度，您必须拥有计划、工作或审查许可证，并且是验证用户。如果您不确定您的[!DNL Workfront]配置文件是否满足这些要求，请与组织的验证系统管理员联系。

## 使用 [!UICONTROL SOCD] 指示器和验证状态跟踪验证进度

使用 [!UICONTROL SOCD] 列表中的 [!UICONTROL Documents] 图标，从高层角度了解验证在审查和审批过程中的进展情况。这些图标表示对验证采取的具体操作。

![[!DNL  Workfront] 项目中 [!UICONTROL Documents] 列表的图像，其中突出显示 [!UICONTROL SOCD] 图标。](assets/manage-proofs-socd.png)

图标表示从您将验证发送给收件人到他们对验证作出决策为止，在该验证上所做的工作。

* **S—**&#x200B;验证已发送给收件人。
* **O—**&#x200B;验证已经打开。
* **C —**&#x200B;已对验证进行了评论。
* **D —**&#x200B;已对验证作出决策（审批、拒绝等）。

颜色指示操作是否完成。

* **白色 —**&#x200B;步骤尚未发生。
* **绿色—**&#x200B;该步骤已完成。
* **橙色 —**&#x200B;验证截止日期在24小时内，尚未执行此步骤。
* **红色 —**&#x200B;证明截止日期已过，尚未执行步骤。

[!UICONTROL Documents]列表、摘要面板或[!UICONTROL Document Details]中的[!UICONTROL SOCD]是验证进度的高级摘要。 [!DNL Workfront]根据验证过程中“最落后”的收件人配置此项。

例如，如果有三名审核人/审批人，其中只有两人查看了该验证并发表了评论，则 [!UICONTROL SOCD] 图标将会显示该验证已发送 ([!UICONTROL S]) 并且已打开 ([!UICONTROL O])，但没有发表评论 ([!UICONTROL C])。

**在对验证做出最终决定**（例如，批准或拒绝）后，该阶段的用户可能会看到所有SOCD指示器呈绿色，即使未执行单个操作（例如打开验证或发表评论）也是如此。 这是一种全系统行为，旨在反映总体阶段完成情况，而非个人参与情况。

**在注册决策之前**，每个SOCD指示器都反映了实际的用户活动（例如，如果未执行任何操作，则为白色；如果操作已完成，则为绿色）。 做出决定后，系统假定工作流已完成，并相应地更新所有指标。

如果您想了解每个验证收件人的工作情况，请打开验证工作流。总体验证进度位于窗口顶部。每个阶段在灰色栏中都有自己的进度指示器。在每个用户旁边就是该个人的进步。

![文档的 [!UICONTROL Proofing Workflow] 部分的图像。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 验证状态

验证状态基于阶段的验证收件人的状态。 在 [!UICONTROL Documents] 页面上的 [!UICONTROL SOCD] 指示器的右侧会显示整体验证状态，以便您可以轻松地判断自己是否已对该验证作出决策。

![[!DNL  Workfront] 项目中 [!UICONTROL Documents] 列表的图像，其中突出显示了总体验证状态。](assets/manage-proofs-overall-status.png)

此验证状态表示验证的总体状态。例如，如果两个收件人审批了该验证，则他们的个人状态将会显示 [!UICONTROL Approved]。但是，第三个收件人尚未做出决定，因此该人员的状态为[!UICONTROL Pending]。 因此，总体状态显示为 [!UICONTROL Pending]。

如果您的组织配置有自定义状态，则会使用这些状态。否则，您将看到以下标准状态选项：

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

打开验证工作流窗口，查看分配有 [!UICONTROL Reviewer & Approver] 或 [!UICONTROL Approver] 验证角色的收件人的验证状态。

## [!DNL Workfront] 中的报告

您还可以利用 [!DNL Workfront's] 报告功能来跟踪验证在审查和审批过程中的进展。

验证审批报告可帮助您跟踪未完成的审批事项，以确保在截止日期前完成。

![[!DNL  Workfront] 中的验证审批报告的图像。](assets/proof-approval-report.png)

您可以使用文档版本管理和跟踪验证版本。

![[!DNL  Workfront] 中文档版本报告的图像。](assets/document-version-report.png)

我们建议您与 [!DNL Workfront] 顾问合作，创建符合组织要求的报告。生成某些报告需要熟悉 [!DNL Workfront's] 的文本模式报告。

## 到您了

与您的团队或验证系统管理员联系，了解您将在Workfront中使用哪种类型的报告，以使验证工作流平稳运行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
