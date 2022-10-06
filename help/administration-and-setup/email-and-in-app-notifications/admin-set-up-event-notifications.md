---
title: 设置事件通知
description: 了解如何通过管理事件通知来控制用户收到的电子邮件和应用程序内通知。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# 设置事件通知

>[!NOTE]
>
>由于分阶段推出，系统和组管理员管理事件通知的功能暂时不适用于某些人员 [!DNL Workfront] 客户。 有关此版本的更新，请阅读本文：解锁组事件通知的配置。

系统管理员确定用户应通过接收哪些通知 [!DNL Workfront].

![[!UICONTROL Email Notifications] 窗口 [!UICONTROL Setup] 面积](assets/admin-fund-notifications-1.png)

的 [!UICONTROL Event Notifications] 列表按类型分组。 对于列出的每个事件通知，您将看到五条信息：

* **[!UICONTROL Active]—** 的 [!UICONTROL Active] 列中，您可以在系统范围内打开或关闭通知。
* **[!UICONTROL Name]—** 这是 [!DNL Workfront].
* **[!UICONTROL Description]—** 该描述简要说明了为触发通知而采取了哪些操作，或在收到通知时需要采取哪些操作。
* **[!UICONTROL Email Subject]—** 向用户发送电子邮件时，主题行中将向用户显示的内容。
* **[!UICONTROL Group Access]—** 解锁通知，以便群组管理员可以管理这些通知。

## 打开通知

要在全局系统级别管理通知，请确保搜索栏显示 [!UICONTROL System Event Notifications].

通过单击切换按钮打开特定通知，使其可供所有用户使用，以使蓝色显示。 如果蓝色被隐藏，则通知关闭。

![[!UICONTROL Active] 列 [!UICONTROL Email Notifications] 页面](assets/admin-fund-notifications-2.png)

打开事件通知后，即会在事件发生时立即发送消息。

## 允许组管理员控制

系统管理员可以根据其组和子组的工作方式及其工作流程，为群组管理员授予进一步自定义通知列表的权限。

![[!UICONTROL Group Access] 列 [!UICONTROL Email Notifications] 页面](assets/ganotifications_01.png)

要让组管理员能够管理其组和子组的通知，需要解锁系统级通知。

* 导航到“电子邮件通知”页面的事件通知选项卡。

* 确保搜索栏显示“系统事件通知”。

* 通过单击“组访问”列中的切换开关，为所有组管理员解锁单个通知，以使蓝色显示。

* 通过选中每个通知左侧的框并单击列表上方工具栏中的解锁图标，一次解锁多个通知。

![[!UICONTROL Group Access] 列 [!UICONTROL Email Notifications] 页面](assets/ganotifications_02.png)

通过单击切换锁定已解锁通知，使灰色显示。 通过选中复选框并单击工具栏中的解锁图标，可同时锁定多个通知。

![[!UICONTROL Group Access] 列 [!UICONTROL Email Notifications] 页面](assets/ganotifications_03.png)

顶层组管理员将显示解锁通知，以确定其组和子组是否需要该通知。 子组将从其顶部父组继承通知配置。 ﻿


## 管理组通知

系统管理员具有解锁通知选项后，群组管理员可以通过单击左侧面板菜单中的事件通知，从单个群组页面管理群组的通知。 然后，您可以激活或停用通知选项。

![[!UICONTROL Group Access] 列 [!UICONTROL Email Notifications] 页面](assets/managegroupnotifications_01.png)

如果需要，系统管理员可以通过在窗口顶部的搜索栏中输入组名称，从“通知”页面管理组的通知。

![[!UICONTROL Group Access] 列 [!UICONTROL Email Notifications] 页面](assets/managegroupnotifications_02.png)

## 专业技巧

有一些通知 [!DNL Workfront] 建议向用户提供。

对于大多数用户：

* [!UICONTROL A predecessor of one of my tasks is completed]
* [!UICONTROL Someone includes me on a directed update]
* [!UICONTROL Someone comments on my work item]
* [!UICONTROL The due date changes on a task I’m assigned to]


具体针对项目经理：

* [!UICONTROL A project I’m on becomes active]
* [!UICONTROL A project I own gets behind]
* [!UICONTROL An issue is added to a project I own]
* [!UICONTROL Milestone task is completed on a project I own]

<!---
learn more URLs
--->
