---
title: 了解未完成的执行
description: 了解未完成的执行是什么，以及如何处理导致在 [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 了解未完成的执行

未完成的执行可以存储在Workfront Fusion中，以后可以在其中进行审核和解析。 了解如何利用这项令人惊叹的功能。

在此视频中，您将学习：

* 未完成的执行
* 如何处理导致执行不完整的错误

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## 导致执行不完整的错误

存储不完整执行时会出现几类错误。

收到的不同错误类型将取决于您连接到的API。 该错误可能是由于数据不完整或错误而导致的验证错误，主要是因为缺少需要成功处理通过模块的所有数据的项目。 或者，由于临时或长期连接失败（例如，在与电子邮件或远程FTP服务器的连接过程中），最终目标的不可用性可能会导致错误。

如果方案中第一个模块发生错误，则执行会立即停止，并且不会存储不完整的执行。

如果任何其他模块发生错误，并且未附加错误处理程序路由，则：

* 如果错误类型为ConnectionError、RateLimitError、OutOfSpaceError或ModuleTimeoutError，则会存储不完整的执行记录WITH自动重试。
* 如果错误类型为DataError、InvalidConfigurationError、InvalidAccessTokenError、InquestedError、MaxFileSizeExceededError或MaxResultsExceededError，则会存储不完整的执行记录（不自动重试）。
* 如果错误类型与上述内容不同，则执行会失败。

## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
