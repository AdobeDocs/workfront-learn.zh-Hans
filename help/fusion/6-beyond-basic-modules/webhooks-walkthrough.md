---
title: Webhook 演练
description: 了解如何使用 Webhook 创建应用程序，以确定客户的年龄是否足以购买酒精饮料，一切尽在  [!DNL Adobe Workfront Fusion]。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 100%

---

# Webhook 演练

此场景创建了一个便利店应用程序，以便他们可以轻松确定顾客的年龄是否足以购买酒精饮料。收银员只需将顾客的姓名和出生日期以及一个经过验证的客户端令牌发布到所提供的 URL 即可。输入后，这会引发我们的场景来计算相应的响应并将其返回给请求者。

![使用切换模块的图像](assets/beyond-basic-modules-5.png)

## Webhook 演练

Workfront 建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on)


## Postman 设置

要完成演练练习，您需要下载免费的 Postman 应用程序。按照以下步骤导航到 Postman 的右侧区域进行练习。

1. 创建一个工作区，然后将其打开。
1. 单击“新建”选项卡并创建一个名为“Drinking Age”的新集合。
1. 再次单击“新建”选项卡，然后创建一个名为“GET birthdate”的新 GET 请求。
1. 将请求操作从 GET 更改为 POST。
1. 转至 POST URL 字段下方的“正文”子选项卡区域。
1. 选择“授权”子选项卡下方的表单数据。
1. 创建三个键：Name、Birthdate 和 clientToken。

![使用切换模块的图像](assets/beyond-basic-modules-6.png)

## 到您了

>[!NOTE]
>
>练习和挑战是可选的，并不是完成 Fusion 培训所必需的。

本练习以您在演练中学到的内容为基础，但未提供解决方案。

创建一个 Workfront Webhook，等待创建的新更新，然后记录日期、更新人员的姓名以及更新内容。通过电子邮件将此信息发送给您自己。

**提示**：使用 Workfront Watch Events 触发器模块创建 Webhook。此外，在 Workfront 中，更新被称为“注释”。

**挑战**：您能否找到并添加更新位置的 URL 以便于访问？


## 想要了解详情？我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hans)
