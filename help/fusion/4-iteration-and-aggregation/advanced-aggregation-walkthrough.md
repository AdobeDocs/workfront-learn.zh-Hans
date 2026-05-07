---
title: 高级聚合演练
description: 学习如何调用网络服务返回多个国家/地区的详细信息并确定按子区域分组的人口，一切尽在  [!DNL Adobe Workfront Fusion]。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 84%

---

# 高级聚合演练

调用网络服务返回多个国家/地区的详细信息，并确定所有国家/地区的总人口（按子区域分组）。

![Fusion 场景的图像](assets/iteration-and-aggregation-3.png)

## 高级聚合演练

Workfront 建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## 练习 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## 强化聚合原则

每当一个模块输出多个捆绑包时，之后的每个模块都会执行每个捆绑包。

为了防止这种情况，请在可能产生多个捆绑包的模块后面添加一个聚合器。

在您的场景中，从&#x200B;**开始的迭代器**&#x200B;到&#x200B;**结束的聚合器**，您将会看到一个阴影围绕着所有区段。 这有助于在您的 Workfront Fusion 场景中轻松发现这些区段。

## 到您了

>[!NOTE]
>
>练习和挑战是可选的，并不是完成 Fusion 培训所必需的。

本练习以您在演练中学到的内容为基础，但未提供解决方案。

创建一个新场景来汇总营销项目组合中的项目内已记录任务的所有小时数。 然后，发送一封电子邮件，说明“您的{Project Name}项目团队已记录总共{planned hours}个计划小时数中的{summed hours}，使您处于计划的{percentage}。”

**挑战：**&#x200B;看看您是否可以进行同样的操作，但仅限今年记录的小时数。

## 想要了解详情？ 我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
