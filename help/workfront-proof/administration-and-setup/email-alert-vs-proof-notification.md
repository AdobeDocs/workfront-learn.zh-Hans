---
title: 了解电子邮件提醒和验证通知
description: 了解  [!DNL  Workfront] 中电子邮件提醒和验证通知之间的区别。
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 65%

---

# 了解电子邮件提醒和验证通知

电子邮件提醒与验证通知电子邮件不同。当为您分配了新验证以供审阅、验证延迟或存在新版本验证供您查看时，您将收到验证通知电子邮件。

![验证通知电子邮件的图像，其表明有新的验证需要审核。](assets/email-alert-1.png)

如果您在上传验证时关闭通知选项，则没有人会收到[!DNL Workfront]关于有新验证需要审查的任何通信。

电子邮件提醒是根据审核人/审批人设置的，最常见的是在上传校样时设置。默认电子邮件警报类型可能会分配给验证收件人，因此您无需每次上传验证时都进行设置。 请与您的系统管理员讨论如何设置这些默认值。

![电子邮件提醒的图像，其中表明已对验证做出决策，并且有评论可供审查。](assets/email-alert-2.png)

即使电子邮件提醒设置为 [!UICONTROL Disabled]，验证收件人仍会收到出现新验证或版本的通知。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 在Workfront设置中，禁用“对验证进行评论时从Workfront发送电子邮件”设置 | 启用此设置后（默认启用），用户可能会针对校样的每条评论收到多封电子邮件通知——一封来自验证功能，一封来自 Workfront 本身。这些重复的通知会导致电子邮件通知受到干扰并出现混乱，并且可能会堵塞电子邮件收件箱，最终可能会导致用户忽略他们收到的验证通知。这进而可能意味着错过最后期限。 <br> <br>注意：此设置可在Workfront主菜单>设置>电子邮件>审阅和批准中找到。 |


