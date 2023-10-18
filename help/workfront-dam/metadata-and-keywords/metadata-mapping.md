---
title: 设置元数据映射
description: 了解如何设置元数据映射 [!UICONTROL Workfront DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 设置元数据映射

[!DNL Workfront]有关资产的相关信息可从以下位置传输： [!DNL Workfront] 到 [!UICONTROL Workfront DAM] 与资产同步。 中的元数据映射选项 [!DNL Workfront] [!UICONTROL Setup] 区域允许进行此信息传输。

与您的 [!DNL Workfront] 咨询人获取有关设置元数据映射的最佳实践建议。

您必须是 [!DNL Workfront] 管理员和 [!UICONTROL Workfront DAM] 管理员设置元数据映射。 在开始之前，您必须先连接 [!DNL Workfront] 和 [!UICONTROL Workfront DAM] 帐户。

## 连接帐户

1. 登录 [!DNL Workfront].
1. 打开项目、任务或问题，然后单击 **[!UICONTROL Documents]** 选项卡。
1. 单击 **[!UICONTROL Add New]** 按钮并选择 **[!UICONTROL From Workfront DAM]** 从下拉菜单中。
1. 在“ ”中输入登录名和密码 [!UICONTROL Workfront DAM] 出现的授权框。
1. 接下来，单击 **[!UICONTROL Yes]** 给予 [!DNL Workfront] 访问 [!UICONTROL DAM] 帐户。
1. 如果需要，请刷新页面以更新对的访问权限 [!UICONTROL Workfront DAM].

建立此连接后，现在可以开始在两个系统之间映射元数据。 确保您已在中创建所需的元数据字段 [!UICONTROL Workfront DAM] 开始映射之前。

## 设置映射

1. 登录 [!DNL Workfront].
1. 选择 **[!UICONTROL Setup]** 从 [!UICONTROL Main Menu].
1. 展开 **[!UICONTROL Documents]** 部分。
1. 然后单击 **[!UICONTROL Metadata Mapping]**.
1. 在Workfront字段中，键入 [!DNL Workfront] 要映射的字段。
1. 然后选择相应的或目标 **[!UICONTROL Workfront DAM]** 元数据字段。
1. 单击 **[!UICONTROL Add Mapping]** 按钮。
1. 您将会看到 [!UICONTROL Workfront Field Source] 和 [!UICONTROL Workfront DAM Target Field] 在窗口底部的图表中。
1. 对所有所需的元数据字段重复此操作。

![屏幕截图 [!UICONTROL Metadata Mapping] screen in [!DNL Workfront]](assets/01-metadata-mapping.png)
