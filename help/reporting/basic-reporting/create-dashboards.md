---
title: 创建仪表板
description: 该视频旨在帮助用户在Workfront中有效创建、自定义和管理功能板，以监控和共享与项目相关的数据。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
exl-id: 7adc2aeb-6618-4894-acc3-298e35175854
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 62%

---

# 创建仪表板

本视频涵盖以下要点：

* **功能板简介：**&#x200B;说明Workfront中的功能板及其作为相关报表集合的目的。&#x200B;AEM
* **创建仪表板：**&#x200B;有关如何通过导航到“仪表板”区域、选择“新仪表板”、命名它并选择布局来创建新仪表板的指南。&#x200B;AEM
* **添加报告：**&#x200B;演示如何将各种报告（如项目报告、任务报告和问题报告）添加到功能板，并在所选布局中排列它们。&#x200B;AEM
* **自定义视图：**&#x200B;显示如何通过编辑报告并选择要显示的特定列，自定义在仪表板视图中显示哪些列。&#x200B;AEM
* **添加其他元素：**&#x200B;说明如何将自定义日历和外部页面（例如，联机文档）添加到仪表板。&#x200B;AEM
* **保存和固定：**&#x200B;有关保存仪表板并将其固定以便轻松访问的说明。&#x200B;AEM
* **查看和编辑：**&#x200B;提供有关查看和编辑仪表板的提示，包括调整列可见性以便更好地显示。&#x200B;AEM
* **查找和共享功能板：**&#x200B;介绍如何通过主菜单查找功能板、将其添加到收藏夹并与其他用户共享。&#x200B;AEM
* **打印仪表板：**&#x200B;说明打印仪表板的过程。&#x200B;AEM


>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on)


## “创建功能板”活动

### 活动 1：创建一个仪表板

创建一个只有一个报告的 [!UICONTROL dashboard]——“搜索该项目中的注释。”这对于快速查找项目上的任何更新非常有用，即使有数千条更新内容需要搜索也是如此。这将会搜索更新跟帖内容，以快速提取能够满足您在提示中指定的条件的任何更新。

通过复制您在“创建注释报告”活动中创建的“搜索注释”报告来创建此报告（如果您没有进行该活动，请使用其他报告）。

* 从副本中删除“项目名称”提示，并将报告重命名为“搜索该报告中的注释”。
* 将 [!UICONTROL Dashboard] 命名为“搜索注释。”
* 转到任何项目登陆页面，并为 [!UICONTROL dashboard] 创建一个自定义部分。
* 请注意，当您在自定义部分中搜索注释时，它只会显示您当前所在项目中包含的注释。

### 答案 1

1. 运行您在“创建注释报告”活动中创建的报告。
1. 单击 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Copy]**。[!DNL Workfront] 会创建一个名为“注释搜索（副本）”的新报告。
1. 前往 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Edit]**。单击 **[!UICONTROL Report Settings]** 并将名称更改为“搜索该项目中的注释。”
1. 单击 [!UICONTROL Report Prompts] 并从列表中删除 [!UICONTROL Project] > [!UICONTROL Name] 提示。

   ![创建新仪表板的屏幕图像](assets/edit-report-prompts.png)

1. 选中 **[!UICONTROL Show Prompts in Dashboard]** 框。
1. 单击 **[!UICONTROL Done]**，然后单击 **[!UICONTROL Save + Close]**。您现在会看到报告的 [!UICONTROL Prompts] 屏幕。

   接下来，您要使用快捷方式创建一个新仪表板，并向其中添加该报告。

1. 单击 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Add to Dashboard]** > **[!UICONTROL New Dashboard]**。
1. 将报告“在该项目中搜索”拖至 **[!UICONTROL Layout]** 面板。
1. 请注意，报告的名称将会成为仪表板的名称。将名称编辑为“搜索注释”。

   ![创建新仪表板的屏幕图像](assets/create-dashboard.png)

1. 单击 **[!UICONTROL Save + Close]**。

   现在将仪表板添加到项目页面。

   ![创建新仪表板的屏幕图像](assets/add-custom-section.png)

1. 转到任何项目。从左侧面板菜单中，单击 **[!UICONTROL Add custom section]** 图标。
1. 在 **[!UICONTROL Add a Dashboard]** 字段中，输入“搜索注释”，并从列表中选择 [!UICONTROL dashboard]。
1. 在 **[!UICONTROL Custom section title]** 字段中，输入“搜索注释”。
1. 单击 **[!UICONTROL Add new section]**。
1. 从左侧面板菜单中，找到“搜索注释”。单击该部分名称左侧的点，并将其拖至“更新”下方。
