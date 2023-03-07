---
title: 创建基本过滤器活动
description: 在本练习中，您将创建一个名为“本月结束的我所拥有的项目”的项目过滤器。
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
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 1%

---

# 创建基本过滤器活动

在本视频中，您将创建一个名为“本月关闭的我所拥有的项目”的项目过滤器。 如果您正在关注许多项目，此过滤器可以帮助您放大即将关闭的项目。

以下包含分步说明。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## 答案

![用于创建新过滤器的屏幕图像](assets/basic-filter-activity-updated-6-15-21.png)

1. 导航到 [!UICONTROL Projects] 区域 [!UICONTROL Main Menu]. 这将向您显示一个项目列表。
1. 单击 **[!UICONTROL Filter]** 菜单并选择 **[!UICONTROL New Filter]**.
1. 将您的过滤器命名为“本月关闭的我所拥有的项目”。
1. 单击 **[!UICONTROL Add Filter Rule]**.
1. 在 [!UICONTROL Start typing field name] 字段，键入“owner”。 然后选择 [!UICONTROL Owner ID] 在 [!UICONTROL Project] 字段源。
1. 保留 [!UICONTROL Equal] 运算符。
1. 在开始键入名称字段中键入“$$”。
1. 选择 [!UICONTROL $$USER.ID]. 这是登录用户的通配符。
1. 单击 [!UICONTROL Add Filter Rule] 再来一次。
1. 在 [!UICONTROL Start typing field name] 字段中，开始键入“Is Complete”。 然后选择 [!UICONTROL Is Complete] 在项目字段源下。
1. 保留 [!UICONTROL Equal] 运算符。
1. 选择“False”。
1. 单击 [!UICONTROL Add Filter Rule] 再来一次。
1. 在 [!UICONTROL Start typing field name] 字段类型“已计划”，然后选择 [!UICONTROL Planned Completion Date] 在 [!UICONTROL Project] 字段源。
1. 更改 [!UICONTROL Equal] 运算符为 [!UICONTROL This Month].
1. 单击 **[!UICONTROL Save Filter]**
