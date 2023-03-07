---
title: Webhook演练
description: 了解如何使用webhook创建应用程序以确定客户是否到了购买酒精的年龄，所有这些都可以 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhook演练

## 概述

此方案创建一个便利店应用程序，以便他们轻松确定客户是否到了购买酒精饮料的年龄。 出纳只需将客户的名称和出生日期以及经过验证的客户端令牌发布到提供的URL即可。 输入后，这将触发我们的方案以计算相应的响应并将其返回给请求者。

![使用交换机模块的图像](assets/beyond-basic-modules-5.png)

## Webhook演练

Workfront建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>有关完成演练的分步说明，请转到 [Webhook演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 运动。

## Postman设置

要完成演练练习，您需要下载免费的Postman应用程序。 按照以下步骤导航到Postman的右侧区域进行练习。

1. 创建一个工作区，然后将其打开。
1. 单击“新建”选项卡，并创建一个名为“饮酒年龄”的新收藏集。
1. 再次单击新建选项卡，并创建一个名为GET生日的GET请求。
1. 将请求操作从GET更改为POST。
1. 转到POSTURL字段下的正文子选项卡区域。
1. 在“授权”子选项卡下方选择表单数据。
1. 为Name、Birthdate和clientToken创建三个密钥。

![使用交换机模块的图像](assets/beyond-basic-modules-6.png)

## 轮到你了

>[!NOTE]
>
>练习和挑战是可选的，不是完成Fusion培训所必需的。

此练习练习基于您在演练中所学到的内容，但未提供解决方案。

创建一个等待创建新更新的Workfront webhook，然后记录日期、进行更新的人员姓名以及更新的内容。 将此信息发送给您自己。

**提示**：使用Workfront Watch事件触发器模块创建您的webhook。 此外，在Workfront中，更新称为注释。

**挑战**：您可以查找并添加进行更新的URL以便轻松访问吗？


## 想要了解更多信息？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
