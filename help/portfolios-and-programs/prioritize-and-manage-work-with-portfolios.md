---
title: 使用 [!UICONTROL Portfolio Optimizer] 确定工作的优先顺序并对其进行管理
description: 了解如何使用 [!UICONTROL Portfolio Optimizer] 对项目组合中的项目进行优先排序和管理。
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
workflow-type: ht
source-wordcount: '808'
ht-degree: 100%

---

# 使用 [!UICONTROL Portfolio Optimizer] 确定工作的优先顺序并对其进行管理

在 [!UICONTROL Business Case] 中为您项目组合中的每个项目输入的信息会汇总到项目组合中，并会进入 [!UICONTROL Portfolio Optimization] 部分的标题中。

![[!UICONTROL Portfolio Optimizer] 区域的图像，其中的信息来自于 [!UICONTROL Business Case]](assets/10-portfolio-management9.png)

现在让我们利用这些信息来分析哪些项目应该快速投入生产，哪些项目可以在下一轮之前留在旁边。[!UICONTROL Portfolio Optimization] 工具可以极大地帮助实现这一点。

[!UICONTROL Portfolio Optimizer] 可以在以下情况下为您提供最全面的帮助：

* 所有项目的 [!UICONTROL Business Case] 均已完成并提交。
* 单击 [!UICONTROL Business Case] 中的 [!UICONTROL Submit] 按钮，Workfront 将会计算项目的分数。
* 您可以提供一个预算来表示所选项目的总体财务上限。

## 优化标准

[!UICONTROL Portfolio Optimizer] 使用一套标准的衡量条件来比较和确定项目的优先级。

这些标准是：

* 低成本
* 高度一致性
* 高价值
* 低风险收益比
* 高 ROI

单击“优化”图标将会打开一组滑块，其中的每个滑块都与一个标准相关联。您可以通过向右移动滑块来设置具有较高优先级的标准，或者通过向左推动滑块来设置具有较低优先级的标准。

![[!UICONTROL Portfolio Optimizer] 区域的图像，其中的信息来自于 [!UICONTROL Business Case]](assets/11-portfolio-management10.png)

使用这些标准，[!DNL Workfront] 会生成 1 到 100 之间的项目分数。数字较高的项目表明它们更符合您希望项目组合发展的方向。

![[!UICONTROL Portfolio Optimizer] 区域的图像，其中显示有项目分数信息](assets/12-portfolio-management14.png)

>[!NOTE]
>
>即使填写了 [!UICONTROL Business Case] 的所有部分，[!UICONTROL Portfolio Optimizer] 也不会对项目进行评分，除非 [!UICONTROL Business Case] 已通过 [!DNL Workfront] 提交给了项目组合。您在 [!UICONTROL Portfolio Optimizer] 的 [!UICONTROL Score] 列中看到的不是分数，而是警告符号。将鼠标悬停在警告符号上可查看有关项目评分的更多信息。

![[!UICONTROL Portfolio Optimizer] 的 [!UICONTROL Score] 列中的警告符号的图像。](assets/13-portfolio-management12.png)

## 确定项目的优先顺序

现在项目已获得评分，您就可以快速轻松地重新组织列表。

通过单击 [!UICONTROL Score] 列的标题，项目会重新排序，并且会按从最高分到最低分或从最低分到最高分的顺序列出。您可以通过单击数字左侧的条形图标并按照您想要的顺序放置项目来手动对项目进行排序。

您的清单上可能有您不想比较的项目。如果您不想在列表中看到这些项目，请首先取消选择它们，然后通过向右滑动切换按钮来隐藏它们，此时该按钮的背景为蓝色。如果您想包含这些项目，请将切换按钮滑动到左侧，以显示灰色。

![[!UICONTROL Portfolio Optimizer] 中未选定项目的图像。](assets/14-portfolio-management13.png)

这样您就可以只看到您想要进行比较的项目。通过对项目进行评分、过滤和排序，您现在可以就是否需要更改项目优先级排序标准作出明智的决策。

请记住，[!DNL Workfront] 构建了项目组合和优化工具，以顺利安排项目的优先顺序。但是，您不是必须使用建议的标准。如果该工具所做的只是为您提供一个良好的开端或工作基础，那也没关系。

但是，如果项目已按优先级排序，并且您已准备好在 [!DNL Workfront] 中最终确定其优先级，请单击左上角的 **[!UICONTROL Set Priority]** 按钮，然后系统将会从 1 开始对项目进行编号，并会使用该编号在每个项目中设置 [!UICONTROL Portfolio Priority] 字段。

要保留这些数字，请确保单击底部的 **[!UICONTROL Save]** 按钮。

![使用 [!UICONTROL Set Priority] 按钮对 [!UICONTROL Portfolio Optimizer] 中的项目进行优先级排序的图像。](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* 您可以显示通过 [!UICONTROL Resource Planner] 中的 [!UICONTROL Portfolio Optimizer] 设置的项目优先级。单击 **[!UICONTROL Settings]** 图标并开启 **[!UICONTROL Display Portfolio Priorities]** 选项。屏幕会刷新并在左侧栏中显示项目组合的优先级。单击列顶部的 **[!UICONTROL Order]** 选项，将 [!UICONTROL Resource Planner] 优先级与项目组合优先级对齐。完成后请务必保存。

  ![[!UICONTROL Resource Planner] 中 [!UICONTROL Portfolio Priorities] 列的图像。](assets/16-portfolio-management17.png)

## 管理更改

项目组合当然不是万能的，但它们可以缓解转变优先事项的痛苦。以前需要几天时间完成的工作现在可能只需要几个小时甚至几分钟。

当新项目添加到项目组合中时，仍然需要对其进行分析和优先级排序。通过使用 [!UICONTROL Business Case] 和优化分数，您可以毫不费力地将新项目与请求的、规划的和当前的项目进行比较。

![[!UICONTROL Portfolio Optimizer] 中的项目 [!UICONTROL Status] 列的图像。](assets/17-project-management16.png)

如果在比较过程中，您发现新项目应该具有更高的优先级，您可以根据优化分数重新对列表进行排序，或者将它们拖放到列表中更高的位置。完成后，只需单击 **[!UICONTROL Set Priority]** 按钮，进行保存，您的工作就完成了。

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
