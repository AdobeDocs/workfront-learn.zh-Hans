---
title: 复制现有目标
description: 了解如何在  [!DNL Workfront Goals] 中复制现有目标。
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 100%

---

# 复制现有目标

假设现在是一个季度末，您想为下一个季度重新创建一个现有的目标。或者也许您没有完成目标，并需要将其延长到下一个时间段。创建这一目标的最佳选择是什么？您需要复制并修改现有目标。

如果多个团队成员有相似的目标并且您需要为每个人创建一个目标，则复制现有目标也会很有帮助。

<!--
Pro-tips graphic
-->

在复制目标之前需要考虑以下几点：

* 原始目标的所有信息都会被复制，但目标期间除外（因为这已经过去）。
* 您可以复制现有目标的结果，它们会转移到新的目标。
* 默认情况下，复制的结果会分配给同一所有者。
* 您无法将现有目标的进度复制到新目标。
* 复制目标时无法复制目标的活动。

## 如何复制目标

1. 单击目标名称以打开 **[!UICONTROL Goal Details]** 面板。
1. 单击三点图标，然后选择 **[!UICONTROL Copy]**。
1. 更新所复制的目标的以下任何信息：
   * **新名称**——这是新目标的名称。其默认为原始目标的名称。
   * **期间**——您想要实现目标的时段。从下拉菜单中选择一个时段，或单击“定义自定义日期”以指示自定义时段。默认时段始终是当前季度。
   * **所有者**——目标的所有者。这可以是用户、团队、组或公司。其默认为原始目标的所有者。
   * **描述**——有关目标的附加信息。

1. 如果原始目标已添加结果并且您想要将其复制到新目标，请勾选 **[!UICONTROL Copy results]** 框。复制的目标的结果与原始目标的结果具有相同的所有者、名称和测量值。

1. 单击 **[!UICONTROL Save]**。复制的目标会以草稿状态保存。

   ![[!DNL Workfront Goals] 中 [!UICONTROL Goal Details] 面板的图像，其中显示了 [!UICONTROL Copy] 选项](assets/03-workfront-goals-copy-a-goal.png)

1. 单击 **[!UICONTROL Activate]**，这会将目标状态更新为“活动”。目标必须有相关的活动或结果才能“激活”。

1. 单击 [!UICONTROL Goal Details] 面板右上角的 **X** 以关闭它。

如果您复制了之前时段内未完成的目标，并希望在接下来的时段内继续实现该目标，请执行以下操作：

1. 转到 **[!UICONTROL Goal List]**、**[!UICONTROL Check-in]** 或 **[!UICONTROL Pulse]** 部分中的原始目标。
1. 对目标进行评论以表明它已被复制并创建了更新的目标。
1. 关闭原始目标以保留在原始时段内取得的进展。单击 **[!UICONTROL Goal Details]** 面板中的三点图标，并从菜单中选择 **[!UICONTROL Close]**。
1. 更新新结果的 [!UICONTROL Initial] 值，以匹配之前的结果的 **[!UICONTROL Target]** 值，这样您新目标的进度将会从上一阶段实现的目标阶段开始计算。
