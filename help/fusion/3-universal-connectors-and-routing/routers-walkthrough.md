---
title: 路由器演练
description: 了解如何使用路由器将Pokemon与超级英雄捆绑在 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: 57b112921738c01fe4222e50403c8953c412a0f7
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 路由器演练

使用路由器将Pokemon与超级英雄捆绑到正确的路径中，然后为每个字符创建一个任务。

![融合场景的图像](assets/universal-connectors-and-routing-2.png)

## 路由器演练

Workfront建议先观看练习视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on)

## 练习URL

* 超级英雄API网站： `https://www.superheroapi.com/`
* 练习的第一个URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* 练习的第二个URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

如果您在访问自己的超级英雄令牌时遇到问题，您可以使用此共享令牌：10110256647253588。 请考虑您调用超级英雄API的次数，以便此共享令牌可继续适用于所有人。

>[!TIP]
>
>有关完成演练的分步说明，请转到 [路由器演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) 练习。


## 在映射面板中搜索项目

映射面板顶部的搜索项目字段可帮助您快速查找面板中的字段，即使这些字段嵌套在数组中也是如此。 搜索不区分大小写。

![第一个搜索面板的图像](assets/universal-connectors-and-routing-3.png)

![第二个搜索面板的图像](assets/universal-connectors-and-routing-4.png)

## 使用API的提示和技巧

到目前为止，您还使用了一个非常简单的API（应用程序编程接口），它不需要额外的身份验证即可获取场景中所需的信息。 以下是一些提示，可帮助您使用API和通用连接器进行导航。

## 步骤1:确定API类型

Workfront和许多软件系统都使用REST（代表性状态传输）API构建，REST是当今最简单、最标准的API类型。 但是，还有一些其他因素，例如：

* SOAP（简单对象访问协议）(Workfront的校样API基于SOAP)
* FTP（文件传输协议）
* SFTP（安全文件传输协议）
* 要了解更多信息，请进行Web搜索以查找所关注的API类型和关键字。

>[!NOTE]
>
>连接到Salesforce等较大的平台时，这些平台的不同区域将提供不同的API。 确保找到要连接到的服务的正确服务。

## 步骤2:确定API所需的身份验证类型

API身份验证是一种用于控制对服务的访问的标识形式，例如，当您尝试通过Workfront Fusion进行连接时。 它有助于您向其他系统证明您有权访问该系统。 OAuth 2是当前使用的最常见的身份验证类型。 通过Internet搜索了解有关API身份验证的更多信息。

使用API时，身份验证可能是最困难的方面。 Workfront Fusion通用连接器的最有价值的功能之一是，当使用基本身份验证等常用身份验证方法（如OAuth 2、API密钥等）时，Workfront Fusion可以为您处理身份验证。 在您为身份验证方法（例如OAuth 2）使用相应的Workfront Fusion模块创建连接后，每当您想要运行方案时，Workfront Fusion都会持续生成API密钥和/或令牌。

了解Workfront在关于Experience League的增强身份验证概述文章中提供的不同类型的身份验证。

## 步骤3:阅读API文档并查找所需的端点

当API与其他系统交互时，此通信的接触点被视为端点。 端点是API发送请求和资源所在的位置。

在使用通用连接器与API交互时，您需要了解API支持的端点以及每个请求需要哪些数据。 API文档应描述API的端点以及如何执行常见操作，如创建、读取、更新或删除。 执行这些调用需要一些实践，特别是当您是初次使用API调用或新API的用户时。

进一步了解Workfront Fusion Universal Connectors，以及如何将它们设置为与Experience League所需的API连接。

## 最终说明

您可以在Experience League中查看我们预建应用程序连接器的完整列表。 如果您想向Workfront Fusion产品团队建议一个新的应用程序连接器，请将您的想法提交给Innovation Lab。 如果您以前没有提交过，请进一步了解创新实验室，以及如何投票支持创意并参与一年两次的领导委员会优先安排。 如果您已经有权访问创新实验室，请登录并提交您的想法。

## 该你了

>[!NOTE]
>
>实践练习和挑战是可选的，完成融合培训并非必需的。

此练习以您在演练中学到的内容为基础，但未提供解决方案。

在为Pokemon字符设置多个变量模块中，创建一个名为“Stat(Level)”的变量。 将Pokemon统计资料的名称映射到此变量。 使用数组值功能更改数组的显示方式，以便每个Stat都是一条新线，如下所示。

**提示：** 只有6个不同的Pokemon统计资料具有相应的级别。

![统计资料图像](assets/universal-connectors-and-routing-5.png)

**挑战：** 查看是否可以使用数组公式获取与上述不同行显示相同的功能，而不是用逗号分隔的值字符串。 下面的屏幕截图中提供了提示。

![数组名称的图像](assets/universal-connectors-and-routing-6.png)

## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
