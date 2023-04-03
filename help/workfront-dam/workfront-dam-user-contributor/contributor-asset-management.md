---
title: 了解如何在 [!UICONTROL Workfront DAM]
description: 了解如何在 [!UICONTROL Workfront DAM] 以改进您的工作流。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 参与者：资产管理

在此视频中，您将学习如何：

* 对资产使用编辑菜单
* 设置过期日期
* 查看通知
* 建立单个通知设置
* 上传资产版本
* 创建新文件夹
* 将元数据模板应用到文件夹
* 建立文件夹权限

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## 资产版本的工作原理

工作流的一部分可能包括管理资产的多个版本（或轮次、校样、小版本，无论您称之为什么）。 您可以通过 [!UICONTROL Workfront DAM].

当将与现有文件同名的文件上传到同一文件夹时，系统允许自动控制资产版本。 请咨询系统管理员，以查看此功能是否已打开。

如果启用了自动版本控制，则只有当资产加载到包含原始资产的文件夹中时，该资产才会进行版本化。 两个资产的文件名必须相同。 如果资产加载到其他文件夹，则资产将作为新文件进入。
如果未启用版本控制，则与现有文件同名的文件将上传为新文件，而不管它放入哪个文件夹。 这可能会导致在同一文件夹中存在两个具有相同名称的资产。

您还可以手动上传特定资产的版本。 单击资产上的编辑图标，然后选择 **[!UICONTROL Upload new version]**.

如果您将包含版本的资产发布到Brand Connect，则Brand Connect用户只会看到该资产的最新版本。

## 文件夹和资产状态及到期

状态是您管理中文件夹和资产访问权限的另一种方式 [!UICONTROL Workfront DAM]. 状态可用于隐藏某些资产或文件夹 [!UICONTROL Brand Connect] 用户或使资产或文件夹过期，这样除系统管理员外，任何人都无法访问该资产或文件夹。

* **[!UICONTROL Active]** — 用于资产和文件夹。 资产和文件夹 [!UICONTROL Active] 状态对所有具有权限的用户都可见，并可以发布到 [!UICONTROL Brand Connect]. [!UICONTROL Active] 在资产或文件夹上以绿色圆点指示。
* **[!UICONTROL Inactive]** — 用于资产和文件夹。 资产和文件夹 [!UICONTROL Inactive] 状态可见于 [!UICONTROL Workfront DAM] 用户，但在 [!UICONTROL Brand Connect]. [!UICONTROL Inactive] 在资产或文件夹上以红色圆点表示。
* **[!UICONTROL Unexpired]** — 仅用于资产。 这是所有资产的默认状态。 未届满资产亦 [!UICONTROL Active] 在 [!UICONTROL Brand Connect].
* **[!UICONTROL Expired]** — 仅用于资产。 资产 [!UICONTROL Expired] 除系统管理员外，任何用户都无法下载状态。 过期的资产在 [!UICONTROL Brand Connect]，具体取决于系统配置。
