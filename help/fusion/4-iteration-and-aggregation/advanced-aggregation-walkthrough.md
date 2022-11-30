---
title: 高级聚合演练
description: 了解如何调用Web服务以返回有关多个国家/地区的详细信息并识别按子区域分组的人口，所有这些均位于 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: 0618bf27478744e0e9976015a24c5ec8519efbb7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 高级聚合演练

## 概述

请致电Web服务，以返回有关多个国家/地区的详细信息，并确定按子区域分组的所有国家/地区的总人口。

![融合场景的图像](assets/iteration-and-aggregation-3.png)

## 高级聚合演练

Workfront建议先观看练习视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## 练习URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>有关完成演练的分步说明，请转到 [高级聚合演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 练习。

## 聚合原理的强化

每当模块输出多个包时，每个模块在输出后都将执行每个包。

要防止出现这种情况，请在可能会生成多个包的模块之后添加聚合器。

在您的方案中，您将看到 **初迭代器** 到 **结束聚合器**. 这有助于在Workfront Fusion场景中轻松发现这些区段。

## 该你了

>[!NOTE]
>
>实践练习和挑战是可选的，完成融合培训并非必需的。

此练习以您在演练中学到的内容为基础，但未提供解决方案。

创建一个新方案，以汇总营销组合中项目中已登录任务的所有小时数。 然后发送一封电子邮件，说明“您的{项目名称}项目团队已记录{计划时数}总计划时数的{总和时数}，使您达到计划的{百分比}。”

**挑战：** 查看您是否可以执行相同的操作，但仅在今年记录的小时内。

## 想了解更多吗？ 我们建议执行以下操作：

[Workfront Fusion文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
