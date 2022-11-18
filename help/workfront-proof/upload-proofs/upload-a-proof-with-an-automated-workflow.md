---
title: 使用自动工作流上传校样
description: 了解何时使用自动校样工作流，如何使用校样模板应用工作流，以及如何从头开始设置自动工作流。
activity: use
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335133.png
kt: 8833
exl-id: 8301ef00-1f47-4779-aa35-c735b66fdcac
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 使用自动工作流上传校样

在此视频中，您将学习：

* 何时可使用自动校样工作流
* 如何使用校样模板应用工作流
* 如何从头开始设置自动化工作流

>[!VIDEO](https://video.tv.adobe.com/v/335133/?quality=12)



## 其他校样工作流设置

校样上传窗口底部的设置是可选的，因此请咨询您的组织，了解是否以及您是如何使用这些设置的。

![图像 [!UICONTROL New Proof ]窗口 [!UICONTROL Stage settings] 突出显示。](assets/additional-proof-workflow-settings.png)

* **[!UICONTROL Lock stage]—** 这样可防止此工作流阶段的人员在工作流阶段完成后做出评论或更改决策。
* **[!UICONTROL Transfer primary decision rights to]—** 通过指定主决策者来加快校对过程。 设置后， [!DNL Workfront] 将此人的证明决定识别为THE决定。 一旦他们做出决定，就会结束，不需要其他决定。
* **[!UICONTROL Require only one decision for this stage]—** 简化校样流程的另一种方法是，只需对校样做出一个决定。 启用此设置后，无论您在该阶段有多少批准者，如果其中任何人做出决定，该阶段即告结束。
* **[!UICONTROL Make this stage private]—** 默认情况下，校样中的注释对所有阶段的每个人都可见。 通过单击方框，防止其他阶段的校样收件人看到在此阶段中的评论。

在校样上载窗口的底部，有一些校样设置会影响校样的安全性，例如要求登录才能查看校样。

<!--
Learn more about these in the Proof settings section of the Configure a proof article.
-->

![图像 [!UICONTROL Proof settings] 校样上传窗口的部分。](assets/additional-proof-workflow-settings-2.png)

<!--
### Learn more
* Automated workflow overview
* Automated workflow stages overview
-->

<!--
### Guides
* Plan an advanced workflow worksheet
-->

## 为什么要使用校样工作流？

您会注意到自己位于校样收件人列表中，因为您是上传校样的人。 这也会使您成为校样所有者，从而为您提供校样的编辑权限，从而允许您更改工作流设置或上传新版本等。

![校样上传窗口的图像，校样所有者在收件人列表中突出显示。](assets/proof-owner.png)

如果您只是上传校样，但其他人将管理工作流，则可以通过单击 [!UICONTROL Owner] 链接并输入其名称。 如果原始Uploader之外的其他人将要上传版本，则建议使用此方法。

## 该你了

>[!IMPORTANT]
>
>别忘了提醒你的同事，作为Workfront培训的一部分，你要向他们发送证据。


使用高级工作流上传校样。 如果贵组织已设置校样模板，请选择团队使用的模板，然后进行一些调整。

* 调整电子邮件警报，以便在校样中发生活动时，不会收到任何通知。
* 第一阶段应有2名审查人/批准人。
* 第二个阶段应当只有1个审核者/审批者。

如果贵组织尚未创建校样模板，请从头开始设置一个两步工作流。

* 将您自己和您最喜爱的同事分配到第一个阶段。
* 将创建校样后第1步的截止日期设为1天。
* 将另一个最喜爱的同事分配到第二阶段。
* 当第一阶段的截止期限过后，舞台就会开始。
* 为此阶段中的人员提供2天的时间来完成审阅，但必须在中午之前完成。


