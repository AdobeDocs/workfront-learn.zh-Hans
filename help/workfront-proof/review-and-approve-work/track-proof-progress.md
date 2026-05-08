---
title: 跟踪校样进度
description: 了解如何使用 [!UICONTROL SOCD] 指标、校样进度和报告来跟踪  [!DNL &#x200B; Workfront] 中的校样进度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T19:53:35.724Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 736
ht-degree: 63%

---

# 跟踪校样进度

作为审阅和批准流程中的项目经理、验证经理或其他利益相关者，您将需要跟踪验证的进度。 您可以使用 [!UICONTROL Documents] 页面上的 [!DNL Workfront's] 内置&#x200B;**校样进度指示器**&#x200B;或通过编写自定义报告来进行跟踪。

要在 [!DNL Workfront] 中审阅校对进度，您必须拥有计划、工作或审阅许可证，并且是校对用户。 如果您不确定您的[!DNL Workfront]配置文件是否满足这些要求，请与组织的验证系统管理员联系。

## 使用 [!UICONTROL SOCD] 指示器和校样状态跟踪校样进度

使用 [!UICONTROL SOCD] 列表中的 [!UICONTROL Documents] 图标，从高层角度了解校对在审阅和审批过程中的进展情况。 这些图标表示对校样采取的具体操作。

![[!DNL &#x200B; Workfront] 项目中 [!UICONTROL Documents] 列表的图像，其中突出显示 [!UICONTROL SOCD] 图标。](assets/manage-proofs-socd.png)

图标表示从您将校样发送给收件人到他们对校样作出决策为止，在该校样上所做的工作。

* **S—**&#x200B;校样已发送给收件人。
* **O—**&#x200B;校样已经打开。
* **C —**&#x200B;已对校样进行了评论。
* **D —**&#x200B;已对校样作出决策（审批、拒绝等）。

颜色指示操作是否完成。

* **白色 —**&#x200B;步骤尚未发生。
* **绿色—**&#x200B;该步骤已完成。
* **橙色 —**&#x200B;验证截止日期在24小时内，尚未执行此步骤。
* **红色 —**&#x200B;证明截止日期已过，尚未执行步骤。

[!UICONTROL Documents]列表、摘要面板或[!UICONTROL Document Details]中的[!UICONTROL SOCD]是验证进度的高级摘要。 [!DNL Workfront]根据验证过程中“最落后”的收件人配置此项。

例如，如果有三名审阅者/审批者，其中只有两人查看了该校对并发表了评论，则 [!UICONTROL SOCD] 图标将会显示该校对已发送 ([!UICONTROL S]) 并且已打开 ([!UICONTROL O])，但没有发表评论 ([!UICONTROL C])。

**在对验证做出最终决定**（例如，批准或拒绝）后，该阶段的用户可能会看到所有SOCD指示器呈绿色，即使未执行单个操作（例如打开验证或发表评论）也是如此。 这是一种全系统行为，旨在反映总体阶段完成情况，而非个人参与情况。

**在注册决策之前**，每个SOCD指示器都反映了实际的用户活动（例如，如果未执行任何操作，则为白色；如果操作已完成，则为绿色）。 做出决定后，系统假定工作流已完成，并相应地更新所有指标。

如果您想了解每个校对收件人的工作情况，请打开校对工作流。 总体校样进度位于窗口顶部。 每个阶段在灰色栏中都有自己的进度指示器。  在每个用户旁边就是该个人的进步。

![文档的 [!UICONTROL Proofing Workflow] 部分的图像。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校样状态

验证状态基于阶段的验证收件人的状态。 在 [!UICONTROL Documents] 页面上的 [!UICONTROL SOCD] 指示器的右侧会显示整体校样状态，以便您可以轻松地判断自己是否已对该校样作出决策。

![[!DNL &#x200B; Workfront] 项目中 [!UICONTROL Documents] 列表的图像，其中突出显示了总体校样状态。](assets/manage-proofs-overall-status.png)

此校样状态表示校样的总体状态。 例如，如果两个收件人审批了该校样，则他们的个人状态将会显示 [!UICONTROL Approved]。 但是，第三个收件人尚未做出决定，因此该人员的状态为[!UICONTROL Pending]。 因此，总体状态显示为 [!UICONTROL Pending]。

如果您的组织配置有自定义状态，则会使用这些状态。 否则，您将看到以下标准状态选项：

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

打开校对工作流窗口，查看分配有 [!UICONTROL Reviewer & Approver] 或 [!UICONTROL Approver] 校对角色的收件人的校对状态。

## [!DNL Workfront] 中的报告

您还可以利用 [!DNL Workfront's] 报告功能来跟踪校对在审阅和审批过程中的进展。

校样审批报告可帮助您跟踪未完成的审批事项，以确保在截止日期前完成。

![[!DNL &#x200B; Workfront] 中的校样审批报告的图像。](assets/proof-approval-report.png)

您可以使用文档版本管理和跟踪校样版本。

![[!DNL &#x200B; Workfront] 中文档版本报告的图像。](assets/document-version-report.png)

我们建议您与 [!DNL Workfront] 顾问合作，创建符合组织要求的报告。 生成某些报告需要熟悉 [!DNL Workfront's] 的文本模式报告。

## 到您了

与您的团队或验证系统管理员联系，了解您将在Workfront中使用哪种类型的报告，以使验证工作流平稳运行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
