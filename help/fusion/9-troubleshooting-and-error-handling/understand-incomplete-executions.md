---
title: 了解未完成的执行
description: 了解执行不完整是什么以及如何处理导致执行不完整的错误 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 了解未完成的执行

未完成的执行可以存储在Workfront Fusion中，稍后可以在其中查看和解析它们。 了解如何利用这一令人惊叹的功能。

在本视频中，您将了解：

* 未完成的执行是什么
* 如何处理导致执行不完整的错误

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## 导致执行不完整的错误

有几类错误会导致存储不完整的执行。

收到的不同错误类型将取决于您连接到的API。 该错误可能是由于数据不完整或错误导致的验证错误，主要原因是缺少预期的项目才能成功处理通过模块的所有数据。 或者，由于临时或长期连接故障（例如，在连接电子邮件或远程FTP服务器期间），最终目标不可用也会发生错误。

如果场景中的第一个模块发生错误，执行将立即停止，并且不会存储不完整的执行。

如果任何其他模块发生错误，并且没有附加错误处理程序路由，则：

* 如果错误类型为ConnectionError、RateLimitError、OutOfSpaceError或ModuleTimeoutError，则存储不完整的执行记录WITH自动重试。
* 如果错误类型为DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError或MaxResultsExceededError，则会存储不完整的执行记录（没有自动重试）。
* 如果错误类型不是上述类型，则执行失败。

## 想要了解更多信息？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
