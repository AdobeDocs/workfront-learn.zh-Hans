---
title: 创建带有图表的报告
description: 了解图表如何提升数据的可视化，以及如何使用 Workfront 中的图表工具。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: ht
source-wordcount: '285'
ht-degree: 100%

---

# 创建带有图表的报告

在本视频中，您将了解到：

* 图表如何改善数据的可视化
* 如何使用 Workfront 的图表工具

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## 创建带有图表活动的报告

[单击此处](/help/assets/create-reports-with-charts-activities.pdf)下载此页面的 PDF。

### 活动 1：将图表添加到报告中

本季度即将结束，您想看看最近完成的项目是否符合预算。创建一份报告，其中显示项目的规划成本与实际成本。您只想查看上一季度完成的项目。使用自定义颜色添加组合柱形图。

### 答案 1

1. 从 **[!UICONTROL Main Menu]** 中选择 **[!UICONTROL Reports]**。
1. 单击 **[!UICONTROL New Report]** 菜单并选择 **[!UICONTROL Project]**。
1. 在 **[!UICONTROL Columns (View)]** 选项卡中，单击 **[!UICONTROL Add Column]**。
1. 选择 [!UICONTROL Project] > [!UICONTROL Planned Cost]，并按 **[!UICONTROL Sum]** 对本列进行汇总。
1. 再次单击 **[!UICONTROL Add Column]**。
1. 选择 [!UICONTROL Project] > [!UICONTROL Actual Cost]，并按 **[!UICONTROL Sum]** 对本列进行汇总。

   ![在报告中添加列的屏幕图像](assets/chart-report-columns.png)

1. 在 **[!UICONTROL Groupings]** 选项卡中，将报告设置为根据 [!UICONTROL Project] > [!UICONTROL Name] 分组。

   ![在报告中添加分组的屏幕图像](assets/chart-report-groupings.png)

1. 在 **[!UICONTROL Filters]** 选项卡中，添加两条过滤规则：

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Complete]
   * [!UICONTROL Project] >[!UICONTROL  Actual Completion Date] > [!UICONTROL Last Quarter]

   ![在报告中添加过滤器的屏幕图像](assets/chart-report-filters.png)

1. 在 **[!UICONTROL Chart]** 选项卡中，为图表类型选择 **[!UICONTROL Column]**。
1. 对于 [!UICONTROL Left (Y) Axis]，选择 [!UICONTROL Project] > [!UICONTROL Planned Cost]。
1. 对于 [!UICONTROL Bottom (X) Axis]，选择 [!UICONTROL Project] > [!UICONTROL Name]。
1. 单击 **[!UICONTROL Combination Chart]** 按钮，并选择 **[!UICONTROL Value]** 字段中的 [!UICONTROL Project] > [!UICONTROL Actual Cost]。
1. 单击颜色框旁边的箭头可更改 [!UICONTROL Actual Cost] 颜色。选择出现的颜色之一或单击右下角的框以调出调色板。
1. 单击&#x200B;**[!UICONTROL Save + Close]**。当系统提示输入报告名称时，将其命名为“上季度完成项目的规划成本与实际成本”。

   ![在报告中添加图表的屏幕图像](assets/chart-report-chart.png)
