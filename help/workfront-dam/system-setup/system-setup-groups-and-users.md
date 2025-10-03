---
title: 设置组和用户
description: 了解如何在 [!UICONTROL Workfront DAM] 中创建文件夹、组和用户。了解用户角色类型并授予文件夹权限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 100%

---

# 设置组和用户

在本视频中，您将学习如何：

* 了解组设置如何影响对资源的访问权限
* 按特定顺序创建文件夹、组和用户
* 了解用户角色类型
* 授予文件夹权限
* 创建和编辑组
* 添加和编辑用户

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on&enablevpops=1)

## 组和用户审阅

在配置 [!UICONTROL Workfront DAM] 系统时，需要考虑用户和组在全局中扮演的角色，这一点很重要。

组控制对 [!UICONTROL Workfront DAM] 中的资源文件夹的访问权限。组设置还可以控制用户可以对其具有访问权限的资源执行哪些操作（查看、下载、编辑等）。

创建组时，必须记住该组的成员需要访问 [!UICONTROL Workfront DAM] 中的哪些资源文件夹。

用户是指可以登录 [!UICONTROL Workfront DAM] 的个人。用户不能访问 [!UICONTROL Workfront DAM] 中的任何内容，除非他们被分配到一个组。根据用户的需要，用户可以属于多个组。

## 默认组

[!UICONTROL Workfront DAM] 附带两个默认组。所有用户都自动属于这些组，这取决于他们是否具有 [!UICONTROL Workfront DAM] 登录凭据。您无法在这些组中添加或删除用户：

* **访客组**——用于控制匿名用户的访问权限。这可能是没有登录凭据的人或当前未登录的用户。
* **已登录**&#x200B;组——所有已登录的用户都属于该组。

默认情况下，管理员组及其设置也存在。您可以将用户添加到该组，但无法调整设置。

## 角色类型

创建组时，系统会为它们分配角色类型。角色类型决定了 [!UICONTROL Workfront DAM] 系统用户在登录时获得的部分——[!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect]。

[!UICONTROL Workfront DAM] 许可证带有三种角色类型：

* **[!UICONTROL Brand Portal]**——这些用户只具有对 [!UICONTROL Brand Connect] 的访问权限，他们可以在其中查看和下载获得审批的资源。
* **[!UICONTROL Contributor]**——这些用户可以访问 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]。他们拥有对资源和文件夹的完全访问权限——查看、下载、上传、编辑、移动和删除。
* **[!UICONTROL Administrator]**——系统管理员可以访问 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM] 中的所有内容，并且还可以为每个内容建立全局系统设置。他们还可以访问已过期或设置为非活动的资源。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
