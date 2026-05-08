---
title: 设置组和用户
description: 了解如何在 [!UICONTROL Workfront DAM] 中创建文件夹、组和用户。 了解用户角色类型并授予文件夹权限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:28:55.491Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 378
ht-degree: 94%

---

# 设置组和用户

在本视频中，您将学习如何：

* 了解组设置如何影响对资源的访问权限
* 按特定顺序创建文件夹、组和用户
* 了解用户角色类型
* 授予文件夹权限
* 创建和编辑组
* 添加和编辑用户

>[!VIDEO](https://video.tv.adobe.com/v/3414465/?captions=chi_hans&quality=12&learn=on&enablevpops=1)

## 组和用户审阅

在配置 [!UICONTROL Workfront DAM] 系统时，需要考虑用户和组在全局中扮演的角色，这一点很重要。

组控制对 [!UICONTROL Workfront DAM] 中的资源文件夹的访问权限。 群组设置还可控制用户可以对资产执行的操作（查看、下载、编辑等） 他们有权访问。

创建组时，必须记住该组的成员需要访问 [!UICONTROL Workfront DAM] 中的哪些资源文件夹。

用户是指可以登录 [!UICONTROL Workfront DAM] 的个人。 用户不能访问 [!UICONTROL Workfront DAM] 中的任何内容，除非他们被分配到一个组。 根据用户的需要，用户可以属于多个组。

## 默认组

[!UICONTROL Workfront DAM] 附带两个默认组。 所有用户都自动属于这些组，这取决于他们是否具有 [!UICONTROL Workfront DAM] 登录凭据。 您无法在这些组中添加或删除用户：

* **访客组**——用于控制匿名用户的访问权限。 这可能是没有登录凭据的人或当前未登录的用户。
* **已登录**&#x200B;组——所有已登录的用户都属于该组。

默认情况下，管理员组及其设置也存在。 您可以将用户添加到该组，但无法调整设置。

## 角色类型

创建组时，系统会为它们分配角色类型。 角色类型决定了 [!UICONTROL Workfront DAM] 系统用户在登录时获得的部分——[!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect]。

[!UICONTROL Workfront DAM] 许可证带有三种角色类型：

* **[!UICONTROL Brand Portal]**——这些用户只具有对 [!UICONTROL Brand Connect] 的访问权限，他们可以在其中查看和下载获得审批的资源。
* **[!UICONTROL Contributor]**——这些用户可以访问 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]。 他们拥有对资源和文件夹的完全访问权限——查看、下载、上传、编辑、移动和删除。
* **[!UICONTROL Administrator]**——系统管理员可以访问 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM] 中的所有内容，并且还可以为每个内容建立全局系统设置。 他们还可以访问已过期或设置为非活动的资源。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* 
-->
