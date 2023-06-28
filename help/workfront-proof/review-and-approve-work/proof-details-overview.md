---
title: 了解校样详细信息
description: 深入了解中证明背后的详细信息 [!DNL  Workfront] 通过摘要面板和 [!UICONTROL Document Details] 页面。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 了解校样详细信息

## 查看校对详细信息

作为校样经理或所有者，您可以通过摘要面板和 [!UICONTROL Document Details] 页面。 首先，请在以下位置查找您的证明： [!UICONTROL Documents] 项目、任务或问题的部分。

### 摘要面板

摘要面板提供了校对基本详细信息的高级概述。 需要时可使用图标展开面板，不需要时折叠面板。您甚至可以将鼠标悬停在验证的缩略图上以打开或下载验证。

![的图像 [!UICONTROL Documents] 选定了校样并展开摘要面板的项目部分。 摘要面板图标和摘要面板都会突出显示。](assets/document-summary.png)

注意： [!UICONTROL Approvals] 摘要面板中的部分用于 **文档** 批准和 **不是** 绑定到您在本课程中学习到的验证审阅和批准流程。 这两个过程在中是分开的 [!DNL Workfront].

### [!UICONTROL Document Details]

如果您需要有关证明的更多信息，请 [!UICONTROL Document Details] 链接会将您转到以下位置的校样“页面”： [!DNL Workfront].

![中验证页面的图像 [!DNL  Workfront].](assets/document-details.png)

请务必注意，查看与验证过程相关的信息的能力取决于您在中的验证权限 [!DNL Workfront].

在校样页面中，您可以从左侧面板菜单访问以下部分：

* **更新 —** 在验证查看器中所做的评论将显示在此处，并带有“验证评论”标记。 您也可以对文件添加注释，就像对任务或项目添加注释一样（这些注释不会出现在校样查看器中）。
* **批准 —** 此部分用于文档审批，而不是验证审批。 这两种类型的批准是中独立的流程 [!DNL Workfront] 不要链接在一起。 如果您正在将验证工作流用于审阅和审批，则不会使用此部分。
* **所有版本 —** 跟踪和管理验证的版本历史记录。 您可能会发现在 [!UICONTROL Documents] 列表。
* **自定义Forms —** 自定义表单用于验证以捕获特定于组织的信息。 此信息可以与文件一起传送到集成的文档存储系统，例如 [!DNL Workfront] DAM或 [!DNL Adobe’s] AEM。 自定义表单由您设置 [!DNL Workfront] 系统管理员或组管理员。 与您的团队或管理员交谈，了解您是否将在验证上使用自定义表单。
* **校对工作流 —** 管理或修改分配给验证的工作流。 您可以使用以下方式打开此窗口 [!UICONTROL Proofing Workflow] 中证明的链接 [!UICONTROL Documents] 清单上也有。 了解如何使用编辑验证工作流视频更改工作流。

让我们仔细看一下以下两个部分： [!UICONTROL Proofing Viewer Settings] 和 [!UICONTROL Proofing Activity].

### [!UICONTROL Proofing Viewer Settings]

这些设置可帮助您控制对验证本身的访问。

![的图像 [!UICONTROL Proofing Viewer Settings] 从带有的校样页面 [!UICONTROL Proofing Viewer Settings] 选项在左侧面板菜单中突出显示。](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Require login. This proof cannot be shared with guest users]—** 只有具备以下条件的用户才能共享证明： [!DNL Workfront] 校对许可证。
* **[!UICONTROL Require decisions to be electronically signed]—** 共享验证时，这要求收件人拥有验证权限 [!DNL Workfront] 在做出校对决定时，通过输入校对密码使他们“电子签名”校对。 (注意：验证密码与您的验证密码不同， [!DNL Workfront] 密码。 验证密码不可轻松访问，因此大多数收件人不会知道此密码。) [!DNL Workfront] 建议与您的 [!DNL Workfront] 顾问。
* **[!UICONTROL Lock proof when all required decisions are made]—** 一旦对校对做出了每个决定，就会将校对锁定到任何进一步的评论、回复、决定等。 这锁定了整个验证版本，而不仅仅是验证工作流的特定阶段。
* **[!UICONTROL Allow downloading the original file]—** 验证收件人可以从验证查看者下载验证的原始源文件（右侧面板菜单中的选项）。
* **[!UICONTROL Allow sharing proof via public URL or embed code]—** 校样收件人可以与任何人共享可公开访问的校样链接。
* **[!UICONTROL Allow subscribing to proof via public URL or embed code]—** 任何已发送公共URL的人均可将其电子邮件地址和名称（如果不是验证用户）或其电子邮件地址和验证密码（如果是验证用户）添加到验证中。 (注意：验证密码与 [!DNL Workfront] 密码。)

在中上传验证时，可以设置这些相同的设置 [!UICONTROL Proof settings] 部分，位于“上载”窗口底部。

![的图像 [!UICONTROL Proof settings] 区域。](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Proofing Activity]

此页面跟踪验证中发生的所有活动，以及就此验证发送的电子邮件。

![的图像 [!UICONTROL Proofing Activity] 验证页面的部分 [!UICONTROL Proofing Activity] 选项在左侧面板菜单中突出显示。](assets/proofing-activity-in-details.png)

此 [!UICONTROL Activity] 章节时间戳包括何时做出评论和决定，以及由谁做出评论。 它还跟踪验证工作流阶段的开始时间、收件人首次打开验证的时间，以及验证经理或所有者希望了解的其他信息。 例如，当您尝试了解为什么从未启动验证工作流阶段时，这些详细信息可能会很有用。

此 [!UICONTROL Messages] 部分时间戳（将电子邮件警报和消息发送给收件人、发送者以及消息的内容）。 在有人声称未收到有关校样的电子邮件进行故障排除时，这可能会很有用。 您可以检查是否以及何时发送了电子邮件。

[!DNL Workfront] 建议校样管理人员和校样所有者熟悉这两部分中的信息。 当您结合此信息并了解如何阅读 [!UICONTROL SOCD] 进度条，无论验证工作流中的何处，您都可以真正了解和管理验证。

一旦您完成了在 [!UICONTROL Document Details] 部分，使用痕迹导航痕迹导航返回到 [!UICONTROL Documents] 部分附加证明。

![标头中的痕迹导航痕迹的图像。](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
