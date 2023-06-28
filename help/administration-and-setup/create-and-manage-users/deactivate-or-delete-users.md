---
title: 何时以及如何停用或删除用户
description: 了解停用和删除用户之间的区别。 然后，根据贵组织的需求管理用户配置文件。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10037.jpeg
jira: KT-10037
exl-id: 89b7d083-97d3-4783-a61d-35226d6582c0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# 何时以及如何停用或删除用户

当用户离开组织或不再使用 [!DNL Workfront]，您将需要取消激活其登录信息。 仅应在特定情况下删除用户配置文件。

## 停用

停用用户会将许可证从用户的配置文件中删除，因此他们无法再登录或访问 [!DNL Workfront]. 他们的许可证可分配给另一个用户。

不能为已停用的用户分配新工作，但是他们仍将分配给任何现有工作。

例如，自由职业者已完成特定项目的工作，因此您希望取消激活其登录，直到下次需要他们时。

## 删除

在极少数情况下（例如意外登录或测试用户），可能需要从删除用户登录 [!DNL Workfront]. 删除用户将删除该用户与中的项目的关联 [!DNL Workfront] — 工作分配、注释、小时、文档、它们创建的对象等。

此 **仅限** 时间 [!DNL Workfront] 如果用户从未被分派工作，或绝对没有使用Workfront项目的历史记录，则建议删除用户。

[!DNL Workfront] **强烈** 建议停用用户而不是删除用户。 停用会保留用户信息 [!DNL Workfront]，这可用于准确报告、项目管理等。 如果您对是否应该停用或删除用户有任何疑问，请联系您的 [!DNL Workfront] 顾问或 [!DNL Workfront] 客户支持。

![更多菜单显示选项 [!DNL Users] 页面](assets/admin-fund-adding-users-11.png)

### 停用或删除用户

1. 选择 **[!UICONTROL Users]** 从 [!UICONTROL Main Menu].
1. 通过选中用户名称旁边的框来选择用户。
1. 单击 **[!UICONTROL More]** 下拉菜单。
1. 选择 **[!UICONTROL Deactivate]** 或 **[!UICONTROL Delete]**.
