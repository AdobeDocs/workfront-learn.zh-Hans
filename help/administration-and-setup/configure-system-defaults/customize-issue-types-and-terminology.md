---
title: 自定义问题类型和术语
description: 了解如何自定义和重命名四种默认问题类型以满足贵组织的需求。
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
source-wordcount: '298'
ht-degree: 0%

---

# 自定义问题类型和术语

## 重命名默认问题类型

[!DNL Workfront] 提供四种类型的问题，帮助您的用户分类正在创建的问题类型。 默认值为：

* [!UICONTROL Bug Report]
* [!UICONTROL Change Order]
* [!UICONTROL Issue]
* [!UICONTROL Request]

如果现有问题类型与贵组织的问题管理需求不匹配，该怎么办？ 或者，您的组织可能使用不同的术语？

例如，有一个团队希望使用问题跟踪项目风险。 作为系统管理员，您知道您的组织不跟踪错误报告。 因此，您可以更改未使用问题类型的名称，例如 [!UICONTROL Bug Reports]，以规避项目风险。

问题类型在系统级别重命名，因此该更改适用于所有用户。

1. 单击 **[!UICONTROL Setup]** 在 **[!UICONTROL Main Menu]**.
1. 展开 **[!UICONTROL Project Preferences]** 左侧菜单面板中的部分。
1. 选择 **[!UICONTROL Statuses]**.
1. 选择 **[!UICONTROL Issues]** 选项卡。
1. 确保将右上角的菜单设置为 [!UICONTROL System Statuses].
1. 将光标悬停在列表顶部问题类型旁边。 单击铅笔图标以启用字段编辑。
1. 重命名问题类型。
1. 单击字段外部以保存。

![[!UICONTROL Issues] 的选项卡 [!UICONTROL Statuses] 页面位置 [!UICONTROL Setup]](assets/admin-fund-issue-types.png)

>[!NOTE]
>
>您无法创建更多问题类型或删除问题类型。

<!---
learn more URLs
Customize default issue types
--->

## 更改Workfront中的术语“问题”

某些组织使用“问题”以外的术语来指计划外工作项。 问题为默认术语，出现在整个软件中 — 菜单、报告、字段名称等。
Workfront管理员可以使用布局模板功能重命名问题项，以匹配其组织的术语。 然后，新术语会出现在整个 [!DNL Workfront] 适用于那些已分配到布局模板的用户。

![[!UICONTROL Terminology] 窗口 [!UICONTROL Issue] 突出显示](assets/admin-fund-issue-custom-terminology.png)

<!---
paragraph below needs a hyperlink
--->

了解系统和组管理员如何在学习路径（新版管理员基础知识）中创建布局模板 [!DNL Workfront] 体验：第3部分控制和界面体验。

<!---
learn more URLs
Create and manage layout templates
--->
