---
title: 了解 [!UICONTROL Business Case]
description: 了解如何使用 [!UICONTROL Business Case] Workfront以评估请求的项目，并将它们与您项目组合中的其他项目进行比较。
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: introduction-to-the-business-case.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13836
role: User
level: Intermediate
exl-id: febb7378-81d4-4348-ac57-e9c4756966c0
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# 了解 [!UICONTROL Business Case]

作为经理，您的目标是确保项目以积极的方式为公司的总体目标和计划做出贡献。 为了做出明智的决策，您需要项目经理提供信息，告知他们推进项目将需要什么。 这可以通过以下方式实现 [!UICONTROL Business Case].

## 什么是 [!UICONTROL Business Case]？

想一想 [!UICONTROL Business Case] 作为需要完成的工作的蓝图或提议。 它捕获帮助您规划和管理项目组合的概要性初步估计。 在这里，可以输入潜在支出、资源和风险，以构建该项目让公司受益的“案例”。

## [!UICONTROL Business Case] 建议用于项目优先级的字段

每个部分 [!UICONTROL Business Case] 提供有关项目的独特重要信息。 让我们看一下将信息馈送到的部分 [!UICONTROL Portfolio Optimizer] 工具，这将帮助您确定项目组合中的项目的优先级。

## [!UICONTROL Project Info]

大多数的信息输入于 [!UICONTROL Project Info] 部分涉及一般项目详细信息，如项目发起人和项目所属的程序。

但是，有一个信息可能会影响项目的优先顺序 — [!UICONTROL Planned Benefit].

![的图像 [!UICONTROL Planned Benefit] 中的区域 [!UICONTROL Project Info] 的部分 [!UICONTROL Business Case]](assets/05-portfolio-management4.png)

此 [!UICONTROL Planned Benefit] 表示如果项目完成，贵公司可能从中受益的预计美元金额。

这是部分内容之一，对于让您的公司推进此项目而言，这可能是一个转折点。 如果能证明该项目将对贵公司的盈利水平产生重大影响，那么该项目被更快地推进的几率就更高。

## [!UICONTROL Expenses]

[!UICONTROL Expenses] 指项目期限内可能产生的非劳动成本。

![的图像 [!UICONTROL Expenses] 中的部分 [!UICONTROL Business Case]](assets/06-portfolio-management5.png)

例如，用户会议的费用可能包括地点付款、礼品包物品或地点大厅的标志。

## [!UICONTROL Resource Budgeting]

此 [!UICONTROL Resource Budgeting] 部分允许您估计项目前进所需的人力。 信息提取自 [!DNL Workfront's] [!UICONTROL Resource Planner].

![的图像 [!UICONTROL Resource Budgeting] 中的部分 [!UICONTROL Business Case]](assets/07-portfolio-management6.png)

通过输入每个工作角色的估计需求，这会创建项目可能需要的预算，并深入分析项目组合有多少预算可用于项目。

>[!NOTE]
>
>您必须在中设置资源池 [!DNL Workfront] 要使用的 [!UICONTROL Business Case].

## [!UICONTROL Risks]

您始终对项目的顺利运行抱着最高的希望。 但识别风险并据此制定计划很重要。 这就是 [!UICONTROL Risks] 中的部分 [!UICONTROL Business Case] 会有所帮助。

![的图像 [!UICONTROL Risks] 中的部分 [!UICONTROL Business Case]](assets/08-portfolio-management7.png)

您应该与团队集思广益，确定项目存在的任何风险。 对于可以估计发生风险时的成本以及发生风险的可能性，请确保并输入这些值。 Workfront会将潜在成本乘以概率，并将之用于 [!UICONTROL Potential Risk] 从项目投资中扣除的基金 [!UICONTROL Planned Benefit] 在计算其 [!UICONTROL Net Value].

## [!UICONTROL Scorecards]

[!UICONTROL Scorecards] 帮助确定所提议的项目与为项目组合或公司设定的总体目标和计划的匹配程度。

每个记分卡都有一个问题列表，其中包含附加值的问题和答案。 当记分卡填写完毕后， [!DNL Workfront] 可以计算项目与您组织预先确定的目标的对齐情况。

![的图像 [!UICONTROL Scorecards] 中的部分 [!UICONTROL Business Case]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>项目经理将无法看到分配给每个答案的值。 只有创建记分卡的用户才能看到值。

## [!UICONTROL Business Case] 非必填

此 [!UICONTROL Business Case] 非常灵活。 您可以只填写几个部分或根本不填写任何部分。 这些字段都不是必填字段。 但是，您填写的信息越多，就越容易分析和优先处理争夺相同预算或资源的项目。

一旦 [!UICONTROL Business Case] 已填写，请单击 **[!UICONTROL Submit]** 窗口右侧“摘要”面板中的按钮。 这会将项目状态更改为 [!UICONTROL Requested]. 现在您已准备好使用 [!UICONTROL Portfolio Optimization] 优先处理同一项目组合中的项目。

>[!NOTE]
>
>中的对齐分数 [!UICONTROL Business Case] 填写记分卡时，会生成摘要面板。 对齐分数是计算中使用的值之一 [!UICONTROL Portfolio Optimizer] 分数。

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
