---
title: 了解未完成的执行
description: 了解什么是未完成的执行，以及如何处理在  [!DNL Adobe Workfront Fusion] 中导致未完成执行的错误。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 93%

---

# 了解未完成的执行

未完成的执行可以存储在 Workfront Fusion 中，稍后可以在那里对其进行审阅和解决。 了解如何利用这个精彩的功能。

在本视频中，您将了解到：

* 什么是未完成的执行
* 如何处理导致执行未完成的错误

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## 导致执行未完成的错误

有几类错误会导致存储未完成的执行。

所收到的不同错误类型取决于您连接的 API。 该错误可能是由未完成或错误的数据引起的验证错误，其主要是因为缺少成功处理通过模块的所有数据所需的项目。 或者，由于临时或长期连接失败（例如，在连接到电子邮件或远程 FTP 服务器期间），最终目的地不可用，从而可能会出现错误。

如果场景中的第一个模块发生错误，则执行会立即停止，并且不会存储未完成的执行。

如果任何其他模块上发生错误并且没有附加错误处理程序路由，则：

* 如果错误类型是 ConnectionError、RateLimitError、OutOfSpaceError 或 ModuleTimeoutError，则会存储未完成的执行记录并会自动重试。
* 如果错误类型为 DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError 或 MaxResultsExceededError，则会存储未完成的执行记录，但不会自动重试。
* 如果错误类型不是上述类型，则执行失败。

## 想要了解详情？ 我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
