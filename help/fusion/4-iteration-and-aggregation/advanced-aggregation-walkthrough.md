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
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '278'
ht-degree: 100%

---

# 高级聚合演练

调用网络服务返回多个国家/地区的详细信息，并确定所有国家/地区的总人口（按子区域分组）。

![Fusion 场景的图像](assets/iteration-and-aggregation-3.png)

## 高级聚合演练

Workfront 建议先观看练习演练视频，然后再尝试在您自己的环境中重新创建练习。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 练习 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>有关完成该演练的分步说明，请参阅[高级聚合演练](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=zh-Hans)练习。

## 强化聚合原则

每当一个模块输出多个捆绑包时，之后的每个模块都会执行每个捆绑包。

为了防止这种情况，请在可能产生多个捆绑包的模块后面添加一个聚合器。

在您的场景中，从&#x200B;**开始的迭代器**&#x200B;到&#x200B;**结束的聚合器**，您将会看到一个阴影围绕着所有区段。这有助于在您的 Workfront Fusion 场景中轻松发现这些区段。

## 到您了

>[!NOTE]
>
>练习和挑战是可选的，并不是完成 Fusion 培训所必需的。

本练习以您在演练中学到的内容为基础，但未提供解决方案。

创建一个新场景来汇总营销项目组合中的项目内已记录任务的所有小时数。然后发送一封电子邮件，其中写明“您的 {Project Name} 项目团队的总规划小时数为 {planned hours}，现已记录 {summed hours}，达到计划的 {percentage}”。

**挑战：**&#x200B;看看您是否可以进行同样的操作，但仅限今年记录的小时数。

## 想要了解详情？我们建议查看以下内容：

[Workfront Fusion 文档](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hans)
