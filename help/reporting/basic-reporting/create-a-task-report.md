---
title: 创建任务报告
description: 了解如何创建具有复杂过滤器的任务报告以及查找您在 Workfront 中创建的报告。活动 - 创建带有提示的备注报告。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 创建任务报告

在此视频中，您将学习：

* 如何创建具有复杂过滤器的任务报告
* 如何查找您创建的报表

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## 活动：创建带提示的注释报告

创建注释报表，以便根据注释内容、作者、登入日期、项目名称或审核类型搜索用户注释（即注释或更新）或系统注释。 将报表命名为“注释搜索”。

使用“注释文本”提示时，此报表将在更新线程中搜索，以快速提取符合提示中指定条件的任何内容。 运行报表时，您无需填写所有提示，只需填写您关心的提示。 将自动忽略空白的。

视图应包含以下列：

* 注释文本
* 审计文本
* 输入日期
* 所有者：名称
* 审计类型
* 任务名称
* 问题名称

将过滤器选项卡留空。

项目名称组。

包括以下提示：

* 审计文本
* 注释文本
* 所有者名称
* 输入日期
* 项目名称
* 审计类型

## 回答

1. 选择 **[!UICONTROL Reports]** 从 **[!UICONTROL Main Menu]**.
1. 单击 **[!UICONTROL New Report]** 菜单和选择 **[!UICONTROL Note]**.
1. 在 **[!UICONTROL Columns (View)]** 设置要包含的列：

   ![用于创建注释报表列的屏幕图像](assets/note-report-columns.png)

   * [!UICONTROL Note] > [!UICONTROL Note Text]
   * [!UICONTROL Note] > [!UICONTROL Audit Text]
   * [!UICONTROL Note] > [!UICONTROL Entry Date]
   * [!UICONTROL Owner] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Audit Type]
   * [!UICONTROL Task] > [!UICONTROL Name]
   * [!UICONTROL Issue] > [!UICONTROL Name]

1. 选择 **[!UICONTROL Entry Date]** 列，并更改 **[!UICONTROL Sort to Descending]**.
1. 在 **[!UICONTROL Groupings]** 选项卡，将报表设置为按 [!UICONTROL Project] > [!UICONTROL Name].

   ![用于创建注释报表分组的屏幕图像](assets/note-report-groupings.png)

1. 离开 [!UICONTROL Filters] 空白。
1. 打开 **[!UICONTROL Report Settings]** 并将报表命名为“注释搜索”。
1. 在 [!UICONTROL Description] 字段中，输入“根据选定的审核类型和其他提示搜索系统或用户注释”等内容。 系统注释显示在“审核文本”列中，用户注释显示在“注释文本”列中。

   ![用于创建注释报表设置的屏幕图像](assets/note-report-report-options.png)

1. 选择 **[!UICONTROL Details Tab]** 以便在报表加载时显示。
1. 将报表设置为在功能板中包含报表时显示200个项目。
1. 单击 **[!UICONTROL Report Prompts]** 并添加：

   ![用于创建注释报表提示的屏幕图像](assets/note-report-report-prompts.png)

   * [!UICONTROL Note] > [!UICONTROL Audit Text]
   * [!UICONTROL Note] > [!UICONTROL Note Text]
   * [!UICONTROL Owner] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Entry Date]
   * [!UICONTROL Project] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Audit Type]

1. 选中 **[!UICONTROL Show Prompts in Dashboards]**.
1. 保存并关闭您的报表。
