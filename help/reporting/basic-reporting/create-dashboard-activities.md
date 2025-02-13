---
title: 创建功能板活动
description: 按照分步说明，练习创建功能板。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 46%

---

# 创建功能板活动

按照分步说明，练习创建功能板。

## 活动1：创建功能板

创建一个仅包含一个报告的[!UICONTROL dashboard] — “在此项目中搜索注释”。 这对于快速查找项目上的任何更新非常有用，即使有数千条更新内容需要搜索也是如此。这将会搜索更新跟帖内容，以快速提取能够满足您在提示中指定的条件的任何更新。

通过复制您在“创建备注报告”活动中创建的“搜索备注”报告来创建此报告(或者使用其他报告（如果未执行该活动）。

* 从副本中删除“项目名称”提示并将报告重命名为“在此项目中搜索注释”。
* 将[!UICONTROL Dashboard]命名为“搜索备注”。
* 转到任何项目登陆页面，并为 [!UICONTROL dashboard] 创建一个自定义部分。
* 请注意，在自定义分区中搜索注释时，它将只显示您当前所在项目中包含的注释。

## 答案1

1. 运行您在“创建注释报告”活动中创建的报告。
1. 单击 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Copy]**。[!DNL Workfront]创建一个名为“注释搜索（复制）”的新报告。
1. 前往 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Edit]**。单击&#x200B;**[!UICONTROL Report Settings]**&#x200B;并将名称更改为“在此项目中搜索注释”。
1. 单击 [!UICONTROL Report Prompts] 并从列表中删除 [!UICONTROL Project] > [!UICONTROL Name] 提示。

   ![创建新仪表板的屏幕图像](assets/edit-report-prompts.png)

1. 选中 **[!UICONTROL Show Prompts in Dashboard]** 框。
1. 单击 **[!UICONTROL Done]**，然后单击 **[!UICONTROL Save + Close]**。您现在会看到报告的 [!UICONTROL Prompts] 屏幕。

   接下来，您将使用快捷方式创建新功能板并将此报表添加到其中。

1. 单击 **[!UICONTROL Report Actions]** 并选择 **[!UICONTROL Add to Dashboard]** > **[!UICONTROL New Dashboard]**。
1. 将报告“在此项目中搜索注释”拖到&#x200B;**[!UICONTROL Layout]**&#x200B;面板。
1. 请注意，报告的名称将会成为仪表板的名称。将名称编辑为只是“Search Notes”。

   ![创建新仪表板的屏幕图像](assets/create-dashboard.png)

1. 单击 **[!UICONTROL Save + Close]**。

   现在将仪表板添加到项目页面。

   ![创建新仪表板的屏幕图像](assets/add-custom-section.png)

1. 转到任何项目。从左侧面板菜单中，单击 **[!UICONTROL Add custom section]** 图标。
1. 在&#x200B;**[!UICONTROL Add a Dashboard]**&#x200B;字段中，键入“搜索注释”并从列表中选择[!UICONTROL dashboard]。
1. 在&#x200B;**[!UICONTROL Custom section title]**&#x200B;字段中，键入“搜索备注”。
1. 单击 **[!UICONTROL Add new section]**。
1. 从左侧面板菜单中，找到“搜索注释”。单击该部分名称左侧的点，并将其拖至“更新”下方。
