---
title: 创建和管理问题严重程度
description: 了解如何设置和管理问题严重性。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 创建和管理问题严重程度

## 问题严重程度简介

严重程度可用于指示问题的严重程度或它对正在完成的工作有何影响。

![[!UICONTROL Severity] 中的菜单 [!UICONTROL Issue Details] 窗口](assets/admin-fund-severity-issue-details.png)

此 [!UICONTROL Severity] 字段可在以下位置访问： [!UICONTROL Issue Details]. 它还可以包含在列表上的列视图和自定义报告中。

[!DNL Workfront] 具有五种默认严重程度：

* [!UICONTROL Cosmetic]
* [!UICONTROL Causes Confusion]
* [!UICONTROL Bug with workaround]
* [!UICONTROL Bug with no workaround]
* [!UICONTROL Fatal error]

如果需要，系统管理员可以重命名这些默认严重程度或创建新严重程度。

严重程度仅适用于中的问题 [!DNL Workfront].

## 创建和管理问题严重程度

作为系统管理员，您可以根据需要创建新严重程度以完成问题的工作流。

![[!UICONTROL Severities] 页面位置 [!UICONTROL Setup]](assets/admin-fund-severity-section.png)

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Severities]**.
1. 单击 **[!UICONTROL Add a New Severity]**.
1. 为严重程度提供一个与其预期用途相符的名称。
1. 此 **[!UICONTROL Importance]** 编号与问题的严重性匹配。 最高编号对应于最高严重程度。 此 [!UICONTROL Importance] 数字必须是唯一的。
1. 选择优先级颜色。 这用于图表报表和以下位置中的其他位置 [!DNL Workfront].
1. 指定一个严重性选项作为 **[!UICONTROL Default Severity]**. 这会自动应用于Workfront中的所有新问题。
1. 包括严重性的描述，例如如何使用。
1. 单击字段外部以保存。

![[!UICONTROL Severities] 列表](assets/admin-fund-severity-new.png)

### 修改严重程度

如果某个严重程度不再与您的问题工作流相关，则可以重命名、隐藏或删除该严重程度。

如果不再需要某个严重性， [!DNL Workfront] 建议您隐藏严重性(单击 [!UICONTROL Hide] 框)。 这会从问题的下拉菜单中删除严重性选项，但保留历史数据的严重性，以便仍可用于报告。

![[!UICONTROL Hide] 突出显示的列 [!UICONTROL Severities] 页面位置 [!UICONTROL Setup]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] 建议您 **不要** 删除已在过去的问题上使用的严重程度。 删除某个严重性时，会要求您替换另一个严重性。 这可能会更改历史数据并影响报表。

![“删除严重性”窗口](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
