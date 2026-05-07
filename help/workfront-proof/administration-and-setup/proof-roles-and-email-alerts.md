---
title: 校样角色和电子邮件提醒
description: 了解如何启用恰当的校样角色和电子邮件提醒，以便校样收件人可以在  [!DNL  Workfront] 中访问校样并了解正在完成的工作。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:05:31.746Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 544
ht-degree: 100%

---

# 校样角色和电子邮件提醒

校样角色和电子邮件提醒有助于推动校样工作流，确保收件人有权访问校样并了解正在完成的工作。

让我们来回顾一下一些基本的校对术语：

* **校样角色——**&#x200B;定义用户可以对校样执行哪些操作（例如，评论、标记、审批等）。
* **电子邮件提醒——**&#x200B;当校样出现活动时发送给校样工作流中的人员的电子邮件。

![突出显示了 [!UICONTROL Proof role] 和 [!UICONTROL Email alerts] 列的 [!UICONTROL New Proof] 窗口的图像。](assets/proof-roles-and-email-alerts.png)

您的校样系统管理员可以为组织的校样用户设置默认校样角色和电子邮件提醒。 此外，此信息可以内置到校样工作流模板（也称为自动化工作流模板）中。

但是，有时您可能需要在上传校样时手动设置此信息。

[!DNL Workfront] 在向校样收件人分配校样角色时提供以下一般建议：

* **审阅者及审批者——**&#x200B;这些用户既可以对校对发表评论，也可以对校对作出决策（例如审批或拒绝）。 在审阅过程中对关键的内部和外部利益相关者使用此校对角色。
* **审阅者——**&#x200B;如果您的校对工作流中的某些人只需要发表评论，这个角色非常适合他们。 审阅者角色也可以分配给主要上传校对或作为校对所有者但不参与校对流程的 [!DNL Workfront] 用户。
* **只读——**&#x200B;非常适合只需要查看校样的收件人。 [!UICONTROL Read Only] 提供查看访问权限，但不允许发表评论。

[!DNL Workfront] 在向校样收件人分配电子邮件提醒时提供以下一般建议：

* **最终决策——**&#x200B;当最后一个人对校样作出决策时会发送一封电子邮件。 将它分配给监控校样工作流的人员。 这可以是校样管理者、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。 [!DNL Workfront] 建议在使用基本工作流时使用此提醒，以便监控校样的人员知道所有决策均已做出。
* **决策——**&#x200B;当每个校对工作流利益相关者对校对作出决策时会发送提醒。 当使用带有多个决策的自动化工作流时，此选项是最佳选择。 分配给监控校样工作流的人员。 这可以是校样管理者、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。
* **禁用——**&#x200B;对访客校样用户使用此选项，以限制他们收到的有关该校样的电子邮件数量。 收件人仍会收到有关新的校样、新的版本和延迟校样的通知，另外 [!DNL Workfront] 用户会直接收到使用 @username 在校样评论中发出的消息，以及使用 @emailaddress 的访客收件人。

## 到您了

1. 登录 Workfront 并创建将会使用您之前未创建的校对的用户。 根据该人将会在校样工作流中扮演的角色，在用户设置中设置校样权限配置文件。
1. 对于已创建的用户，如果有需要，请编辑其设置，以调整校样权限配置文件选择。
1. 访问校对设置区域，并转到“用户”选项卡。 检查用户的个人设置——语言、时区、日期格式、默认校样角色和默认电子邮件提醒。 如果这些用户是在建立全局系统默认值之前创建的，这一点很重要。

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
