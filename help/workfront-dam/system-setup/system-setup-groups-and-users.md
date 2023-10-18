---
title: 设置组和用户
description: 了解如何在中创建文件夹、组和用户 [!UICONTROL Workfront DAM]. 了解用户角色类型并授予文件夹权限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 设置组和用户

在本视频中，您将学习如何：

* 了解组设置如何影响对资源的访问
* 按特定顺序创建文件夹、组和用户
* 了解用户角色类型
* 向文件夹授予权限
* 创建和编辑组
* 添加和编辑用户

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## 组和用户审核

当您配置 [!UICONTROL Workfront DAM] 系统，考虑用户和群组在全局中扮演的角色非常重要。

组控制对中资源文件夹的访问 [!UICONTROL Workfront DAM]. 群组设置还可控制用户可以对资产执行的操作（查看、下载、编辑等） 他们有权访问。

在创建组时，一定要牢记该组成员需要访问哪些资产文件夹 [!UICONTROL Workfront DAM].

用户是登录到的个人 [!UICONTROL Workfront DAM]. 用户无法访问中的任何内容。 [!UICONTROL Workfront DAM] 除非已将其分配给组。 用户可属于多个组，具体取决于其需求。

## 默认组

随附有两个默认组 [!UICONTROL Workfront DAM]. 所有用户是否均属于这些组，根据其是否属于 [!UICONTROL Workfront DAM] 登录凭据。 您无法从这些组添加或删除用户：

* **来宾组** — 用于控制匿名用户的访问。 可能是没有登录凭据的用户或当前未登录的用户。
* **已记录**-In组 — 所有登录用户都属于该组。

默认情况下，管理员组及其设置也存在。 您可以将用户添加到此组，但无法调整设置。

## 角色类型

在创建组时，将为它们分配角色类型。 角色类型决定了 [!UICONTROL Workfront DAM] 系统用户登录时获得 —  [!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect].

提供了三种角色类型 [!UICONTROL Workfront DAM] 许可证：

* **[!UICONTROL Brand Portal]** — 这些用户只能访问 [!UICONTROL Brand Connect]，用户可以在其中查看和下载批准的资产。
* **[!UICONTROL Contributor]** — 这些用户可以访问 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]. 执行用户拥有对资源和文件夹的完全访问权限 — 查看、下载、上传、编辑、移动和删除。
* **[!UICONTROL Administrator]** — 系统管理员可以访问中的所有内容 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM]，并可为每个设置全局系统设置。 他们还可以访问已过期或已设置为不活动的资源。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
