---
title: 跟踪校样进度
description: 了解如何使用 [!UICONTROL SOCD] 用于跟踪中校样进度的指标、校样进度和报告 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 跟踪校样进度

作为审核和批准流程中的项目经理、校样经理或其他利益相关方，您将需要跟踪校样的进度。 您可以使用 [!DNL Workfront’s] 内置 **验证进度指标** 在 [!UICONTROL Documents] 页面或通过编写自定义报表。

要查看 [!DNL Workfront]，则您必须拥有“计划”、“工作”或“审阅”许可证，并且是校样用户。 如果你不确定 [!DNL Workfront] 配置文件符合这些要求，请咨询贵组织的校样系统管理员。

## 跟踪校样进度 [!UICONTROL SOCD] 指标和验证状态

通过 [!UICONTROL SOCD] 图标 [!UICONTROL Documents] 列表。 这些图标指示对校样执行的特定操作。

![图像 [!UICONTROL Documents] 列表 [!DNL  Workfront] 项目 [!UICONTROL SOCD] 图标。](assets/manage-proofs-socd.png)

这些图标表示从您向收件人发送校样到他们决定校样时对校样所做的工作。

* **S —** 校样已发送给收件人。
* **O —** 校样已打开。
* **C —** 已对证据提出意见。
* **D —** 对证据（批准、拒绝等）作出了决定。

颜色指示操作是否完成。

* **白色 —** 这步还没发生。
* **绿色 —** 该步骤已完成。
* **橙色 —** 校样截止时间在24小时内，且步骤尚未发生。
* **红色 —** 校样截止日期已过，并且步骤未发生。

的 [!UICONTROL SOCD] 在 [!UICONTROL Documents] 列表、摘要面板或 [!UICONTROL Document Details]，是校样进度的高级摘要。 [!DNL Workfront] 根据校样过程中“落后最多”的收件人配置此设置。

例如，如果有三个审阅者/批准者，并且其中只有两个审阅者/批准者查看了校样并做出了评论，则 [!UICONTROL SOCD] 图标将显示校样已发送([!UICONTROL S])和已打开([!UICONTROL O])，但尚未发表评论([!UICONTROL C])。

如果您想了解每个校样收件人的工作方式，请打开校样工作流。 整个验证进度位于窗口顶部。 每个阶段在灰色栏中都有其自己的进度指示器。  每个用户旁边都是这个人的进度。

![图像 [!UICONTROL Proofing Workflow] 文档的子部分。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校样状态

校样状态基于阶段校样收件人的状态。 在 [!UICONTROL Documents] 页面右侧 [!UICONTROL SOCD] 指示器，以便您能够轻松判断是否对证明做出了决定。

![图像 [!UICONTROL Documents] 列表 [!DNL  Workfront] 项目，并突出显示整体校样状态。](assets/manage-proofs-overall-status.png)

此校样状态表示校样的整体状态。 例如，如果两个收件人批准了校样，则其各个状态将显示 [!UICONTROL Approved]. 但是，第三个收件人尚未做出决定，因此该人的状态为 [!UICONTROL Pending]. 因此，整体状态显示为 [!UICONTROL Pending].

如果为贵组织配置了自定义状态，则将使用这些状态。 否则，您将看到以下标准状态选项：

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

打开校样工作流窗口，以查看分配了 [!UICONTROL Reviewer & Approver] 或 [!UICONTROL Approver ]校样角色。

## 报表 [!DNL Workfront]

您还可以利用 [!DNL Workfront’s] 报告功能来跟踪在审阅和批准过程中发生的校样。

校样批准报表可帮助您跟踪未完成的批准，以确保满足截止日期。

![中校样批准报告的图像 [!DNL  Workfront].](assets/proof-approval-report.png)

利用文档版本报表，可管理和跟踪校样版本。

![文档版本报表的图像，位于 [!DNL  Workfront].](assets/document-version-report.png)

我们建议您与 [!DNL Workfront] 顾问创建符合贵组织要求的报表。 有些报表需要熟悉 [!DNL Workfront’s] 文本模式报告。

## 该你了

请与您的团队或校样系统管理员联系，以了解您将在Workfront中使用哪种报表来保持校样工作流的顺利运行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
