---
title: 轮到您创建日历
description: 了解如何创建显示未完成任务和问题的客户日历。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# 轮到您创建日历

在本练习中，您将获得有关创建您自己的日历的体验。

## 活动：创建日历

创建名为“我的未完成工作”的客户日历。

包含一个名为“未完成任务”的日历组，该组显示在当前项目上分配给您的所有未完成任务。

选择红色作为这些项目的颜色。

包括另一个名为“未完成问题”的日历组，该组显示当前项目分配给您的所有未完成问题。 选择蓝色作为这些项目的颜色。

## 答案

1. 从主菜单导航到日历区域。
1. 单击“新建日历”按钮并将日历命名为“我的未完成工作”。
1. 在第一个分组下，单击添加高级项目。
1. 在弹出的将项目添加到日历窗口中，将组命名为“未完成任务”。
1. 选择红色作为颜色。
1. 将日期字段更改为计划日期。
1. 将“在日历上，显示字段”设置为“仅结束日期”。
1. 将“Switch to actual dates when available（可用时切换到实际日期）”字段设置为“No（否）”。

   ![用于将项目添加到日历的屏幕图像](assets/calendar-activity-1.png)

1. 在“What want to add to the calendar？（要将什么添加到日历？）”中 部分，选择任务。
1. 添加三个筛选规则：

   * “项目”>“状态等于”>“等于”>“当前”
   * 任务用户> ID >等于> $$USER.ID
   * 任务>完成>等于> False

1. 单击保存。

   ![用于将项目添加到日历的屏幕图像](assets/calendar-activity-2.png)

1. 通过单击添加到日历创建第二个分组。
1. 在此分组下，单击添加高级项目。
1. 在弹出的将项目添加到日历窗口中，将组命名为“未完成问题”。
1. 选择蓝色作为颜色。
1. 将日期字段更改为计划日期。
1. 将“在日历上，显示字段”设置为“仅结束日期”。
1. 将“Switch to actual dates when available（可用时切换到实际日期）”字段设置为“No（否）”。
1. 在“What want to add to the calendar？（要将什么添加到日历？）”中 部分，选择问题。
1. 添加以下三个筛选规则：

   * “项目”>“状态等于”>“等于”>“当前”
   * 任务用户> ID >等于> $$USER.ID
   * 问题>完成>等于> False

1. 单击保存。

   ![用于将项目添加到日历的屏幕图像](assets/calendar-activity-3.png)

由于您在筛选器中使用了$$USER.ID，因此您可以与其他人共享此日历，这样他们将看到自己的未完成任务和问题。
