---
title: Webhooks演练
description: 了解如何使用WebHook创建应用程序来确定客户是否年纪大到足以购买酒精，所有这些操作均在 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 0618bf27478744e0e9976015a24c5ec8519efbb7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhooks演练

## 概述

这种情景会创建一个便利店应用程序，以便他们能够轻松确定顾客是否年纪大到足以购买酒精。 收银员只需将客户的姓名和出生日期以及经过验证的客户令牌发布到提供的URL即可。 输入后，将触发我们的方案以计算相应的响应并将其返回给请求者。

![使用开关模块的图像](assets/beyond-basic-modules-5.png)

## Webhooks演练

Workfront建议先观看练习视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>有关完成演练的分步说明，请转到 [Webhooks演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 练习。

## Postman设置

要完成演练练习，您需要下载免费的Postman应用程序。 请按照以下步骤导航到Postman的正确区域进行练习。

1. 创建工作区，然后将其打开。
1. 单击“新建”选项卡，然后创建一个名为“饮用年龄”的新集合。
1. 再次单击新建选项卡，然后创建一个名为GET出生日期的新GET请求。
1. 将请求操作从GET更改为POST。
1. 转到“POSTURL”字段下方的“正文”子选项卡区域。
1. 在“授权”子选项卡下方选择表单数据。
1. 为Name、Martidate和clientToken创建三个键。

![使用开关模块的图像](assets/beyond-basic-modules-6.png)

## 该你了

>[!NOTE]
>
>实践练习和挑战是可选的，完成融合培训并非必需的。

此练习以您在演练中学到的内容为基础，但未提供解决方案。

创建一个Workfront Webhook，等待创建的新更新，然后记录日期、进行更新的人员姓名以及更新的内容。 向您自己发送此信息。

**提示**:使用Workfront Watch事件触发模块创建Webhook。 此外，在Workfront中，更新称为注释。

**挑战**:能否找到并添加进行更新的URL以便轻松访问？


## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
