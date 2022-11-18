---
title: 了解 [!UICONTROL Workfront DAM]
description: 了解如何在中创建文件夹、组和用户 [!UICONTROL Workfront DAM]. 了解用户角色类型并授予文件夹权限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 系统设置：组和用户

在此视频中，您将学习如何：

* 了解组设置如何影响资产访问
* 按特定顺序创建文件夹、组和用户
* 了解用户角色类型
* 授予文件夹的权限
* 创建和编辑群组
* 添加和编辑用户

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## 组和用户查看

在配置 [!UICONTROL Workfront DAM] 系统中，从整体上考虑用户和群组所扮演的角色至关重要。

组控制对 [!UICONTROL Workfront DAM]. 群组设置还可以控制用户可以对资产执行的操作（查看、下载、编辑等） 他们有权访问。

在创建组时，切记组成员需要在中访问的资产文件夹 [!UICONTROL Workfront DAM].

用户是指登录到 [!UICONTROL Workfront DAM]. 用户无法访问 [!UICONTROL Workfront DAM] 除非将它们分配给组。 用户可以属于多个组，具体取决于其需求。

## 默认组

附带两个默认组 [!UICONTROL Workfront DAM]. 所有用户都会根据他们是否自动属于这些组 [!UICONTROL Workfront DAM] 登录凭据。 您不能从以下群组添加或删除用户：

* **来宾组** — 用于控制匿名用户的访问。 这可能是没有登录凭据的人或当前未登录的用户。
* **已记录**-In组 — 登录的所有用户都属于此组。

默认情况下，管理员组及其设置也存在。 您可以将用户添加到此组，但无法调整设置。

## 角色类型

在创建群组时，会为其分配角色类型。 角色类型决定 [!UICONTROL Workfront DAM] 系统用户登录后会得到 —  [!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect].

有三种可用的角色类型 [!UICONTROL Workfront DAM] 许可证：

* **[!UICONTROL Brand Portal]** — 这些用户只能访问 [!UICONTROL Brand Connect]，用户可以在此处查看和下载已批准的资产。
* **[!UICONTROL Contributor]** — 这些用户可以访问 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]. 他们拥有资产和文件夹的完全访问权限 — 查看、下载、上传、编辑、移动和删除。
* **[!UICONTROL Administrator]** — 系统管理员有权访问 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM]，以及为每个系统建立全局系统设置的功能。 他们还可以访问已过期或设置为不活动的资产。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
