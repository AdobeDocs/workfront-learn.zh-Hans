---
title: 编辑自动化工作流模板
description: 了解如何更改中的现有自动验证工作流模板 [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 编辑自动化工作流模板

随着校样审核和批准流程的完善或组织更改的进行，自动化工作流模板应该更新，以反映使用Workfront的团队的当前操作。

使模板保持最新可确保审核和批准流程的一致性，并且无需不断调整工作流，从而节省上传校样的时间。

1. 选择 **[!UICONTROL Proofing]** 从 **[!UICONTROL Main Menu]** 在 [!DNL Workfront].
1. 从该位置，选择 **[!UICONTROL Workflows]** （在左侧面板菜单中）。
1. 单击模板名称最右侧的三个圆点菜单，然后选择 **[!UICONTROL View template details]**.

共享、复制和删除模板的选项跨每个模板的模板详细信息窗口的顶部。 删除模板不会影响已应用该模板的正在进行中的验证，但这意味着该模板将无法再使用。

![模板详细信息窗口](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

单击箭头以展开 [!UICONTROL Details] 部分，以更改模板名称或模板时区等。

## 对阶段和收件人进行更改

中可能需要更改 [!UICONTROL Workflow] 区域，此时简化的流程意味着更早的截止日期，或者当有人加入团队并将审核验证时。

自动化工作流的每个阶段都有其自己的部分，从而允许单独修改截止日期、隐私、验证收件人和其他信息。

此视频简要演示了您可在以下内容中进行的一些更改： [!UICONTROL Workflow] 区域。 请参阅此视频下的项目符号列表，其中会审核这些设置。 此视频中没有音频。

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

作为审核，以下是您可以在中进行的验证模板更改 [!UICONTROL Workflow] 部分：

* 单击 [!UICONTROL stage name] 字段或 [!UICONTROL deadline] 字段以更新该信息。
* 选择旁边的箭头 [!UICONTROL deadline] 要锁定舞台，请确定何时激活舞台，或者只需一个决定。
* 在收件人列表中，单击 [!UICONTROL Role] 或 [!UICONTROL Email alerts] 字段以选择其他选项。
* 转到收件人姓名最右侧的3个圆点菜单，从列表中删除他们，让他们成为该工作流阶段的主要决策者，或编辑验证角色和电子邮件警报信息。
* 您有两个选项可以将收件人添加到列表。 打开 [!UICONTROL Add people to stage] 窗口中，单击将它们添加到哪个阶段。 然后，在收件人列表中输入其姓名或电子邮件地址，并分配验证角色和电子邮件警报。 单击 [!UICONTROL Add people] 按钮。
   1. 在每个舞台部分的右上角，转到 [!UICONTROL More] 菜单并选择 [!UICONTROL Add people to stage].
   1. 在顶部 [!UICONTROL Workflow] 区域，选择 [!UICONTROL Add people to stage].

## 模板共享

此 [!UICONTROL Shared With] 区域显示可以使用模板的验证用户。 通过单击姓名最右侧的3点菜单并选择 [!UICONTROL Remove].

![[!UICONTROL Shared With] 列表](assets/proof-system-setups-edit-template-shared-with.png)

但是，您无法从此分区将人员添加到共享列表。 要执行此操作，请返回模板详细信息窗口的顶部，然后单击 [!UICONTROL Share template] 按钮。

## 活动部分

[!DNL Workfront] 保留对模板进行更改时的审核历史记录。 您可以查看更改日期、更改人员和更改内容的简要信息。

此部分不记录有关何时在验证上使用模板的信息。

![校对活动列表](assets/proof-system-setups-edit-template-activity.png)
