---
title: 了解验证细节
description: 通过摘要面板和 [!UICONTROL Document Details] 页面，深入了解  [!DNL  Workfront]  中验证背后的细节。
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
ht-degree: 100%

---

# 了解验证细节

## 查看验证细节

作为验证管理者或所有者，您可以通过摘要面板和 [!UICONTROL Document Details] 页面深入了解验证背后的细节。首先在项目、任务或问题的 [!UICONTROL Documents] 部分找到您的验证。

### 摘要面板

摘要面板提供了对验证基本细节的高级概述。使用该图标可在需要时展开面板，并在不需要时折叠面板。您甚至可以通过将鼠标悬停在验证的缩略图上来打开或下载它。

![项目 [!UICONTROL Documents] 部分的图像，其中已选择验证并已展开摘要面板。摘要面板图标和摘要面板均突出显示。](assets/document-summary.png)

注释：摘要面板中的 [!UICONTROL Approvals] 部分用于&#x200B;**文件**&#x200B;审批，****&#x200B;与您在本课程中学习的验证审查和审批流程无关。这两个流程在 [!DNL Workfront] 中是分开的。

### [!UICONTROL Document Details]

如果您需要有关验证的更多信息，[!UICONTROL Document Details] 链接可带您前往 [!DNL Workfront] 中的验证“页面”。

![[!DNL  Workfront] 中验证页面的图像。](assets/document-details.png)

需要注意的是，能否查看与验证过程相关的信息取决于您在 [!DNL Workfront] 中的验证权限。

在验证页面中，您可以从左侧面板菜单访问这些部分：

* **更新——**&#x200B;在验证查看器中所做的评论会在此处显示，并带有“验证评论”标记。您还可以对文件发表评论，就像对任务或项目发表评论一样（这些评论不会出现在验证查看器中）。
* **审批——**&#x200B;此部分用于文件审批，而不是验证审批。这两种类型的审批在 [!DNL Workfront] 中是单独的流程，它们之间没有关联。如果您使用验证工作流进行审核和审批，则不会用到此部分。
* **所有版本——**&#x200B;跟踪和管理验证的版本历史记录。您可能会发现在 [!UICONTROL Documents] 列表的摘要面板中更容易访问这些信息。
* **自定义表单——**&#x200B;自定义表单用于验证，以捕获特定于组织的信息。该信息可以与文件一起传递到集成文档存储系统，例如 [!DNL Workfront] DAM 或 [!DNL Adobe’s] AEM。自定义表单由您的 [!DNL Workfront] 系统管理员或组管理员设置。请与您的团队或管理员沟通，了解您是否会在验证上使用自定义表单。
* **验证工作流——**&#x200B;管理或修改分配给验证的工作流。您也可以使用 [!UICONTROL Documents] 列表中验证上的 [!UICONTROL Proofing Workflow] 链接打开此窗口。通过观看《编辑验证工作流》视频，了解如何更改该工作流。

让我们仔细看看其中的两个部分：[!UICONTROL Proofing Viewer Settings] 和 [!UICONTROL Proofing Activity]。

### [!UICONTROL Proofing Viewer Settings]

这些设置可以帮助您控制对验证本身的访问。

![验证页面中 [!UICONTROL Proofing Viewer Settings] 的图像，其中左侧面板菜单中突出显示 [!UICONTROL Proofing Viewer Settings] 选项。](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Require login. This proof cannot be shared with guest users]——**&#x200B;该验证只能与拥有 [!DNL Workfront] 验证许可的人共享。
* **[!UICONTROL Require decisions to be electronically signed]——**&#x200B;共享验证时，要求收件人在 [!DNL Workfront] 中具有验证权限，并在作出验证决策时通过输入验证密码对验证进行“电子签名”。（注：验证密码与您的 [!DNL Workfront] 密码不同。验证密码不易获取，因此大多数收件人都不会知道该密码。）[!DNL Workfront] 建议在使用此功能之前与您的 [!DNL Workfront] 顾问沟通。
* **[!UICONTROL Lock proof when all required decisions are made]——**&#x200B;在对验证作出每个决策后，这会对其进行锁定，无法再进一步地评论、回复、作出决策等。这会锁定整个验证版本，而不仅仅是验证工作流中的特定阶段。
* **[!UICONTROL Allow downloading the original file]——**&#x200B;验证收件人可以从验证查看器中下载验证的原始源文件（该选项位于右侧面板菜单中）。
* **[!UICONTROL Allow sharing proof via public URL or embed code]——**&#x200B;验证收件人可以与任何人共享可公开访问的验证链接。
* **[!UICONTROL Allow subscribing to proof via public URL or embed code]——**&#x200B;收到公共 URL 的任何人都可以使用其电子邮件地址和姓名（如果不是验证用户）或其电子邮件地址和验证密码（如果是验证用户）将自己添加到验证中。（注释：验证密码与 [!DNL Workfront] 密码不同。）

在上传窗口底部的 [!UICONTROL Proof settings] 部分上传验证时，可以进行相同的设置。

![上传窗口底部的 [!UICONTROL Proof settings] 部分的图像。](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Proofing Activity]

此页面会跟踪验证上出现的所有活动，以及所发送的有关此验证的电子邮件信息。

![验证页面中 [!UICONTROL Proofing Activity] 部分的图像，其中左侧面板菜单中突出显示 [!UICONTROL Proofing Activity] 选项。](assets/proofing-activity-in-details.png)

[!UICONTROL Activity] 部分标记了发表评论和作出决策的时间，以及发表评论和作出决策的人。它还会跟踪验证工作流阶段何时开始、收件人何时首次打开验证，以及验证管理者或所有者想要了解的其他信息。例如，当您希望弄清楚为什么验证工作流阶段从未启动等问题时，这些详细信息可能会很有帮助。

[!UICONTROL Messages] 部分标记了向收件人发送电子邮件提醒和消息的时间、发送者以及消息的内容。如果有人说他们没有收到有关验证的电子邮件，这在对此进行故障排除时会很有用。您可以检查电子邮件是否以及何时发送。

[!DNL Workfront] 建议验证管理者和所有者熟悉这两个部分中的信息。当您将这些信息与有关理解如何阅读 [!UICONTROL SOCD] 进度条的信息相结合时，无论验证在验证工作流中处于何处，您都可以真正地理解和管理您的验证。

在完成 [!UICONTROL Document Details] 部分后，使用痕迹导航路径返回附有该验证的项目、任务或问题的 [!UICONTROL Documents] 部分。

![标题中痕迹导航路径的图像。](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
