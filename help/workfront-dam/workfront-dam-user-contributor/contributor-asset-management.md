---
title: 了解作为投稿人如何管理资源
description: 了解如何管理 [!UICONTROL Workfront DAM] 中的资源，以改善工作流。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 100%

---

# 了解作为投稿人如何管理资源

在本视频中，您将学习如何：

* 使用资源的“编辑”菜单
* 设置过期日期
* 查看通知
* 建立个人通知设置
* 上传资源版本
* 创建新文件夹
* 将元数据模板应用到文件夹
* 建立文件夹权限

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on&enablevpops=1)

## 资源版本如何工作

您的工作流的一部分可能包括管理资源的多个版本（或轮次、校样、迭代，无论您如何称呼它们）。您可以通过 [!UICONTROL Workfront DAM] 管理所有版本。

当与现有文件同名的文件上传到同一文件夹时，系统允许进行自动资源版本控制。请咨询您的系统管理员以查看此功能是否已开启。

如果开启自动版本控制，则仅当资源加载到保存原始资源的文件夹中时，该资源才会进行版本控制。这两个资源必须具有相同的文件名。如果资源被加载到不同的文件夹中，则资源会作为新文件进入该文件夹。
如果未开启版本控制，则与现有文件同名的文件将作为新文件上传，无论将它放在哪个文件夹中均是如此。这可能会导致同一文件夹中出现两个同名的资源。

您还可以手动上传特定资源的版本。单击资源上的编辑图标，然后选择 **[!UICONTROL Upload new version]**。

如果您将带有版本的资源发布到 Brand Connect，则 Brand Connect 用户只能看到该资源的最新版本。

## 文件夹和资源状态和到期时间

状态是您管理对 [!UICONTROL Workfront DAM] 中的文件夹和资源的访问的另一种方式。状态可用于隐藏 [!UICONTROL Brand Connect] 用户的某些资源或文件夹，或使资源或文件夹过期，以便除系统管理员之外的任何人都无法访问它。

* **[!UICONTROL Active]**—用于资源和文件夹。处于 [!UICONTROL Active] 状态的资源和文件夹对所有有权限的用户可见，并且可以发布到 [!UICONTROL Brand Connect]。[!UICONTROL Active] 在资源或文件夹上用绿点表示。
* **[!UICONTROL Inactive]**—用于资源和文件夹。处于 [!UICONTROL Inactive] 状态的资源和文件夹对 [!UICONTROL Workfront DAM] 用户可见，但在 [!UICONTROL Brand Connect] 中不可见。[!UICONTROL Inactive] 在资源或文件夹上用红点表示。
* **[!UICONTROL Unexpired]**—仅用于资源。这是所有资源的默认状态。同样为 [!UICONTROL Active] 的未到期资源在 [!UICONTROL Brand Connect] 中可见。
* **[!UICONTROL Expired]**—仅用于资源。除系统管理员外，任何用户都不能下载状态为 [!UICONTROL Expired] 的资源。根据系统配置，过期资源在 [!UICONTROL Brand Connect] 中可见/不可见。
