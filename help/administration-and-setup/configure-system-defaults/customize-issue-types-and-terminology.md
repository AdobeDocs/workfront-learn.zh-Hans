---
title: 自定义问题类型和术语
description: 了解如何自定义和重命名四种默认问题类型，以满足您组织的需求。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10021
exl-id: d1e5c2d6-b001-4e9e-b72d-c792c70d09e8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 100%

---

# 自定义问题类型和术语

## 重命名默认问题类型

[!DNL Workfront] 提供四种类型的问题，以帮助您的用户对所创建的问题类型进行分类。默认值为：

* [!UICONTROL Bug Report]
* [!UICONTROL Change Order]
* [!UICONTROL Issue]
* [!UICONTROL Request]

如果现有问题类型不符合您组织的问题管理需求怎么办？或者您的组织可能使用的是不同的术语？

例如，有一个团队希望使用问题来跟踪项目风险。作为系统管理员，您知道您的组织不会跟踪错误报告。因此，您可以将未使用的问题类型（如 [!UICONTROL Bug Reports]）的名称更改为“项目风险”。

问题类型在系统范围内进行重命名，因此更改适用于所有用户。

1. 单击 **[!UICONTROL Main Menu]** 中的 **[!UICONTROL Setup]**。
1. 展开左侧菜单面板中的 **[!UICONTROL Project Preferences]** 部分。
1. 选择 **[!UICONTROL Statuses]**。
1. 选择 **[!UICONTROL Issues]** 选项卡。
1. 确保右上角的菜单设置为 [!UICONTROL System Statuses]。
1. 将光标悬停在列表顶部的问题类型旁边。单击铅笔图标以启用字段编辑。
1. 重命名问题类型。
1. 单击字段外部进行保存。

![[!UICONTROL Issues] 选项卡，在 [!UICONTROL Statuses] 页面中，位于 [!UICONTROL Setup]](assets/admin-fund-issue-types.png)

>[!NOTE]
>
>您无法创建更多问题类型或删除问题类型。

<!---
learn more URLs
Customize default issue types
--->

## 更改 Workfront 中的术语“问题”

有些组织使用不同于“问题”的术语来指代规划外的工作项目。“问题”是默认术语，并会在整个软件中出现——菜单、报告、字段名称等。
Workfront 管理员可以使用布局模板功能重命名问题项目，以匹配其组织使用的术语。对于分配到布局模板的人员，新术语随后会出现在整个 [!DNL Workfront] 中。

![[!UICONTROL Terminology] 窗口，其中突出显示 [!UICONTROL Issue]](assets/admin-fund-issue-custom-terminology.png)

<!---
paragraph below needs a hyperlink
--->

通过学习路径《全新 [!DNL Workfront] 体验中的管理员基础知识：第三部分 控制与界面体验》，了解系统和组管理员如何创建布局模板。

<!---
learn more URLs
Create and manage layout templates
--->
