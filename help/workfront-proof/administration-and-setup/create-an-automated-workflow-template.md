---
title: 创建自动化工作流模板
description: 了解如何通过分配验证收件人和设置验证截止日期来创建自动化工作流模板。然后与其他用户共享该模板。
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 58%

---

# 创建自动化工作流模板

在本视频中，您将学习如何：

* 创建用于 [!DNL  Workfront] 验证的自动化工作流模板
* 分配验证收件人
* 设定审查和审批流程的截止日期
* 与其他人共享自动化工作流模板

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## 附加阶段激活选项

很少（如果有的话）使用两个选项来确定校对工作流阶段的启动时间： [!UICONTROL Date and time] 选项和&quot;[!UICONTROL When the previous stage deadline passes]”选项。

第二个选项真的只适用于有大量人员查看并且您不想等待所有人员的场景。 这有点像是“我会给你一些时间来完成您的审核，然后您就失去了机会”选项。 但即使这样也会减慢审查过程。

如果您确实使用“[!UICONTROL when the previous stage deadline passes]，”请务必记住，如果您不想等待截止日期过去，可以随时手动激活阶段。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 将校对创建者的校对角色设置为查看者。 | 审核人验证角色可确保验证创建者能够发表评论并访问其他人留下的评论。大多数情况下，校样创建者无需对已上传的校样做出决定。 审批人、审核人及审批人、作者或主持人验证角色都需要做出决策。如果验证创建者分配获得这些验证角色中的一个但从未做出决策，这可能会对满足验证截止日期产生不利影响。 |
| 避免使用“审批人”验证角色。 | 审批人验证角色不允许用户对此验证发表评论。这可能导致用户拒绝验证，且没有任何解释，因为他们无法发表评论。 请改用审核人及审批人验证角色，以便用户可以提供反馈。 |
| 避免使用“所有活动”验证电子邮件提醒选项。 | 每当校样出现任何情况时（做出评论、发布回复、做出决策等），此选项都会发送校样电子邮件通知。收件人实质上会实时看到验证活动。<br><br>对于验证所有者和创建者，决策电子邮件警报最适合多阶段验证工作流，最终决策最适合单阶段工作流。 一般来说，可以将其他人都设置为“禁用”，除非他们希望收到其他人做出评论或决策的通知（在这种情况下，选择摘要电子邮件选项中的一个可能效果最好）。 |
