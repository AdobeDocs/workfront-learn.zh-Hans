---
title: 创建基本过滤器活动
description: 在此活动中，您将创建一个名为“本月关闭的项目”的项目过滤器。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 100%

---

# 创建基本过滤器活动

## 活动 1 - 营销项目组合中的所有项目

在此活动中，您将会在 [!UICONTROL Legacy filter] 体验中创建一个名为“营销项目组合中的所有项目”的项目过滤器。这将会向您显示名为“营销项目组合”的项目组合中的所有项目，无论其状态如何。

下面包含分步说明。

### 活动 1 答案

![用于创建新过滤器的屏幕图像](assets/basic-filter-activity-1.png)

1. 从 [!UICONTROL Main Menu] 导航到 [!UICONTROL Projects] 区域。这会向您显示项目列表。
1. 单击 **[!UICONTROL Filter]** 菜单并选择 [!UICONTROL Legacy Filters]。
1. 选择 **[!UICONTROL New Filter]**。
1. 将您的过滤器命名为“营销项目组合中的所有项目”。
1. 单击 **[!UICONTROL Add Filter Rule]**。
1. 在 [!UICONTROL Start typing field name] 字段中，输入“[!UICONTROL portfolio name]”。然后在 [!UICONTROL Portfolio] 字段源下选择 [!UICONTROL Name]。
1. 使 [!UICONTROL Equal] 运算符保持原样。
1. 在 [!UICONTROL Start typing name] 字段中，输入“[!UICONTROL marketing]”。
1. 选择 [!UICONTROL Marketing Portfolio]，假设您有一个要筛选的名称的项目组合。如果没有，只需使用提前输入功能即可找到您想要的项目组合。
1. 单击 **[!UICONTROL Save Filter]**。

## 活动 2 - 我拥有的本月结束的项目

在此视频中，您将会在 [!UICONTROL Legacy filter] 体验中创建一个名为“我拥有的本月结束的项目”的项目过滤器。如果您正在关注大量项目，此过滤器可以帮助您重点关注规划很快关闭的项目。

下面包含分步说明。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### 活动 2 答案

![用于创建新过滤器的屏幕图像](assets/basic-filter-activity-updated-6-15-21.png)

1. 从 [!UICONTROL Main Menu] 导航到 [!UICONTROL Projects] 区域。这会向您显示项目列表。
1. 单击 **[!UICONTROL Filter]** 菜单并选择 [!UICONTROL Legacy Filters]。
1. 选择 **[!UICONTROL New Filter]**。
1. 将您的过滤器命名为“我拥有的本月结束的项目”。
1. 单击 **[!UICONTROL Add Filter Rule]**。
1. 在 [!UICONTROL Start typing field name] 字段中，输入“所有者”。然后在 [!UICONTROL Project] 字段源下选择 [!UICONTROL Owner ID]。
1. 使 [!UICONTROL Equal] 运算符保持原样。
1. 在 [!UICONTROL Start typing name] 字段中输入“$$”。
1. 选择 [!UICONTROL $$USER.ID]。这是登录用户的通配符。
1. 再次单击 [!UICONTROL Add Filter Rule]。
1. 在 [!UICONTROL Start typing field name] 字段中，开始输入“完成”。然后在项目字段源下选择 [!UICONTROL Is Complete]。
1. 使 [!UICONTROL Equal] 运算符保持原样。
1. 选择“False”。
1. 再次单击 [!UICONTROL Add Filter Rule]。
1. 在 [!UICONTROL Start typing field name] 字段中，输入“已规划”，然后选择 [!UICONTROL Project] 字段源下的 [!UICONTROL Planned Completion Date]。
1. 将 [!UICONTROL Equal] 运算符更改为 [!UICONTROL This Month]。
1. 单击 **[!UICONTROL Save Filter]**。
