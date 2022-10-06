---
title: 创建和管理问题严重性
description: 了解如何设置和管理问题严重性。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 创建和管理问题严重性

## 问题严重性简介

严重性可用于指示问题的严重程度或可能如何影响正在完成的工作。

![[!UICONTROL Severity] 菜单 [!UICONTROL Issue Details] 窗口](assets/admin-fund-severity-issue-details.png)

的 [!UICONTROL Severity] 字段 [!UICONTROL Issue Details]. 它还可以包含在列表的列视图和自定义报表中。

[!DNL Workfront] 具有五个默认类别：

* [!UICONTROL Cosmetic]
* [!UICONTROL Causes Confusion]
* [!UICONTROL Bug with workaround]
* [!UICONTROL Bug with no workaround]
* [!UICONTROL Fatal error]

系统管理员可以重命名这些默认服务性，或根据需要创建新服务性。

严重性仅适用于 [!DNL Workfront].

## 创建和管理问题严重性

作为系统管理员，您可以根据需要创建新严重性，以完成问题的工作流程。

![[!UICONTROL Severities] 页面 [!UICONTROL Setup]](assets/admin-fund-severity-section.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 的双曲余切值。
1. 选择 **[!UICONTROL Severities]**.
1. 单击 **[!UICONTROL Add a New Severity]**.
1. 为严重性指定与其预期用途匹配的名称。
1. 的 **[!UICONTROL Importance]** 数字与问题的严重性匹配。 最高值与最高严重性相对应。 的 [!UICONTROL Importance] 数字必须唯一。
1. 选择优先级的颜色。 该函数用于图表报表和 [!DNL Workfront].
1. 指定其中一个严重性选项作为 **[!UICONTROL Default Severity]**. 此操作会自动应用于Workfront中的所有新问题。
1. 包括严重性的描述，如使用方式。
1. 单击要保存的字段外部。

![[!UICONTROL Severities] 列表](assets/admin-fund-severity-new.png)

### 修改严重性

如果严重性不再与您的问题工作流相关，则可以重命名、隐藏或删除该严重性。

如果不再需要严重性， [!DNL Workfront] 建议您隐藏严重性(单击 [!UICONTROL Hide] 框中)。 这会从问题的下拉菜单中删除严重性选项，但它会保留历史数据的严重性，因此仍可用于报告目的。

![[!UICONTROL Hide] 列突出显示 [!UICONTROL Severities] 页面 [!UICONTROL Setup]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] 建议您 **不** 删除过去问题中使用的严重性。 删除严重性时，它会要求您替换另一个严重性。 这会更改历史数据并影响报表。

![删除严重性窗口](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
