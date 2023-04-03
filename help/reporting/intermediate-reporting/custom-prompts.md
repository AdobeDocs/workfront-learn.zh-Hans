---
title: 创建自定义提示
description: 了解自定义提示是什么，如何使用文本模式创建自定义提示，以及一些可在Workfront报表中使用的示例。
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# 创建自定义提示

在此视频中，您将学习：

* 自定义提示是什么
* 如何使用文本模式创建自定义提示
* 可在报表中使用的一些示例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## 活动：创建自定义提示

1. 在“提示”下拉菜单中创建一个自定义提示，以显示以下项目状态：
   * 计划
   * 目前
   * 已完成
   * 废弃
1. 修改提示以显示本月到期的当前项目。

## 答案

1. 您的自定义提示应类似于此模式，并具有以下文本模式：

   ![在文本模式下创建新过滤器的屏幕图像](assets/cp-01.png)

   保存自定义提示后，提示下拉菜单应如下所示：

1. 自定义提示中的文本模式应如下所示：

![在文本模式下创建新过滤器的屏幕图像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

并且应更新活动提示的下拉标签，以反映代码中的更改，如下所示：

![在文本模式下创建新过滤器的屏幕图像](assets/cp-02a.png)
