---
title: 创建自动化工作流模板
description: 了解如何通过分配校样收件人和设置校样截止日期来创建自动化工作流模板。然后与其他用户共享该模板。
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 100%

---

# 创建自动化工作流模板

在本视频中，您将学习如何：

* 创建用于 [!DNL  Workfront] 校对的自动化工作流模板
* 分配校样收件人
* 设定审阅和审批流程的截止日期
* 与其他人共享自动化工作流模板

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops=1)

## 附加阶段激活选项

用于确定校对工作流阶段何时开始的两个选项很少使用（如果用到的话）：[!UICONTROL Date and time] 选项和 [!UICONTROL When the previous stage deadline passes] 选项。

第二种选项实际上只适用于有一大群人在审阅，而您不想等待所有人的情况。这有点像“我会给您一定的时间来完成审阅，在此之后，您就会失去审阅机会”的选择。但即使这样也会减慢审阅过程。

如果您确实要使用“[!UICONTROL when the previous stage deadline passes]”，请记住，如果您不想等待最后期限过去，您可以随时手动激活某个阶段，这一点很重要。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 将校对创建者的校对角色设置为审阅者。 | 审阅者校对角色可确保校对创建者能够发表评论并访问其他人留下的评论。大多数时候，校样创建者不需要对他们上传的校样作出决策。审批者、审阅者及审批者、作者或主持人校对角色都需要作出决策。如果校样创建者分配获得这些校样角色中的一个但从未作出决策，这可能会对满足校样截止日期产生不利影响。 |
| 避免使用“审批人”校样角色。 | 审批人校样角色不允许用户对此校样发表评论。这可能会导致用户拒绝校样，而不做任何解释，因为他们无法发表评论。请改用审阅者及审批者校对角色，以便用户可以提供反馈。 |
| 避免使用“所有活动”校样电子邮件提醒选项。 | 每当校样出现任何情况时（作出评论、发布回复、作出决策等），此选项都会发送校样电子邮件通知。收件人实质上会实时看到校样活动。<br><br>对于校样所有者和创建者来说，“决策”电子邮件提醒最适合多阶段校样工作流，而“最终决策”则最适合单阶段工作流。一般来说，可以将其他人都设置为“禁用”，除非他们希望收到其他人作出评论或决策的通知（在这种情况下，选择摘要电子邮件选项中的一个可能效果最好）。 |
