---
title: 创建自定义提示
description: 了解什么是自定义提示、如何使用文本模式创建自定义提示以及可以在 Workfront 中的报告中使用的一些示例。
activity: use
feature: Text Mode Reporting
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 98%

---

# 创建自定义提示

在本视频中，您将了解到：

* 什么是自定义提示
* 如何使用文本模式创建自定义提示
* 您可以在报告中使用的一些示例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## 创建自定义提示活动

[单击此处](/help/assets/create-custom-prompts-activities.pdf)下载此页面的 PDF。

## 活动：创建自定义提示

1. 创建自定义提示，其中在提示下拉菜单中显示以下项目状态：
   * 规划中
   * 目前
   * 已完成
   * 已停止
1. 修改提示以显示本月到期的当前项目。

## 答案

1. 您的自定义提示应与此类似，并具有以下文本模式：

   ![在文本模式下创建新过滤器的屏幕图像](assets/cp-01.png)

   保存自定义提示后，提示下拉菜单应如下所示：

1. 自定义提示中的文本模式应如下所示：

![在文本模式下创建新过滤器的屏幕图像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

活动提示的下拉标签应该更新，以反映代码中的更改，如下所示：

![在文本模式下创建新过滤器的屏幕图像](assets/cp-02a.png)
