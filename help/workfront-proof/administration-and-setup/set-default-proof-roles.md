---
title: 设置默认验证角色
description: 了解如何设置在创建新用户或人们打开校样时分配的默认校样角色。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 52%

---

# 设置默认验证角色



要完成的第一个默认设置是确定在创建新用户或人们打开校样时将分配的默认验证角色。

验证角色决策了用户能够对校样采取什么操作——只查看它、发表评论、审批它等等。[!DNL Workfront] 建议为所有用户设置验证角色默认值，以便更快、更轻松地将收件人添加到校样中并设置工作流。

![上传校样时可以选择验证角色](assets/proof-system-setups-proof-role-example.png)

但是，这个默认的验证角色可以在上传单个校样时进行更改，以确保每个人都能够在审核和审批过程中履行其所需的角色。


## 设置默认验证角色

1. 从 [!UICONTROL Main Menu] 中选择&#x200B;**设置。**
1. 从左侧菜单选择&#x200B;**审核及审批。**
1. 单击两个新角色所需的默认验证角色旁边的按钮 [!DNL Workfront] “指定收件人”的用户和访客验证用户 — 手动或通过工作流模板添加到验证工作流中的任何人员。
1. 单击两个新角色所需的默认验证角色旁边的按钮 [!DNL Workfront] “非收件人”用户的用户和访客验证用户。 这些规则一般是 [!DNL Workfront] 有权访问验证但不是分配到工作流的人员之一的用户。
1. 保存更改。

![Workfront 中的审核和审批设置](assets/proof-system-setups-workfront-defaults.png)

考虑一下，当您的大多数用户和访客被添加到验证工作流中时，他们应该做什么。这应该是您的默认值。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 对Workfront中的“打开文档验证的非收件人角色”设置使用“只读”或“查看者”。 | 此设置的其他选项都需要做出校对决定，这可能会破坏您的校对工作流。 通常，未添加到验证工作流的人只需要查看验证或发表评论，而不会实际审批验证，因此“只读”或“查看者”选项是您的最佳选择。 <br> <br>注意：此设置可在Workfront主菜单>设置>审阅和批准中找到。 |
