---
title: 了解中的组和用户 [!UICONTROL Workfront DAM]
description: 了解如何在中创建文件夹、组和用户 [!UICONTROL Workfront DAM]. 了解用户角色类型并授予文件夹权限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 系统设置：组和用户

在本视频中，您将了解如何：

* 了解组设置如何影响对资源的访问
* 按特定顺序创建文件夹、组和用户
* 了解用户角色类型
* 向文件夹授予权限
* 创建和编辑组
* 添加和编辑用户

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## 组和用户审核

当您配置 [!UICONTROL Workfront DAM] 在系统中，考虑用户和群组在全局中扮演的角色非常重要。

组控制对资源文件夹的访问 [!UICONTROL Workfront DAM]. 群组设置还控制用户可以如何处理资产（查看、下载、编辑等） 他们有权访问。

在创建组时，必须牢记该组的成员需要访问哪些资源文件夹 [!UICONTROL Workfront DAM].

用户是登录到 [!UICONTROL Workfront DAM]. 用户无法访问中的任何内容 [!UICONTROL Workfront DAM] 除非将它们分配给组。 用户可属于多个组，具体取决于其需求。

## 默认组

随附两个默认组 [!UICONTROL Workfront DAM]. 所有用户是否都属于这些组，取决于他们是否拥有 [!UICONTROL Workfront DAM] 登录凭据。 您无法从这些组添加或删除用户：

* **来宾组** — 用于控制匿名用户的访问。 可能是没有登录凭据的用户或当前未登录的用户。
* **已记录**-In组 — 所有已登录的用户都属于此组。

默认情况下，管理组及其设置也存在。 您可以将用户添加到此组，但无法调整设置。

## 角色类型

在创建组时，会为其分配角色类型。 角色类型决定了 [!UICONTROL Workfront DAM] 系统用户登录时获得 —  [!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect].

提供了三种角色类型 [!UICONTROL Workfront DAM] 许可证：

* **[!UICONTROL Brand Portal]** — 这些用户只能访问 [!UICONTROL Brand Connect]，用户可以在其中查看和下载已批准的资产。
* **[!UICONTROL Contributor]** — 这些用户可以访问 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]. 他们拥有对资源和文件夹的完全访问权限 — 查看、下载、上传、编辑、移动和删除。
* **[!UICONTROL Administrator]** — 系统管理员可以访问中的所有内容 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM]，并可为每个设置全局系统设置。 他们还可以访问已过期或已设置为非活动的资产。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
