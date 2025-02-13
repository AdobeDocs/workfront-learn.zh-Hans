---
title: 向视图活动添加基本条件格式
description: 练习使用分步说明将基本条件格式添加到视图。
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 86%

---

# 向视图活动添加基本条件格式

练习使用分步说明将基本条件格式添加到视图。

## 摘要

要创建条件格式：

1. 选择您想要显示格式的列
1. 确定要更改格式的条件
1. 确定哪种格式更改最有效

   * 背景颜色
   * 文本颜色
   * 替换文本
   * 显示图标

## 活动1：向视图添加条件格式

使用现有的标准视图并在 [!UICONTROL Name] 列上添加此条件格式，创建一个名为“标准+进度”的任务视图。

1. 添加列规则，当任务的进度状态为“延迟”时，该列规则会将字段背景变为红色。
1. 添加列规则，当进度状态为“落后”或“存在风险”时，该列规则会将字段背景变成黄色。

这有助于您发现有问题的任务，而无需将进度状态列包含在视图中。

## 答案1

![创建新列规则的屏幕图像](assets/conditional-formatting-exercise.png)

1. 在任务列表报告中，转至 **[!UICONTROL View]** 下拉菜单并选择 **[!UICONTROL New View]**。
1. 将您的视图命名为“标准+进度”。
1. 使用所提供的默认列。
1. 选择 [!UICONTROL Task Name] 列。这是您要应用条件格式的列，这样一来，如果任务的进度状态不是“按时”，它便会显示为红色或黄色。
1. 单击位于 Report Builder 窗口右上角的 **[!UICONTROL Advanced Options]**。
1. 单击 **[!UICONTROL Add a Rule for this Column]**。
1. 通过将窗口顶部的 [!UICONTROL Task] > [!UICONTROL Name] 更改为 [!UICONTROL Task] > [!UICONTROL Progress Status] 来启动列规则。只需单击 [!UICONTROL Task] > [!UICONTROL Name] 旁边的 **[!UICONTROL X]** 图标即可将其从字段中删除。
1. 在该字段中键入“进度”，然后选择 [!UICONTROL Task] 字段源下的 [!UICONTROL Progress Status]。
1. 在 [!UICONTROL Equal] 限定符右侧的字段中选择 **[!UICONTROL Late]**。
1. 在 [!UICONTROL Text Color] 行中选择红色背景。
1. 单击 **[!UICONTROL Add Rule]** 保存列规则。
1. 现在再次单击 **[!UICONTROL Add Column Rule]** 来添加另一条规则。
1. 和之前一样，从条件字段中删除 [!UICONTROL Task] > [!UICONTROL Name]。将其替换为 [!UICONTROL Task] 字段源下的 [!UICONTROL Progress Status]。
1. 在“等于”限定符右侧的字段中同时选择 [!UICONTROL At Risk] 和 [!UICONTROL Behind]。
1. 在 [!UICONTROL Text Color] 行中选择黄色背景。
1. 单击 **[!UICONTROL Add Rule]** 保存列规则。
1. 单击 **[!UICONTROL Save View]** 保存视图。
