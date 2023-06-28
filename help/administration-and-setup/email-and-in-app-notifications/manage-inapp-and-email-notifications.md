---
title: 管理应用程序内通知和电子邮件事件通知
description: 了解用户如何控制其收到哪些应用程序内通知和电子邮件通知，以使其收到与其工作相关、有帮助的电子邮件。
short-description: 了解用户如何控制他们接收哪些应用内通知和电子邮件通知。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10095.jpeg
jira: KT-10095
exl-id: 831646d2-ecf8-4fe6-8d4e-8c5fc233ed56
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# 管理应用程序内通知和电子邮件事件通知

电子邮件是日常工作的一部分，有时候，您收到的电子邮件数量会变得让人不知所措。 但是，使用 [!DNL Workfront]，系统管理员可以确保每个人都收到有关其参与的工作的相关且有用的电子邮件。

Workfront可以向用户发送多种类型的通知。 其中一些通知在系统级别进行控制，并影响所有用户。 某些通知可以设置为在每日摘要中即时生成电子邮件。 或者关闭电子邮件以仅在Workfront中生成通知。

## 事件通知

事件类似于状态更改、发布的评论或做出的分配，可以在中触发应用程序内通知 [!DNL Workfront].

![通知列表](assets/admin-fund-user-notifications-01.png)

但是，您可以通过选择或取消选择首选项中的选项来确定要接收电子邮件通知的事件。

要进行这些更改，请在 [!UICONTROL Main Menu].

![中的用户名 [!UICONTROL Main Menu]](assets/admin-fund-user-notifications-02.png)

单击 [!UICONTROL Edit] 从 [!UICONTROL More] 菜单。

![用户配置文件页面上的菜单](assets/admin-fund-user-notifications-03.png)

单击 [!UICONTROL Notifications] 在 [!UICONTROL Edit Person] 弹出框。

![[!UICONTROL Edit Person] 窗口](assets/admin-fund-user-notifications-04.png)

从这里，您可以决定要立即、每天或根本不接收哪些通知。 您在此处进行的任何更改都是特定于您的，不会影响Workfront中的任何其他用户。

**[!UICONTROL Daily]**

默认情况下，电子邮件设置为立即发送。 但是，您可以将电子邮件通知频率从 [!UICONTROL Instant] 到 [!UICONTROL Daily]，确保随时随地获取所需的信息。

![[!UICONTROL Notification] 部分 [!UICONTROL Edit Person] 窗口](assets/admin-fund-user-notifications-05.png)

每日选项在一封电子邮件中发送一天事件的摘要。 用户在中看到的每个分组都会收到一封电子邮件 [!UICONTROL Notifications] 部分。

例如， [!UICONTROL Information about Projects I Own] 部分将生成一封每日电子邮件，即 [!UICONTROL Action Needed] 部分将生成一封每日电子邮件等。

![[!UICONTROL Daily Digest] 电子邮件对象 [!UICONTROL Information about Projects I Own]](assets/admin-fund-user-notifications-06.png)

![[!UICONTROL Daily Digest] 电子邮件对象 [!UICONTROL Action Needed]](assets/admin-fund-user-notifications-07.png)

除了选择每日选项外，还应设置发送这些电子邮件的时间。 根据效果最佳的方式，可以在早上上班前或离开上班前发送摘要电子邮件。

![[!UICONTROL Email Daily Digest after] 中的下拉菜单 [!UICONTROL Edit Person] 窗口](assets/admin-fund-user-notifications-08.png)

**完全没有**

最后一个选项是完全关闭电子邮件通知。

![选定的通知在中关闭 [!UICONTROL Edit Person] 窗口](assets/admin-fund-user-notifications-09.png)

如果您决定执行此操作，请了解虽然您没有收到电子邮件，但仍在中分配、评论和更新工作 [!DNL Workfront]. 关闭所有通知可能会丢失您需要了解的重要信息。

以下是一些实例： [!DNL Workfront] 已看到用户关闭电子邮件通知。 例如，如果您通过 [!DNL Workfront] ，您可以关闭电子邮件通知，并仅通过应用程序接收通知。

不论 [!UICONTROL Event Notifications] 您决定接收通知，通知对于成功实现组织目标的工作至关重要。


## Recommendations

有一些通知 [!DNL Workfront] 建议保留选中状态，无论是为了发送即时电子邮件还是发送每日摘要。

对于大多数用户：

* [!UICONTROL A predecessor of one of my tasks is completed]
* [!UICONTROL Someone includes me on a directed update]
* [!UICONTROL Someone comments on my work item]
* [!UICONTROL The due date changes on a task I'm assigned to]


具体到项目经理：

* [!UICONTROL A project I'm on becomes active]
* [!UICONTROL A project I own gets behind]
* [!UICONTROL An issue is added to a project I own]
* [!UICONTROL Milestone task is completed on a project I own]


<!---
learn more URLs
Email notifications
guide: manage your notifications
--->
