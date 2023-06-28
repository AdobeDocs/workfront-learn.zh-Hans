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
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
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
>由于分阶段推出，某些用户暂时无法使用系统和组管理员管理事件通知的功能 [!DNL Workfront] 客户。 有关版本：解锁组事件通知的配置，请参阅本文。

系统管理员确定用户应通过接收哪些通知 [!DNL Workfront].

![[!UICONTROL Email Notifications] 中的窗口 [!UICONTROL Setup] 区域](assets/admin-fund-notifications-1.png)

此 [!UICONTROL Event Notifications] 列表按类型分组。 对于列出的每个事件通知，您将看到五项信息：

* **[!UICONTROL Active]—** 此 [!UICONTROL Active] 列允许您在系统范围级别打开或关闭通知。
* **[!UICONTROL Name]—** 这是中通知的名称 [!DNL Workfront].
* **[!UICONTROL Description]—** 描述简要说明了触发通知时执行的操作或接收通知时需要执行的操作。
* **[!UICONTROL Email Subject]—** 将电子邮件发送给用户时，在主题行中向用户显示的内容。
* **[!UICONTROL Group Access]—** 解锁通知，以便组管理员可以管理这些通知。

## 打开通知

要在全局系统级别管理通知，请确保搜索栏中显示 [!UICONTROL System Event Notifications].

打开特定通知，通过单击切换按钮使其对所有用户都可用，从而显示蓝色。 如果蓝色处于隐藏状态，则通知处于关闭状态。

![[!UICONTROL Active] 列于 [!UICONTROL Email Notifications] 页面](assets/admin-fund-notifications-2.png)

打开事件通知后，将在事件发生时立即发送消息。

## 允许组管理员控制

系统管理员可以向组管理员授予权限，以便根据其组和子组的运作方式及其工作流程进一步自定义通知列表。

![[!UICONTROL Group Access] 列于 [!UICONTROL Email Notifications] 页面](assets/ganotifications_01.png)

要让组管理员能够管理其组和子组的通知，需要解锁系统级通知。

* 导航到“电子邮件通知”页的“事件通知”选项卡。

* 确保搜索栏显示“系统事件通知”。

* 通过单击“组访问”列中的切换，使蓝色显示，可解锁所有组管理员的单个通知。

* 选中每个通知左侧的框，然后单击列表上方工具栏中的解锁图标，可一次性解锁多个通知。

![[!UICONTROL Group Access] 列于 [!UICONTROL Email Notifications] 页面](assets/ganotifications_02.png)

通过单击切换开关锁定解锁的通知，使灰色显示。 通过选中复选框并单击工具栏中的解锁图标，同时锁定多个通知。

![[!UICONTROL Group Access] 列于 [!UICONTROL Email Notifications] 页面](assets/ganotifications_03.png)

将为顶级组管理员显示解锁的通知，以确定其组和子组是否需要该通知。 子组从其顶级父组继承通知配置。 ﻿


## 管理组通知

系统管理员解锁通知选项后，组管理员可以通过单击左侧面板菜单中的“事件通知”，从单独的“组”页面管理组的通知。 然后，您可以激活或取消激活通知选项。

![[!UICONTROL Group Access] 列于 [!UICONTROL Email Notifications] 页面](assets/managegroupnotifications_01.png)

如果需要，系统管理员可以通过在窗口顶部的搜索栏中输入组名称来从“通知”页面管理组通知。

![[!UICONTROL Group Access] 列于 [!UICONTROL Email Notifications] 页面](assets/managegroupnotifications_02.png)

## 专业提示

有一些通知 [!DNL Workfront] 建议向用户提供。

对于大多数用户：

* [!UICONTROL A predecessor of one of my tasks is completed]
* [!UICONTROL Someone includes me on a directed update]
* [!UICONTROL Someone comments on my work item]
* [!UICONTROL The due date changes on a task I’m assigned to]


具体到项目经理：

* [!UICONTROL A project I’m on becomes active]
* [!UICONTROL A project I own gets behind]
* [!UICONTROL An issue is added to a project I own]
* [!UICONTROL Milestone task is completed on a project I own]

<!---
learn more URLs
--->
