---
title: 高级聚合演练
description: 了解如何调用Web服务以返回有关多个国家/地区的详细信息并识别按子区域分组的人口，所有这些都在 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 高级聚合演练

## 概述

调用Web服务可返回有关多个国家/地区的详细信息，并确定按次区域分组的所有国家/地区的总人口。

![融合场景的图像](assets/iteration-and-aggregation-3.png)

## 高级聚合演练

Workfront建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## 练习URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>有关完成演练的分步说明，请转到 [高级聚合演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 运动。

## 聚总原理的强化

每当模块输出多个包时，之后的每个模块都会执行每个包。

要防止出现这种情况，请在可能生成多个捆绑包的模块之后添加一个聚合。

在场景中，您将看到来自的任意区段周围的阴影 **起始迭代器** 到 **结束汇总**. 这有助于在Workfront Fusion场景中轻松发现这些区段。

## 轮到你了

>[!NOTE]
>
>练习和挑战是可选的，不是完成Fusion培训所必需的。

此练习练习基于您在演练中所学到的内容，但未提供解决方案。

创建一个新方案，以合计营销项目组合中项目的所有登录任务小时。 然后，发送一封电子邮件，说明“您的{Project Name}项目团队记录了总计{planned hours}计划小时数中的{summed hours}，使您处于计划的{percentage}。”

**挑战：** 查看您是否可以执行相同的操作，但只能针对今年记录的小时数。

## 想要了解更多信息？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
