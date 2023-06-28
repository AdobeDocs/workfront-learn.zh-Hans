---
title: 验证角色和电子邮件警报
description: 了解如何启用适当的验证角色和电子邮件警报，以便验证收件人能够访问验证并查看在中完成的工作 [!DNL  Workfront].
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
ht-degree: 0%

---

# 验证角色和电子邮件警报

验证角色和电子邮件警报有助于推动验证工作流，确保收件人有权访问验证并查看正在完成的工作。

我们来看看一些基本的校对术语：

* **校对角色 —** 定义用户可以如何处理验证（例如，评论、标记、批准等）。
* **电子邮件警报 —** 当验证上有活动时，向验证工作流中的人员发送的电子邮件。

![的图像 [!UICONTROL New Proof] 带有以下内容的窗口 [!UICONTROL Proof role] 和 [!UICONTROL Email alerts] 高亮显示的列。](assets/proof-roles-and-email-alerts.png)

验证系统管理员可以为贵组织的验证用户设置默认验证角色和电子邮件警报。 此外，此信息可以内置到验证工作流模板（也称为自动化工作流模板）中。

但是，在上传验证时，有时需要手动设置此信息。

[!DNL Workfront] 为验证收件人分配验证角色时提供以下一般建议：

* **审阅者和批准者 —** 这些用户既可以对验证进行评论，也可以对验证做出决定（例如批准或拒绝）。 在审核过程中为关键内部和外部利益相关者使用此验证角色。
* **审阅者 —** 您的验证工作流中的某些人只需要发表评论，此角色非常适合他们。 也可以将审阅者角色分配给 [!DNL Workfront] 主要上传验证或作为验证所有者但不属于验证过程的用户。
* **只读 —** 非常适合只需要查看证明的收件人。 [!UICONTROL Read Only] 提供视图访问权限，不允许进行评论。

[!DNL Workfront] 为验证收件人分配电子邮件警报时提供以下一般建议：

* **最终决定 —** 当最后一个人员对验证做出决定时，这将发送电子邮件。 将此工作流分配给监控验证工作流的人员。 这可以是校样管理器、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。 [!DNL Workfront] 建议在使用基本工作流时发出此警报，以便监控证明的人员知道已做出所有决策。
* **决策 —** 当每个验证工作流利益相关者对验证做出决定时，这会发送警报。 当使用具有多个决策的自动化工作流时，此选项效果最佳。 分配给监控验证工作流的人员。 这可以是校样管理器、校样所有者、校样创建者、项目经理或其他 [!DNL Workfront] 用户。
* **已禁用 —** 对Guest Proof用户使用此项来限制他们收到的有关校对的电子邮件数量。 收件人仍会收到有关新验证、新版本和最新验证的通知，以及 [!DNL Workfront] 用户会收到在验证评论中通过@username和具有@emailaddress的访客收件人发送的私信。

## 轮到你了

1. 登录Workfront并创建将使用您之前未创建的校对的用户。 根据人员在验证工作流中将扮演的角色，在其用户设置中设置验证权限配置文件。
1. 对于已创建的用户，如果需要，可编辑其设置以调整校样权限配置文件选择。
1. 访问校对设置区域，然后转到“用户”选项卡。 检查用户的个人设置 — 语言、时区、日期格式、默认验证角色和默认电子邮件警报。 如果这些用户在全局系统默认值建立之前创建，则这一点很重要。

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
