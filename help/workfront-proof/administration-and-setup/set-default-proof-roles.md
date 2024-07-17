---
title: 设置默认验证角色
description: 了解如何设置在创建新用户或人们打开验证时分配的默认验证角色。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 100%

---

# 设置默认验证角色



要完成的第一个默认设置是确定在创建新用户或人们打开验证时将分配的默认验证角色。

验证角色决定了用户能够对验证采取什么操作——只查看它、发表评论、审批它等等。[!DNL Workfront] 建议为所有用户设置验证角色默认值，以便更快、更轻松地将收件人添加到验证中并设置工作流。

![上传验证时可以选择验证角色](assets/proof-system-setups-proof-role-example.png)

但是，这个默认的验证角色可以在上传单个验证时进行更改，以确保每个人都能够在审核和审批过程中履行其所需的角色。


## 设置默认验证角色

1. 从 [!UICONTROL Main Menu] 中选择&#x200B;**设置**。
1. 从左侧菜单选择&#x200B;**审核及审批**。
1. 单击新 [!DNL Workfront] 用户和“指定收件人”（手动或通过工作流模板添加到验证工作流的任何人）的访客验证用户所需的默认验证角色旁边的按钮。
1. 单击新 [!DNL Workfront] 用户和“非收件人”访客验证用户所需的默认验证角色旁边的按钮。这些用户通常是有权访问验证的 [!DNL Workfront] 用户，但并未分配到工作流的人员。
1. 保存更改。

![Workfront 中的审核和审批设置](assets/proof-system-setups-workfront-defaults.png)

考虑一下，当您的大多数用户和访客被添加到验证工作流中时，他们应该做什么。这应该是您的默认值。

## 最佳实践

| 最佳实践 | 原因如下 |
|---|---|
| 对于 Workfront 中的“打开文档验证的非收件人的角色”设置，仅使用“只读”或“审核人”。 | 此设置的其他选项都需要作出验证决策，而这可能会破坏您的验证工作流。通常情况下，未添加到验证工作流的人员只需要查看验证或发表评论，而不需要实际审批验证，因此“只读”或“审核人”选项是您的最佳选择。<br> <br>注释：此设置可在 Workfront 主菜单 > 设置 > 审核及审批中找到。 |
