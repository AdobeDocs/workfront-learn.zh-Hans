---
title: 创建带有图表的报表
description: 了解图表如何改进数据可视化，以及如何在Workfront中使用图表工具。
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 创建带有图表的报表

在本视频中，您将了解：

* 图表如何改进数据可视化
* 如何使用Workfront的图表工具

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## 活动：向报表中添加图表

本季度末期即将到来，您希望了解最近完成的项目是如何遵守其预算的。 创建一个显示项目计划成本与实际成本的报告。 您只想查看在上季度完成的项目。 使用自定义颜色添加组合柱状图。

## 答案

1. 选择 **[!UICONTROL Reports]** 从 **[!UICONTROL Main Menu]**.
1. 单击 **[!UICONTROL New Report]** 菜单并选择 **[!UICONTROL Project]**.
1. 在 **[!UICONTROL Columns (View)]** 选项卡，单击 **[!UICONTROL Add Column]**.
1. 选择 [!UICONTROL Project] > [!UICONTROL Planned Cost] 并按以下方式总结此列 **[!UICONTROL Sum]**.
1. 单击 **[!UICONTROL Add Column]** 再来一次。
1. 选择 [!UICONTROL Project] > [!UICONTROL Actual Cost] 并按以下方式总结此列 **[!UICONTROL Sum]**.

   ![用于向报表添加列的屏幕图像](assets/chart-report-columns.png)

1. 在 **[!UICONTROL Groupings]** 选项卡，将报表设置为分组依据 [!UICONTROL Project] > [!UICONTROL Name].

   ![向报表添加分组的屏幕图像](assets/chart-report-groupings.png)

1. 在 **[!UICONTROL Filters]** 选项卡，添加两个筛选规则：

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Complete]
   * [!UICONTROL Project] >[!UICONTROL  Actual Completion Date] > [!UICONTROL Last Quarter]

   ![用于将过滤器添加到报表的屏幕图像](assets/chart-report-filters.png)

1. 在 **[!UICONTROL Chart]** 选项卡，选择 **[!UICONTROL Column]** 图表类型。
1. 对于 [!UICONTROL Left (Y) Axis]，选择 [!UICONTROL Project] > [!UICONTROL Planned Cost].
1. 对于 [!UICONTROL Bottom (X) Axis]，选择 [!UICONTROL Project] > [!UICONTROL Name].
1. 单击 **[!UICONTROL Combination Chart]** 按钮并选择 [!UICONTROL Project] > [!UICONTROL Actual Cost] 在 **[!UICONTROL Value]** 字段。
1. 单击颜色框旁边的箭头以更改 [!UICONTROL Actual Cost] 颜色。 选择显示的颜色之一，或单击右下角的框以调出调色板。
1. 单击 **[!UICONTROL Save + Close]**. 当系统提示您输入报表名称时，请将其称为“按上一季度完成的项目列出的计划成本与实际成本”。

   ![向报表中添加图表的屏幕图像](assets/chart-report-chart.png)
