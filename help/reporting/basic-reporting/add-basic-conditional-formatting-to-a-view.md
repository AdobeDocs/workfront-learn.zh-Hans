---
title: 添加基本条件格式
description: 了解如何使用列规则，根据您设置的条件，更改报表或视图中的文本颜色、格式设置和背景颜色。
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 0ee80dceb8208bd0360fd8c9ab68fb8a73677a9d
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 向视图添加基本条件格式

条件格式是通过创建列规则来完成的。 列规则允许您根据您设置的条件以特定方式格式化列。

在本视频中，您将了解：

* 视图中的条件格式是什么
* 如何创建和修改条件格式

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## 摘要

要创建条件格式，请执行以下操作：

1. 选择要显示格式设置的列
1. 决定您希望更改格式的条件
1. 确定哪种格式更改效果最佳

   * 背景颜色
   * 文本颜色
   * 替换文本
   * 显示图标

## 活动：向视图添加条件格式

使用现有的标准视图并将此条件格式添加到上，创建一个名为“标准+进度”的任务视图 [!UICONTROL Name] 列。

1. 添加列规则，当任务的进度状态为“延迟”时，该规则会将字段背景变为红色。
1. 添加一个列规则，当进度状态为“落后”或“有风险”时，该规则将使字段背景变为黄色。

这有助于您识别有问题的任务，而无需在视图中包括进度状态列。

## 答案

![用于创建新列规则的屏幕图像](assets/conditional-formatting-exercise.png)

1. 在任务列表报告中，转到 **[!UICONTROL View]** 下拉菜单并选择 **[!UICONTROL New View]**.
1. 将视图命名为“Standard + Progress”。
1. 使用提供的默认列。
1. 选择 [!UICONTROL Task Name] 列。 这是要将条件格式应用于的列，因此，如果任务的进度状态不是“按时”，它将显示为红色或黄色。
1. 单击 **[!UICONTROL Advanced Options]** Report Builder窗口的右上角。
1. 单击 **[!UICONTROL Add a Rule for this Column]**.
1. 通过更改启动列规则 [!UICONTROL Task] > [!UICONTROL Name] 窗口顶部的 [!UICONTROL Task] > [!UICONTROL Progress Status]. 只需单击 **[!UICONTROL X]** 图标旁边 [!UICONTROL Task] > [!UICONTROL Name] 以将其从字段中删除。
1. 在字段中键入“progress”，然后选择 [!UICONTROL Progress Status] 在 [!UICONTROL Task] 字段源。
1. 选择 **[!UICONTROL Late]** 在右侧的字段中 [!UICONTROL Equal] 限定符。
1. 选择红色背景 [!UICONTROL Text Color] row。
1. 单击 **[!UICONTROL Add Rule]** 以保存列规则。
1. 现在，单击 **[!UICONTROL Add Column Rule]** 以添加其他规则。
1. 就像之前一样，删除 [!UICONTROL Task] > [!UICONTROL Name] 从“标准”字段中。 替换为 [!UICONTROL Progress Status] 在 [!UICONTROL Task] 字段源。
1. 选择两者 [!UICONTROL At Risk] 和 [!UICONTROL Behind] 在“相等”限定符右侧的字段中。
1. 选择黄色背景 [!UICONTROL Text Color] row。
1. 单击 **[!UICONTROL Add Rule]** 以保存列规则。
1. 单击 **[!UICONTROL Save View]** 以保存视图。
