---
title: 验证角色和电子邮件提醒
description: 了解如何启用恰当的验证角色和电子邮件提醒，以便验证收件人可以在  [!DNL  Workfront] 中访问验证并了解正在完成的工作。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 100%

---

# 验证角色和电子邮件提醒

验证角色和电子邮件提醒有助于推动验证工作流，确保收件人有权访问验证并了解正在完成的工作。

让我们来回顾一下一些基本的验证术语：

* **验证角色——**&#x200B;定义用户可以对验证执行哪些操作（例如，评论、标记、审批等）。
* **电子邮件提醒——**&#x200B;当验证出现活动时发送给验证工作流中的人员的电子邮件。

![突出显示了 [!UICONTROL Proof role] 和 [!UICONTROL Email alerts] 列的 [!UICONTROL New Proof] 窗口的图像。](assets/proof-roles-and-email-alerts.png)

您的验证系统管理员可以为组织的验证用户设置默认验证角色和电子邮件提醒。此外，此信息可以内置到验证工作流模板（也称为自动化工作流模板）中。

但是，有时您可能需要在上传验证时手动设置此信息。

[!DNL Workfront] 在向验证收件人分配验证角色时提供以下一般建议：

* **审核人及审批人——**&#x200B;这些用户既可以对验证发表评论，也可以对验证作出决策（例如审批或拒绝）。在审核过程中对关键的内部和外部利益相关者使用此验证角色。
* **审核人——**&#x200B;如果您的验证工作流中的某些人只需要发表评论，这个角色非常适合他们。审核人角色也可以分配给主要上传验证或作为验证所有者但不参与验证流程的 [!DNL Workfront] 用户。
* **只读——**&#x200B;非常适合只需要查看验证的收件人。[!UICONTROL Read Only] 提供查看访问权限，但不允许发表评论。

[!DNL Workfront] 在向验证收件人分配电子邮件提醒时提供以下一般建议：

* **最终决策——**&#x200B;当最后一个人对验证作出决策时会发送一封电子邮件。将它分配给监控验证工作流的人员。这可以是验证管理者、验证所有者、验证创建者、项目经理或其他 [!DNL Workfront] 用户。[!DNL Workfront] 建议在使用基本工作流时使用此提醒，以便监控验证的人员知道所有决策均已做出。
* **决策——**&#x200B;当每个验证工作流利益相关者对验证作出决策时会发送提醒。当使用带有多个决策的自动化工作流时，此选项是最佳选择。分配给监控验证工作流的人员。这可以是验证管理者、验证所有者、验证创建者、项目经理或其他 [!DNL Workfront] 用户。
* **禁用——**&#x200B;对访客验证用户使用此选项，以限制他们收到的有关该验证的电子邮件数量。收件人仍会收到有关新的验证、新的版本和延迟验证的通知，另外 [!DNL Workfront] 用户会直接收到使用 @username 在验证评论中发出的消息，以及使用 @emailaddress 的访客收件人。

## 到您了

1. 登录 Workfront 并创建将会使用您之前未创建的验证的用户。根据该人将会在验证工作流中扮演的角色，在用户设置中设置验证权限配置文件。
1. 对于已创建的用户，如果有需要，请编辑其设置，以调整验证权限配置文件选择。
1. 访问验证设置区域，并转到“用户”选项卡。检查用户的个人设置——语言、时区、日期格式、默认验证角色和默认电子邮件提醒。如果这些用户是在建立全局系统默认值之前创建的，这一点很重要。

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
