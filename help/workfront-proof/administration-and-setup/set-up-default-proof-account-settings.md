---
title: 设置验证帐户默认设置
description: 了解如何设置全局应用于所有校样和验证用户的默认帐户设置。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 57%

---

# 设置验证帐户默认设置

建立全局应用于所有校样和校样用户的默认帐户设置（国家/地区、语言和时区）。如果您的用户跨多个时区或国家/地区，则可以根据需要在每个人的用户配置文件中调整这些设置。

![用于验证的帐户设置窗口](assets/proof-system-setups-default-account-settings.png)

1. 从 [!DNL Workfront's] [!UICONTROL Main Menu] 中选择 **[!UICONTROL Proofing]**。
1. 在顶部导航栏中选择 **[!UICONTROL Account Settings]**。
1. 选择 **[!UICONTROL Details]** 选项卡。
1. 前往 [!UICONTROL Country] 字段，并选择 **[!UICONTROL Edit]**。选择大多数验证用户所在的国家/地区作为默认国家/地区。
1. 为该设置选择 **[!UICONTROL Save]**。
1. 前往 [!UICONTROL Default language] 字段，并选择 **[!UICONTROL Edit]**。选择大多数验证用户将会使用的语言作为默认语言。
1. 为该设置选择 **[!UICONTROL Save]**。
1. 前往 [!UICONTROL Time zone default] 字段，并选择 **[!UICONTROL Edit]**。选择大多数验证用户所在的时区作为默认时区。这将是手动设置的校样工作流所识别的时区。它也适用于校样工作流模板，但每个模板都可以设置时区。
1. 为该设置选择 **[!UICONTROL Save]**。

## 最佳实践


| 最佳实践 | 原因如下 |
|---|---|
| 调整校样后端设置，以便用户看到 12 小时制格式的截止日期。 | 对于想要以 AM/PM 格式查看校样截止日期/时间的用户，请在校样设置中选择 F j, Y, gi:a 选项。对于使用12小时制的地区，这有助于明确截止日期。 <br> <br>注意：通过转到Workfront主菜单>校样>帐户设置>用户>并编辑每个用户的日期格式字段，可找到此设置。 |
| 作为系统设置的一部分设立默认的验证期限。 | 当设置默认验证截止时间（上传日期+ x个工作日）时，如果验证创建者忘记添加截止时间，Workfront会自动将此截止时间应用于上传的每个验证。 <br> <br>注意：通过转到Workfront主菜单>验证>帐户设置>设置>验证默认值>截止日期（+工作日）字段可找到此设置。 |
| 隐藏不相关验证决策选项。 | 此决策选项通常会导致审批人感到困惑，因为组织通常不会定义何时应使用“不相关”选项。“不相关”选项通常表示该验证与验证收件人不相关，并且他们不需要做出审批或拒绝的决策。通过选择不相关，这将允许验证工作流继续。<br> <br>在大多数验证工作流中，不需要不相关的选项。<br> <br>注意：通过转到Workfront主菜单>校样>帐户设置>决策可找到此设置。 |
| 请勿在校样设置中重新排序校样决策选项。 | 每个验证决策设置都有一个特定的值/权重，如果重新排序，这可能会混淆验证配置。决策顺序和值/权重用作验证阶段激活触发器和报告。<br> <br>注意：通过转到Workfront主菜单>校样>帐户设置>决策可找到此设置。 |
| 设置验证角色和电子邮件提醒的用户默认值。 | 在分配验证工作流时，这些设置会自动填充，从而加快流程速度，并促进跨验证工作流的一致性。<br> <br>注意：转到Workfront主菜单>校样>帐户设置>用户>并选择要为其设置默认值的用户，可找到用户默认设置。 |
