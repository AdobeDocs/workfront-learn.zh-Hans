---
title: 了解如何在中管理资源 [!UICONTROL Workfront DAM]
description: 了解如何在中管理资源 [!UICONTROL Workfront DAM] 以改进您的工作流。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 参与者：资产管理

在本视频中，您将了解如何：

* 使用资源上的编辑菜单
* 设置到期日期
* 查看通知
* 建立单个通知设置
* 上传资源版本
* 创建新文件夹
* 将元数据模板应用到文件夹
* 建立文件夹权限

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## 资源版本的工作方式

工作流程的一部分可能包括管理资源的多个版本（或倒圆角、校样、小版本，无论您怎样称呼它们）。 您可以通过管理所有版本 [!UICONTROL Workfront DAM].

当一个与现有文件同名的文件上载到同一文件夹时，系统允许进行自动资源版本控制。 请与系统管理员联系，查看此功能是否已启用。

如果启用了自动版本控制，则仅当资产加载到保存原始资产的文件夹时，才会进行版本控制。 两个资源必须具有相同的文件名。 如果资产加载到其他文件夹中，则该资产会作为新文件进入。
如果未打开版本控制，则与现有文件同名的文件将上载为新文件，而不管它放在哪个文件夹中。 这可能会导致同一文件夹中包含两个同名资产。

您还可以手动上传特定资源的版本。 单击资源上的编辑图标，然后选择 **[!UICONTROL Upload new version]**.

如果将带有版本的资产发布到Brand Connect，则Brand Connect用户只会看到该资产的最新版本。

## 文件夹和资产状态和到期

状态是另一种管理对文件夹和资产访问的方式。 [!UICONTROL Workfront DAM]. 状态可用于对某些资源或文件夹进行隐藏 [!UICONTROL Brand Connect] 使用户或使资源或文件夹过期，以便除系统管理员外无人能访问。

* **[!UICONTROL Active]** — 用于资源和文件夹。 具有的资源和文件夹 [!UICONTROL Active] 状态对具有权限的所有用户可见，并可发布到 [!UICONTROL Brand Connect]. [!UICONTROL Active] 资源或文件夹上以绿色圆点指示。
* **[!UICONTROL Inactive]** — 用于资源和文件夹。 具有的资源和文件夹 [!UICONTROL Inactive] 状态对 [!UICONTROL Workfront DAM] 用户，但在中不可见 [!UICONTROL Brand Connect]. [!UICONTROL Inactive] 资源或文件夹上以红点指示。
* **[!UICONTROL Unexpired]** — 仅用于资产。 这是所有资源的默认状态。 未到期的资产，也 [!UICONTROL Active] 在中可见 [!UICONTROL Brand Connect].
* **[!UICONTROL Expired]** — 仅用于资产。 具有的资产 [!UICONTROL Expired] 除系统管理员外，任何用户都不能下载状态。 过期的资产在中可见/不可见 [!UICONTROL Brand Connect]，具体取决于系统配置。
