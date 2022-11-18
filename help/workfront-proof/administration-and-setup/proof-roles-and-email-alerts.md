---
title: 校样角色和电子邮件警报
description: 了解如何启用适当的校样角色和电子邮件警报，以便校样收件人有权访问校样并了解中正在完成的工作 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 校样角色和电子邮件警报

校样角色和电子邮件警报有助于推动校样工作流程，确保收件人有权访问校样，并能够看到正在完成的工作。

让我们查看一些基本校样术语：

* **证明角色 —** 定义用户可以使用校样执行的操作（例如注释、标记、批准等）。
* **电子邮件警报 —** 当校样上存在活动时，在校样工作流中向人员发送电子邮件。

![图像 [!UICONTROL New Proof] 窗口 [!UICONTROL Proof role] 和 [!UICONTROL Email alerts] 列。](assets/proof-roles-and-email-alerts.png)

校样系统管理员可以为组织的校样用户设置默认校样角色和电子邮件警报。 此外，此信息还可内置到校样工作流模板（也称为自动工作流模板）中。

但是，有时您可能需要在上传校样时手动设置此信息。

[!DNL Workfront] 在为校样收件人分配校样角色时，提供了以下一般建议：

* **审核者和审批者 —** 这些用户既可以对校样进行评论，也可以对校样做出决策（例如批准或拒绝）。 在审核过程中，将此验证角色用于关键的内部和外部利益相关者。
* **审阅人 —** 您的校样工作流中的某些人员只需发表评论，此角色非常适合他们。 也可以将审核者角色分配给 [!DNL Workfront] 主要上传校样或充当校样所有者，但其他情况则不属于校样过程的用户。
* **只读 —** 非常适合只需查看校样的收件人。 [!UICONTROL Read Only] 授予视图访问权限，且不允许进行评论。

[!DNL Workfront] 在向校样收件人分配电子邮件警报时，提供了以下一般建议：

* **最后决定 —** 当最后一个人对校样做出决策时，会发送一封电子邮件。 将其分配给监控校样工作流的人员。 这可以是校样管理器、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。 [!DNL Workfront] 在使用基本工作流时建议使用此警报，以便监控校样的人员知道已做出所有决策。
* **决策 —** 当每个校样工作流利益相关方决定校样时，这会发送警报。 此选项最适合在使用包含多项决策的自动工作流时使用。 将分配给监控校样工作流的人员。 这可以是校样管理器、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。
* **已禁用 —** 将此功能用于来宾校样用户，以限制他们收到的有关校样的电子邮件数量。 收件人仍会收到有关新校样、新版本和延迟校样的通知，以及 [!DNL Workfront] 用户将收到校样评论中使用的@username和来宾收件人在@emailaddress中发送的私信。

## 该你了

1. 登录到Workfront，并创建将使用您之前未创建的校对的用户。 根据人员在校样工作流中将扮演的角色，在用户设置中设置校样权限配置文件。
1. 对于已创建的用户，根据需要编辑其设置以调整和校样权限配置文件选择。
1. 访问校对设置区域，然后转到“用户”选项卡。 检查用户的个人设置 — 语言、时区、日期格式、默认校样角色和默认电子邮件警报。 如果这些用户是在建立全局系统默认值之前创建的（这些设置在此学习路径的第1节中讨论），则这一点很重要。

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
