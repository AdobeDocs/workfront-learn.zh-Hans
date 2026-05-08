---
title: 设置校样帐户默认设置
description: 了解如何设置全局应用于所有校对和校对用户的默认帐户设置。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:04:10.059Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 551
ht-degree: 95%

---

# 设置校样帐户默认设置

建立全局应用于所有校对和校对用户的默认帐户设置（国家/地区、语言和时区）。 如果您的用户跨越多个时区或国家/地区，则可以根据需要在每个人的用户配置文件上调整这些设置。

![用于校对的帐户设置窗口](assets/proof-system-setups-default-account-settings.png)

1. 从 [!DNL Workfront's] [!UICONTROL Main Menu] 中选择 **[!UICONTROL Proofing]**。
1. 在顶部导航栏中选择 **[!UICONTROL Account Settings]**。
1. 选择 **[!UICONTROL Details]** 选项卡。
1. 前往 [!UICONTROL Country] 字段，并选择 **[!UICONTROL Edit]**。 选择大多数校对用户所在的国家/地区作为默认国家/地区。
1. 为该设置选择 **[!UICONTROL Save]**。
1. 前往 [!UICONTROL Default language] 字段，并选择 **[!UICONTROL Edit]**。 选择大多数校对用户将会使用的语言作为默认语言。
1. 为该设置选择 **[!UICONTROL Save]**。
1. 前往 [!UICONTROL Time zone default] 字段，并选择 **[!UICONTROL Edit]**。 选择大多数校对用户所在的时区作为默认时区。 这将是手动设置的校样工作流所识别的时区。 它也适用于校样工作流模板，但每个模板都可以设置时区。
1. 为该设置选择 **[!UICONTROL Save]**。

## 最佳实践


| 最佳实践 | 原因如下 |
|---|---|
| 调整校样后端设置，以便用户看到 12 小时制格式的截止日期。 | 对于希望以AM/PM格式查看验证截止时间/时间的用户，在验证设置中选择F j、Y、gi:a选项。 对于使用 12 小时制的地区，这有助于明确截止日期。<br> <br>注释：此设置可通过前往 Workfront 主菜单 > 校对 > 帐户设置 > 用户 > 并编辑每个用户的日期格式字段找到。 |
| 作为系统设置的一部分设立默认的校样期限。 | 设置默认校样截止日期后（上传日期 + x 个工作日），如果校样创建者忘记添加截止日期，则 Workfront 会自动将此截止日期应用于上传的每个校样。<br> <br>注释：可通过前往 Workfront 主菜单 > 校对 > 帐户设置 > 设置 > 校对默认值 > 截止日期（+ 工作日）字段找到此设置。 |
| 隐藏不相关校样决策选项。 | 此决策选项通常会导致审批人感到困惑，因为组织通常不会定义何时应使用“不相关”选项。 “不相关”选项通常表示该校样与校样收件人不相关，并且他们不需要作出审批或拒绝的决策。 通过选择“不相关”，可以继续进行校样工作流。<br> <br>大多数校样工作流中均不需要“不相关”选项。<br> <br>注释：可通过转至 Workfront 主菜单 > 校对 > 帐户设置 > 决策来找到此设置。 |
| 请勿在校样设置中重新排序校样决策选项。 | 每个校样决策设置都有一个特定的值/权重，如果重新排序，这可能会混淆校样配置。 决策顺序和值/权重可用作校样阶段激活触发器，并且也可以在报告中使用。<br> <br>注释：可通过转至 Workfront 主菜单 > 校对 > 帐户设置 > 决策来找到此设置。 |
| 设置校样角色和电子邮件提醒的用户默认值。 | 分配校样工作流时，这些设置会自动填充，从而加快流程，并有助于保持整个校样工作流中的一致性。<br> <br>注释：通过转至 Workfront 主菜单 > 校对 > 帐户设置 > 用户 > 并选择要设置默认值的用户，可以找到用户默认设置。 |
