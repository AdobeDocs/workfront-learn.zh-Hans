---
title: 设置事件通知
description: 了解如何通过管理事件通知来控制用户接收的电子邮件和应用程序内通知。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 100%

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
>由于分阶段推出，一些 [!DNL Workfront] 客户暂时无法使用允许系统和组管理员管理事件通知的功能。请关注本文以获取有关版本的更新：解锁组的事件通知配置。

系统管理员确定用户应通过 [!DNL Workfront] 接收哪些通知。

![[!UICONTROL Email Notifications] 窗口，在 [!UICONTROL Setup] 区域中](assets/admin-fund-notifications-1.png)

[!UICONTROL Event Notifications] 列表按类型分组。对于列出的每个事件通知，您将会看到五条信息：

* **[!UICONTROL Active]—**[!UICONTROL Active] 列允许您在系统范围内打开或关闭通知。
* **[!UICONTROL Name]—**&#x200B;这是 [!DNL Workfront] 中通知的名称。
* **[!UICONTROL Description]—**&#x200B;该描述简要说明了触发通知所发生的操作或响应接收通知需要采取的操作。
* **[!UICONTROL Email Subject]—**&#x200B;当电子邮件发送给用户时，主题行中向用户显示的内容。
* **[!UICONTROL Group Access]—**&#x200B;解锁通知，以便组管理员可以对其进行管理。

## 打开通知

要在全局系统级别管理通知，请确保搜索栏显示 [!UICONTROL System Event Notifications]。

单击切换按钮以显示蓝色，从而打开特定通知，使其可供所有用户使用。如果蓝色被隐藏，则通知处于关闭状态。

![[!UICONTROL Active] 列，在 [!UICONTROL Email Notifications] 页面上](assets/admin-fund-notifications-2.png)

开启事件通知后，事件发生时会立即发送消息。

## 允许组管理员进行控制

系统管理员可以向组管理员授予权限，以根据其组和子组的运作方式及其工作流进一步自定义通知列表。

![[!UICONTROL Group Access] 列，在 [!UICONTROL Email Notifications] 页面上](assets/ganotifications_01.png)

为了使组管理员能够管理其组和子组的通知，需要解锁系统级通知。

* 导航到电子邮件通知页面的“事件通知”选项卡。

* 确保搜索栏显示“系统事件通知”。

* 单击“组访问权限”列中的切换按钮以显示蓝色，从而为所有组管理员解锁单个通知。

* 通过选中每个通知左侧的框并单击列表上方工具栏中的解锁图标，可以一次解锁多个通知。

![[!UICONTROL Group Access] 列，在 [!UICONTROL Email Notifications] 页面上](assets/ganotifications_02.png)

通过单击切换按钮以显示灰色，从而锁定未锁定的通知。通过选中复选框并单击工具栏中的解锁图标，可以同时锁定多个通知。

![[!UICONTROL Group Access] 列，在 [!UICONTROL Email Notifications] 页面上](assets/ganotifications_03.png)

顶级组管理员会看到解锁的通知，以确定其组和子组是否需要该通知。子组会从其顶级父组继承通知配置。﻿


## 管理组通知

当系统管理员解锁通知选项后，组管理员可以通过单击左侧面板菜单中的“事件通知”，从单个组页面管理组的通知。然后您可以激活或停用通知选项。

![[!UICONTROL Group Access] 列，在 [!UICONTROL Email Notifications] 页面上](assets/managegroupnotifications_01.png)

如果需要，系统管理员可以通过在窗口顶部的搜索栏中输入组名称，从“通知”页面管理组的通知。

![[!UICONTROL Group Access] 列，在 [!UICONTROL Email Notifications] 页面上](assets/managegroupnotifications_02.png)

## 专业提示

[!DNL Workfront] 建议为您的用户提供某些通知。

对于大多数用户：

* [!UICONTROL A predecessor of one of my tasks is completed]
* [!UICONTROL Someone includes me on a directed update]
* [!UICONTROL Someone comments on my work item]
* [!UICONTROL The due date changes on a task I’m assigned to]


特别针对项目经理：

* [!UICONTROL A project I’m on becomes active]
* [!UICONTROL A project I own gets behind]
* [!UICONTROL An issue is added to a project I own]
* [!UICONTROL Milestone task is completed on a project I own]

<!---
learn more URLs
--->
