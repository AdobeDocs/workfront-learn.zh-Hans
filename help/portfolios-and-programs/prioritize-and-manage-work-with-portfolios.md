---
title: 使用 [!UICONTROL Portfolio Optimizer] 优先处理和管理工作
description: 了解如何使用 [!UICONTROL Portfolio Optimizer] 优先处理和管理项目组合中的项目。
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: prioritize-and-manage-work-with-portfolios.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13835
role: User
level: Intermediate
exl-id: b8b91ae8-f0e1-4cab-bf2c-6b8ca9746ea3
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# 使用 [!UICONTROL Portfolio Optimizer] 优先处理和管理工作

输入的信息 [!UICONTROL Business Case] 对于您的项目组合中的每个项目，会汇总到项目组合和 [!UICONTROL Portfolio Optimization] 部分。

![的图像 [!UICONTROL Portfolio Optimizer] 区域，其中包含来自 [!UICONTROL Business Case]](assets/10-portfolio-management9.png)

现在该利用这些信息来分析哪些项目应该进入生产快车道，哪些项目可以袖手旁观，直到下一轮。 此 [!UICONTROL Portfolio Optimization] 工具会对此大有帮助。

此 [!UICONTROL Portfolio Optimizer] 在以下情况下，可以为您提供全面的帮助：

* 此 [!UICONTROL Business Case] 已完成并提交所有项目。
* 单击 [!UICONTROL Submit] 中的按钮 [!UICONTROL Business Case] 以便Workfront计算项目分数。
* 您提供的预算代表所选项目的总财务上限。

## 优化标准

此 [!UICONTROL Portfolio Optimizer] 使用一组标准标准来比较项目并确定其优先级。

这些标准包括：

* 低成本
* 高度一致性
* 高值
* 收益低风险
* 高 ROI

单击“优化”图标将打开一组滑块条，每个滑块条都与其中一个标准关联。 通过将滑块向右移动，您可以设置哪些标准具有较高优先级，或将滑块向左推送，可设置哪些标准具有较低优先级。

![的图像 [!UICONTROL Portfolio Optimizer] 区域，其中包含来自 [!UICONTROL Business Case]](assets/11-portfolio-management10.png)

使用这些标准， [!DNL Workfront] 生成一个介于1和100之间的项目得分。 数字较大的项目表示它们更好地与您希望项目组合发展的方向保持一致。

![的图像 [!UICONTROL Portfolio Optimizer] 区域包含有关项目得分的信息](assets/12-portfolio-management14.png)

>[!NOTE]
>
>此 [!UICONTROL Portfolio Optimizer] 将不会对项目进行评分，即使项目的所有部分 [!UICONTROL Business Case] 填写，除非 [!UICONTROL Business Case] 已通过提交至项目组合 [!DNL Workfront]. 您会看到 [!UICONTROL Score] 列 [!UICONTROL Portfolio Optimizer]. 将鼠标悬停在警告符号上，可查看有关项目评分的更多信息。

![中警告符号的图像 [!UICONTROL Score] 列 [!UICONTROL Portfolio Optimizer].](assets/13-portfolio-management12.png)

## 排定项目优先级

现在项目已计分，您可以快速轻松地重新组织列表。

通过单击 [!UICONTROL Score] 列标题中，项目将重新排序并从最高分到最低分或从最低分到最高分列出。 您可以通过单击数字左侧的栏图标并按所需的顺序拖放项目来手动对项目排序。

您的列表中可能存在您不想比较的项目。 如果您不想看到列表中的这些按钮，请先取消选择它们，然后通过向右滑动切换开关来隐藏它们，这样按钮的背景为蓝色。 如果要包含这些项目，请将切换开关向左滑动，以便显示灰色。

![中未选定项目的图像 [!UICONTROL Portfolio Optimizer].](assets/14-portfolio-management13.png)

这样，您就可以只查看要相互比较的项目。 在对项目进行评分、筛选和排序后，您现在可以做出明智的决策，决定是否需要更改项目优先排序的标准。

请记住， [!DNL Workfront] 构建了项目组合和优化工具，以顺利地完成项目优先排序过程。 但是，您不必使用建议的标准。 如果所有工具都为您提供良好的开端或工作基础，那就没问题。

但是，如果按照优先级的顺序排列项目，并且您已经准备好在中最终确定优先级 [!DNL Workfront]，单击 **[!UICONTROL Set Priority]** 按钮向上键，系统将从1开始为项目编号，并使用该编号设置 [!UICONTROL Portfolio Priority] 每个项目中的字段。

要保留这些数字，请确保单击 **[!UICONTROL Save]** 按钮。

![使用 [!UICONTROL Set Priority] 按钮，以排定项目在 [!UICONTROL Portfolio Optimizer].](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* 您可以显示项目的优先级，如通过 [!UICONTROL Portfolio Optimizer] 在 [!UICONTROL Resource Planner]. 单击 **[!UICONTROL Settings]** 图标并打开 **[!UICONTROL Display Portfolio Priorities]** 选项。 屏幕会刷新并在左侧栏中显示项目组合优先级。 单击 **[!UICONTROL Order]** 选项，用于对齐列顶部的 [!UICONTROL Resource Planner] 优先级与项目组合优先级。 完成后请务必保存。

  ![的图像 [!UICONTROL Portfolio Priorities] 中的列 [!UICONTROL Resource Planner].](assets/16-portfolio-management17.png)

## 管理更改

Portfolio当然不是万灵丹，但它们可以减轻优先次序变化的痛苦。 以前需要几天时间，现在可能需要几个小时，甚至几分钟。

当新项目添加到项目组合时，仍需要分析它们并确定其优先级。 通过使用 [!UICONTROL Business Case] 以及优化分数，您可以轻松地将新项目与请求、计划和当前项目进行比较。

![项目图像 [!UICONTROL Status] 中的列 [!UICONTROL Portfolio Optimizer].](assets/17-project-management16.png)

如果在比较期间发现新项目应具有更高的优先级，则可以根据优化得分对列表重新排序，或者将它们拖放到列表中的较高位置。 完成后，只需单击 **[!UICONTROL Set Priority]** 按钮，保存，您的工作就完成了。

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
