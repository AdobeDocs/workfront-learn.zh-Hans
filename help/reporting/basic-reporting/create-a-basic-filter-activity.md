---
title: 创建基本过滤器活动
description: 在此活动中，您将创建一个名为“我拥有的本月结束项目”的项目筛选器。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 1%

---

# 创建基本过滤器活动

在此视频中，您将创建一个名为“我拥有的本月结束的项目”的项目筛选器。 如果您关注大量项目，此过滤器可以帮助您放大计划不久后关闭的项目。

下面提供了分步说明。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

## 回答

![用于创建新过滤器的屏幕图像](assets/basic-filter-activity-updated-6-15-21.png)

1. 导航到 [!UICONTROL Projects] 区域 [!UICONTROL Main Menu]. 这会显示项目列表。
1. 单击 **[!UICONTROL Filter]** 菜单和选择 **[!UICONTROL New Filter]**.
1. 将您的过滤器命名为“我拥有本月结束的项目”。
1. 单击 **[!UICONTROL Add Filter Rule]**.
1. 在 [!UICONTROL Start typing field name] 字段中，键入“所有者”。 然后选择 [!UICONTROL Owner ID] 下 [!UICONTROL Project] 字段源。
1. 离开 [!UICONTROL Equal] 运算符。
1. 在开始键入名称字段中键入“$$”。
1. 选择 [!UICONTROL $$USER.ID]. 这是登录用户的通配符。
1. 单击 [!UICONTROL Add Filter Rule] 再次。
1. 在 [!UICONTROL Start typing field name] 字段中，开始键入“Is Complete”。 然后选择 [!UICONTROL Is Complete] 在项目字段源下。
1. 离开 [!UICONTROL Equal] 运算符。
1. 选择“False”。
1. 单击 [!UICONTROL Add Filter Rule] 再次。
1. 在 [!UICONTROL Start typing field name] 字段类型“已计划”，然后选择 [!UICONTROL Planned Completion Date] 下 [!UICONTROL Project] 字段源。
1. 更改 [!UICONTROL Equal] 运算符 [!UICONTROL This Month].
1. 单击 **[!UICONTROL Save Filter]**
