---
title: 了解电子邮件提醒和校样通知
description: 了解  [!DNL  Workfront] 中电子邮件提醒和校样通知之间的区别。
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:07:01.396Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 100%

---

# 了解电子邮件提醒和校样通知

电子邮件提醒与校样通知电子邮件不同。 当您分配获得需要审阅的新校对、校对延迟或有新版本的校对供您查看时，您将会收到校对通知电子邮件。

![校对通知电子邮件的图像，其表明有新的校对需要审阅。](assets/email-alert-1.png)

如果您在上传校对时关闭通知选项，则没有人会收到[!DNL Workfront]关于有新校对需要审阅的任何通信。

电子邮件提醒是根据审阅者/审批者设置的，最常见的是在上传校对时设置。 默认电子邮件提醒类型可能会分配给您的校样收件人，因此您不必在每次上传校样时都进行设置。 请与您的系统管理员讨论如何设置这些默认值。

![电子邮件提醒的图像，其中表明已对校对作出决策，并且有评论可供审阅。](assets/email-alert-2.png)

即使电子邮件提醒设置为 [!UICONTROL Disabled]，校样收件人仍会收到出现新校样或版本的通知。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 在 Workfront 设置中禁用“对校样发表评论时从 Workfront 发送电子邮件”设置。 | 启用此设置后（默认启用），用户可能会针对校对的每条评论收到多封电子邮件通知——一封来自校对功能，一封来自 Workfront 本身。 这些重复的通知会导致电子邮件通知受到干扰并出现混乱，并且可能会堵塞电子邮件收件箱，最终可能会导致用户忽略他们收到的校样通知。 而这可能会意味着错过最后期限。<br> <br>注释：此设置可在 Workfront 主菜单 > 设置 > 电子邮件 > 审阅及审批中找到。 |


