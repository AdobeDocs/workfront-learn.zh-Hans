---
title: 了解 [!UICONTROL Business Case]
description: 了解如何使用 Workfront 中的 [!UICONTROL Business Case] 来评估请求的项目，并将其与您项目组合中的其他项目进行比较。
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
ht-degree: 100%

---

# 了解 [!UICONTROL Business Case]

作为一名管理者，您的目标是确保项目以积极的方式为公司的总体目标和举措做出贡献。若要作出明智的决策，您需要项目经理提供有关他们推进其项目所需的信息。这可以通过 [!UICONTROL Business Case] 来完成。

## 什么是 [!UICONTROL Business Case]？

将 [!UICONTROL Business Case] 视为需要完成的工作的 Blueprint 或建议。它捕获的是概括的初步估计值，有助于您规划和管理项目组合。在这里输入潜在的费用、资源和风险，以构建一个“案例”来说明为什么该项目可使公司受益。

## 推荐用于项目优先级排序的 [!UICONTROL Business Case] 字段

[!UICONTROL Business Case] 的每一部分都提供了有关该项目的独特而重要的信息。让我们来看看向 [!UICONTROL Portfolio Optimizer] 工具提供信息的部分，该工具将会帮助您确定您项目组合中的项目的优先级。

## [!UICONTROL Project Info]

在 [!UICONTROL Project Info] 部分输入的大多数信息都涉及项目的一般细节，例如项目赞助者和项目所属的项目群。

然而，有一条信息可能会影响项目的优先级——[!UICONTROL Planned Benefit]。

![图像：[!UICONTROL Project Info] 部分中的 [!UICONTROL Planned Benefit] 区域，位于 [!UICONTROL Business Case]](assets/05-portfolio-management4.png)

[!UICONTROL Planned Benefit] 表示如果项目完成，您的公司可能会从中受益的估计美元金额。

这可能会是促使公司推进该项目的转折点的部分之一。如果您能够验证该项目将会为您公司的盈利做出重大贡献，那么该项目更有可能会加快通过速度。

## [!UICONTROL Expenses]

[!UICONTROL Expenses] 代表一个项目的生命周期内可能产生的非劳动力成本。

![图像：[!UICONTROL Expenses] 部分，位于 [!UICONTROL Business Case]](assets/06-portfolio-management5.png)

例如，用户会议的费用可能包括场地费用、礼品袋项目或场地大厅标志。

## [!UICONTROL Resource Budgeting]

[!UICONTROL Resource Budgeting] 部分允许您估计您认为推进项目所需的劳动力。信息从 [!DNL Workfront's] [!UICONTROL Resource Planner] 中提取。

![图像：[!UICONTROL Resource Budgeting] 部分，位于 [!UICONTROL Business Case]](assets/07-portfolio-management6.png)

通过输入每个工作角色的估计需求，这可以创建项目所需的潜在预算，并深入了解项目组合的预算中有多少可用于该项目。

>[!NOTE]
>
>您必须在 [!DNL Workfront] 中设置资源池才能使用 [!UICONTROL Business Case] 中的该部分。

## [!UICONTROL Risks]

您总是抱着最大的希望，希望您的项目能顺利进行。但识别风险并相应地制定计划非常重要。这就是 [!UICONTROL Business Case] 中的 [!UICONTROL Risks] 部分可以提供帮助的地方。

![图像：[!UICONTROL Risks] 部分，位于 [!UICONTROL Business Case]](assets/08-portfolio-management7.png)

您应该和您的团队一起集思广益，找出项目面临的任何风险。对于可以估计发生时所产生的成本以及发生概率的风险，请一定要输入这些值。Workfront 会将潜在的成本乘以概率，并将其放入 [!UICONTROL Potential Risk] 资金中，在计算其 [!UICONTROL Net Value] 时，会将该资金从项目的 [!UICONTROL Planned Benefit] 中减去。

## [!UICONTROL Scorecards]

[!UICONTROL Scorecards] 有助于确定拟议项目与项目组合或公司的总体目标和举措的一致性。

每个记分卡都有一个问题和答案列表，这些问题和答案都附有值。填写记分卡后，[!DNL Workfront] 可以计算该项目与组织预定目标之间的一致性。

![图像：[!UICONTROL Scorecards] 部分，位于 [!UICONTROL Business Case]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>项目经理将无法看到分配给每个答案的值。只有创建记分卡的用户才能看到这些值。

## [!UICONTROL Business Case] 不是必需的

[!UICONTROL Business Case] 是灵活的。您可以只填写几个部分，也可以不填写。没有任何字段是必填的。但是，您填写的信息越多，就越容易分析和确定争夺相同预算或资源的项目的优先级。

填写 [!UICONTROL Business Case] 后，单击窗口右侧摘要面板中的 **[!UICONTROL Submit]** 按钮。这会将项目状态更改为 [!UICONTROL Requested]。现在，您可以使用 [!UICONTROL Portfolio Optimization] 对同一项目组合中的项目进行优先级排序了。

>[!NOTE]
>
>填写记分卡时，会生成 [!UICONTROL Business Case] 摘要面板中的一致性分数。一致性分数是计算 [!UICONTROL Portfolio Optimizer] 分数时使用的值之一。

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
