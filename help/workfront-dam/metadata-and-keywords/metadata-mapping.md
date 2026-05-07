---
title: 设置元数据映射
description: 了解如何设置 [!UICONTROL Workfront DAM] 的元数据映射。
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
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
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 234
ht-degree: 100%

---

# 设置元数据映射

[!DNL Workfront]-有关资源的相关信息可以随资源从 [!DNL Workfront] 转移到 [!UICONTROL Workfront DAM]。 [!DNL Workfront] [!UICONTROL Setup] 区域中的元数据映射选项允许这种信息传输。

与您的 [!DNL Workfront] 顾问讨论有关设置元数据映射的最佳实践建议。

您必须是 [!DNL Workfront] 管理员和 [!UICONTROL Workfront DAM] 管理员才能设置元数据映射。 在开始之前，您必须连接您的 [!DNL Workfront] 和 [!UICONTROL Workfront DAM] 帐户。

## 连接帐户

1. 登录 [!DNL Workfront]。
1. 打开项目、任务或问题，然后单击 **[!UICONTROL Documents]** 选项卡。
1. 单击 **[!UICONTROL Add New]** 按钮并从下拉菜单中选择 **[!UICONTROL From Workfront DAM]**。
1. 在出现的 [!UICONTROL Workfront DAM] 授权框中输入您的登录名和密码。
1. 接下来，单击 **[!UICONTROL Yes]**，允许 [!DNL Workfront] 访问 [!UICONTROL DAM] 帐户。
1. 如果需要，刷新页面以更新对 [!UICONTROL Workfront DAM] 的访问权限。

建立此连接后，现在您可以开始在两个系统之间映射元数据。 在开始映射之前，请确保您已经在 [!UICONTROL Workfront DAM] 中创建了所需的元数据字段。

## 设置映射

1. 登录 [!DNL Workfront]。
1. 从 [!UICONTROL Main Menu] 中选择 **[!UICONTROL Setup]**。
1. 展开左侧面板菜单中的 **[!UICONTROL Documents]** 部分。
1. 然后单击 **[!UICONTROL Metadata Mapping]**。
1. 在 Workfront 字段中，输入 [!DNL Workfront] 字段的字段源，以进行映射。
1. 然后选择对应的或目标 **[!UICONTROL Workfront DAM]** 元数据字段。
1. 单击 **[!UICONTROL Add Mapping]** 按钮。
1. 您会在窗口底部的图表中看到 [!UICONTROL Workfront Field Source] 和 [!UICONTROL Workfront DAM Target Field]。
1. 对所有所需的元数据字段重复此操作。

![屏幕快照：[!UICONTROL Metadata Mapping] 屏幕，位于 [!DNL Workfront]](assets/01-metadata-mapping.png)
