---
title: 编辑自动化工作流模板
description: 了解如何在 [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 编辑自动化工作流模板

随着校样审核和批准流程的细化或组织更改的进行，应更新自动化的工作流模板，以反映使用Workfront的团队的当前操作。

将模板保持为最新可确保审核和批准流程的一致性，并为这些上传校样节省时间，因为它们不必不断调整工作流。

1. 选择 **[!UICONTROL Proofing]** 从 **[!UICONTROL Main Menu]** in [!DNL Workfront].
1. 从此处，选择 **[!UICONTROL Workflows]** 菜单。
1. 单击模板名称最右侧的3个圆点菜单，然后选择 **[!UICONTROL View template details]**.

用于共享、复制和删除模板的选项位于每个模板详细信息窗口的顶部。 删除模板不会影响正在应用该模板的校样，但它确实意味着模板不再可用。

![“模板详细信息”窗口](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

单击箭头可展开 [!UICONTROL Details] 部分来更改模板名称或模板时区等内容。

## 更改阶段和收件人

可能需要在 [!UICONTROL Workflow] 区域。

自动化工作流的每个阶段都有其自己的部分，该部分允许单独修改截止时间、隐私、校样收件人和其他信息。

此视频简要演示了您在 [!UICONTROL Workflow] 的上界。 请参阅此视频下的项目符号列表，该列表将回顾这些设置。 此视频上没有音频。

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

作为回顾，以下是您可以在 [!UICONTROL Workflow] 部分：

* 单击 [!UICONTROL stage name] 字段或 [!UICONTROL deadline] 字段来更新该信息。
* 选择 [!UICONTROL deadline] 要锁定舞台，请确定舞台何时被激活，或者只需要一个决策。
* 在收件人列表中，单击 [!UICONTROL Role] 或 [!UICONTROL Email alerts] 字段以选择其他选项。
* 转到收件人姓名最右侧的3个圆点菜单，以从列表中删除收件人，使其成为该工作流阶段的主要决策者，或编辑校样角色和电子邮件警报信息。
* 有两个选项可向列表添加收件人。 打开 [!UICONTROL Add people to stage] 窗口中，单击要将其添加到的阶段。 然后，在收件人列表中输入其名称或电子邮件地址，并分配校样角色和电子邮件警报。 单击 [!UICONTROL Add people] 按钮。
   1. 在每个阶段部分的右上角，转到 [!UICONTROL More] 菜单和选择 [!UICONTROL Add people to stage].
   1. 在 [!UICONTROL Workflow] 区域，选择 [!UICONTROL Add people to stage].

## 模板共享

的 [!UICONTROL Shared With] 区域会显示可以使用模板的校样用户。 单击模板最右侧的3个圆点菜单，然后选择，可删除不再需要使用模板的用户 [!UICONTROL Remove].

![[!UICONTROL Shared With] 列表](assets/proof-system-setups-edit-template-shared-with.png)

但是，您无法从此部分将人员添加到共享列表。 为此，请返回到模板详细信息窗口的顶部，然后单击 [!UICONTROL Share template] 按钮。

## 活动部分

[!DNL Workfront] 会保留对模板进行更改的审核历史记录。 您可以查看更改的日期、做出更改的人员，以及有关所做更改的简短信息。

此部分不记录有关何时将模板用于校样的信息。

![校样活动列表](assets/proof-system-setups-edit-template-activity.png)
